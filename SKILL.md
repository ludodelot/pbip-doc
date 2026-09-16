---
name: pbip-documentation
description: Generate documentation for a Power BI Project (PBIP) by reading its TMDL and PBIR files directly and writing Markdown docs — semantic model reference, measure/DAX catalog, report page inventory, and a quality report (orphans, circular dependencies, missing descriptions). Use when the user asks to document, explain, or audit a PBIP/Power BI project folder, or to summarize its tables, measures, or reports.
---

# PBIP Documentation

Reads a Power BI Project (PBIP) folder's TMDL/PBIR source files directly and
writes human-readable Markdown documentation. There is no CLI and no npm
package — this skill's instructions ARE the tool: follow them to read the
project files yourself and author the docs.

## When to use this

The user points you at a PBIP project folder (or a `.SemanticModel` /
`.Report` subfolder) and asks for documentation, an overview, an audit, or an
explanation of its tables, measures, relationships, or report pages.

## Expected input layout

A PBIP project usually looks like:

```
my-project/
├── MyModel.SemanticModel/
│   └── definition/
│       ├── model.tmdl
│       ├── relationships.tmdl
│       ├── tables/
│       │   ├── Sales.tmdl
│       │   └── Customer.tmdl
│       └── ...
└── MyModel.Report/
    ├── definition.pbir
    └── definition/
        ├── report.json          (or pages/ in newer layouts)
        └── pages/
            └── <pageId>/
                ├── page.json
                └── visuals/
```

Older exports may use `report.json` / `.pbi\localSettings.json` style
(TMSL/PBIR-legacy) instead of `.tmdl` files. If you don't find `.tmdl`
files, look for `model.json`/`report.json` and adapt — the concepts below
still apply, just read JSON instead of TMDL text.

If none of these files exist under the given path, say so plainly and stop;
do not invent structure.

## Procedure

1. **Locate the project.** Find the `.SemanticModel` and `.Report` folders
   (or confirm the given path already points at one). Use Glob to find all
   `*.tmdl`, `*.pbir`, and `page.json`/`report.json` files before reading
   any of them, so you know the real scope.

2. **Read the semantic model** (`definition/model.tmdl`, `tables/*.tmdl`,
   `relationships.tmdl`, `cultures/*.tmdl` if present). TMDL is an indented,
   YAML-like text format. For each table extract:
   - Columns (name, dataType, isHidden, formatString, sourceColumn)
   - Measures (name, `expression` block containing the DAX, formatString,
     isHidden, displayFolder)
   - Partitions / source query (M / Power Query) if present
   For `relationships.tmdl` extract each relationship's fromTable/fromColumn,
   toTable/toColumn, cardinality, and crossFilteringBehavior.

3. **Analyze DAX per measure.** For every measure's expression, note:
   - Other measures/columns it references (by scanning identifiers used
     inside the expression against the model's known measure/column names)
   - Whether it uses time-intelligence functions (`CALCULATE`, `DATEADD`,
     `SAMEPERIODLASTYEAR`, `TOTALYTD`, etc.)
   - Rough complexity: count nested iterator functions (`SUMX`, `FILTER`,
     `CALCULATE` inside another) — call it LOW (0-1 nesting), MEDIUM (2),
     HIGH (3+). This is a heuristic, not a benchmarked metric — say so if
     asked.

4. **Build a lineage picture.** From the measure-reference scan and
   relationships, note for each table/measure what depends on it
   (downstream) and what it depends on (upstream). Flag:
   - **Orphans**: measures/columns never referenced by another measure,
     visual, or relationship.
   - **Circular references**: measure A's expression references measure B
     which references A (directly or transitively).
   Only report these as findings if you actually traced the reference —
   don't guess.

5. **Read the report layer** (`.Report/definition/pbir` or
   `report.json`, and each page's `page.json`). For each page collect its
   display name and the visuals on it (visual type + the fields/measures
   each visual is bound to, from its `query`/`prototypeQuery` section).

6. **Write the docs.** Create the output folder the user asked for (default
   `./docs` next to the project) with this structure, generating only the
   sections you have real data for:

   ```
   docs/
   ├── index.md              # Project name, table/measure/page counts, summary
   ├── semantic-model/
   │   ├── tables.md          # One section per table: columns, measures
   │   └── relationships.md   # Relationship list + a Mermaid ER diagram
   ├── dax/
   │   └── measures.md        # Every measure: expression, refs, complexity
   ├── reports/
   │   └── pages.md           # Page → visuals → bound fields
   └── quality.md              # Orphans, circular deps, missing descriptions
   ```

   Use a Mermaid `erDiagram` block for relationships.md built from the
   relationships you actually parsed — don't fabricate cardinalities.

7. **Report language.** If the user asks for documentation in a language
   other than English, translate the prose you write (summaries,
   descriptions) but never translate identifiers — table, column, and
   measure names must stay exactly as they appear in the source files.

## What this skill does NOT do

- No CLI, no npm package, no Docker image, no GitHub Action — those don't
  exist. If asked to run `pbip-doc generate`, explain that this is an
  agent skill, not an installable binary, and offer to run the procedure
  above instead.
- No claimed test coverage, performance benchmarks, or "enterprise grade"
  guarantees — none of that has been measured. If the user needs
  performance numbers, say they haven't been benchmarked.
- No database export, Slack/Discord notifications, or watch mode. These
  were aspirational and are not implemented; mention them only as
  possible future work if the user asks what's next.

## Tips

- Prefer several small Markdown files over one huge dump — one file per
  table if the model is large.
- If a project is large (100+ measures), ask the user whether they want
  full detail or a summarized pass before writing everything out.
- Always cite the source file (`tables/Sales.tmdl`, `page.json` under a
  given page id) inline or in a footer so findings are checkable against
  the real files.
