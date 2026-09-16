# PBIP Documentation Skill

A [Claude Code](https://claude.com/claude-code) skill that documents Power BI
Projects (PBIP). It has **no CLI and no npm package** — it works by having
the agent read your project's `.tmdl`/`.pbir` source files directly and write
Markdown documentation, following the procedure in [SKILL.md](SKILL.md).

## What it does

Given a PBIP project folder, the skill:

- Reads the semantic model (`*.tmdl`: tables, columns, measures,
  relationships) and the report layer (`*.pbir`, `page.json`)
- Traces which measures reference which other measures/columns, to flag
  orphan entities and circular DAX references
- Writes Markdown docs: a project overview, per-table/measure reference,
  a report page → visual inventory, and a quality report
- Can write the prose in a language you request (table/column/measure names
  are never translated)

Everything above happens through the agent reading files and writing
Markdown — there is no compiled parser, no knowledge graph database, no
watch mode, and no benchmarked performance numbers. See
[SKILL.md](SKILL.md) for the exact procedure and its current limitations.

## Installation

Copy `SKILL.md` into your project's `.claude/skills/pbip-documentation/`
directory (or wherever your Claude Code setup loads skills from), or point
Claude Code at this repo directly.

## Usage

Ask Claude Code, e.g.:

> Using the pbip-documentation skill, document the PBIP project in
> `./my-report`.

Claude will locate the `.SemanticModel`/`.Report` folders, read the TMDL and
PBIR files, and write the docs described in [SKILL.md](SKILL.md#procedure).

## Status

This is a working agent skill, not a packaged product. There is no released
binary, npm package, Docker image, or GitHub Action — earlier versions of
this README described those as if they existed; they didn't. If you want
any of that, it would need to be built from scratch (tracked as future
work, not a promise).

## License

MIT License. See [LICENSE](LICENSE).
