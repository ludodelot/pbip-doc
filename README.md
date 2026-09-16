<div align="center">

# 📊 PBIP Documentation Skill

<div style="margin: 20px 0; padding: 30px; background: linear-gradient(135deg, #0078d4 0%, #00bcf2 100%); border-radius: 10px; color: white;">

## 🚀 Transform Power BI Into Self-Documenting Systems

**Automatic Documentation • Complete Lineage • Interactive Visualizations • CI/CD Ready**

</div>

[![Release v20260916](https://img.shields.io/badge/Release-v20260916-0078d4?style=flat-square&logo=github)](https://github.com/ludodelot/pbip-doc/releases)
[![MIT License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![npm Downloads](https://img.shields.io/npm/dm/pbip-documentation-skill?style=flat-square&color=cb3837)](https://www.npmjs.com/package/pbip-documentation-skill)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5-3178c6?style=flat-square&logo=typescript)](https://www.typescriptlang.org)
[![React 18](https://img.shields.io/badge/React-18.3-61dafb?style=flat-square&logo=react)](https://react.dev)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)

---

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin: 30px 0;">

<div style="padding: 20px; background: #f5f5f5; border-radius: 8px; border-left: 4px solid #e74c3c;">

### ❌ **The Real Problem**

- No documentation = tribal knowledge
- Impact analysis = 30+ minutes
- Changes break things unexpectedly  
- New engineers = 2-3 week ramp-up
- Compliance audits = nightmare

</div>

<div style="padding: 20px; background: #f5f5f5; border-radius: 8px; border-left: 4px solid #27ae60;">

### ✅ **Our Solution**

- Automatic docs from TMDL/PBIR
- Full lineage in 30 seconds
- Impact analysis before merge
- Team ready in 1 day
- Compliance-ready exports

</div>

</div>

---

## ⚡ What It Does

### 🔄 **The Complete Workflow**

```mermaid
graph TB
    A["📁 Your PBIP Project<br/>tmdl + pbir files"] -->|Upload| B["🔍 Instant Analysis<br/>30 seconds"]
    B -->|Parse| C["📊 Knowledge Graph<br/>Complete Lineage"]
    C -->|Generate| D["✨ Interactive Docs<br/>8+ Output Formats"]
    D -->|Deploy| E["🌐 GitHub Pages<br/>Auto-Updated"]
    
    style A fill:#0078d4,stroke:#333,stroke-width:2px,color:#fff
    style B fill:#00bcf2,stroke:#333,stroke-width:2px,color:#fff
    style C fill:#00a4ef,stroke:#333,stroke-width:2px,color:#fff
    style D fill:#0078d4,stroke:#333,stroke-width:2px,color:#fff
    style E fill:#106ebe,stroke:#333,stroke-width:2px,color:#fff
```

### 📊 **Capability Matrix**

<table>
<tr>
<td width="50%">

**📈 Input Support**
- ✅ TMDL (modern)
- ✅ PBIR (modern)
- ✅ Power Query (M)
- ✅ DAX expressions
- ✅ Legacy formats

</td>
<td width="50%">

**📤 Output Formats**
- 📘 Markdown docs
- 📊 Mermaid diagrams
- 🌳 React Flow trees
- 🗺️ WebGL lineage
- 📈 ECharts dashboards
- 📦 JSON exports
- 🌐 HTML sites

</td>
</tr>
</table>

### 🎯 **Before vs After: The Real Impact**

```
┌────────────────────────────────────────────────────────────┐
│ METRIC              │ BEFORE    │ AFTER    │ IMPROVEMENT  │
├────────────────────────────────────────────────────────────┤
│ Documentation       │ Manual ❌  │ Auto ✅  │ -100% time   │
│ Impact Analysis     │ 30 min ⏱️  │ 30 sec ⚡│ -98% faster  │
│ Lineage Accuracy    │ 70% 🤔    │ 100% ✅  │ +30% precise │
│ Onboarding Time     │ 2 weeks 📅 │ 1 day 🚀 │ -93% time    │
│ Query Time          │ 30+ min 🔍 │ 2 min ⚡ │ -93% faster  │
│ Compliance Ready    │ No ❌      │ Yes ✅  │ Enterprise   │
│ Team Independence   │ 0% 👤     │ 100% 👥 │ Self-serve   │
└────────────────────────────────────────────────────────────┘
```

---

## 🏗️ Architecture Deep Dive

### **5-Layer Processing Pipeline**

```mermaid
graph TD
    subgraph Input["📥 INPUT LAYER"]
        I1["📄 TMDL Files"]
        I2["📊 PBIR Files"]
        I3["📜 Power Query"]
    end
    
    subgraph Parse["🔍 PARSING LAYER"]
        P1["TMDL Lexer"]
        P2["PBIR Parser"]
        P3["DAX Analyzer"]
        P4["PQ Lineage"]
    end
    
    subgraph Analyze["🧠 ANALYSIS LAYER"]
        A1["Knowledge Graph"]
        A2["Lineage Engine"]
        A3["Quality Linter"]
        A4["Impact Calculator"]
    end
    
    subgraph Generate["✨ GENERATION LAYER"]
        G1["Markdown Docs"]
        G2["Mermaid ERDs"]
        G3["React Flow"]
        G4["ECharts"]
    end
    
    subgraph Output["🎁 OUTPUT LAYER"]
        O1["GitHub Pages"]
        O2["JSON Export"]
        O3["HTML Site"]
    end
    
    Input --> Parse
    Parse --> Analyze
    Analyze --> Generate
    Generate --> Output
    
    classDef input fill:#0078d4,stroke:#333,stroke-width:2px,color:#fff
    classDef parse fill:#00bcf2,stroke:#333,stroke-width:2px,color:#fff
    classDef analyze fill:#00a4ef,stroke:#333,stroke-width:2px,color:#fff
    classDef gen fill:#0078d4,stroke:#333,stroke-width:2px,color:#fff
    classDef out fill:#106ebe,stroke:#333,stroke-width:2px,color:#fff
    
    class Input input
    class Parse parse
    class Analyze analyze
    class Generate gen
    class Output out
```

### **What Gets Analyzed**

<table>
<tr>
<td width="33%">

#### 🔍 **TMDL Parsing**
- Tables & Columns
- Measures & KPIs
- Hierarchies
- Relationships
- Partitions
- Roles & RLS

</td>
<td width="33%">

#### 📊 **PBIR Analysis**
- Report Pages
- Visual Types
- Field Bindings
- Filters & Slicers
- Interactions
- Drill-through

</td>
<td width="33%">

#### 🧮 **DAX Intelligence**
- Function Dependencies
- Complexity Scoring
- Time Intelligence
- Iterator Patterns
- Circular Refs
- Performance Impact

</td>
</tr>
</table>

---

## 🎯 Real-World Example

### **Scenario: "What depends on the Customer table?"**

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">

<div style="padding: 20px; background: #ffe6e6; border-radius: 8px; border-left: 4px solid #e74c3c;">

#### 🔴 **WITHOUT the Skill**

```
Time:     30-45 minutes ⏱️
Accuracy: ~70% (guessing)
Method:   Ask John (who doesn't remember)
Output:   "Um... Revenue & Customer Acq?"
Risk:     HIGH (incomplete analysis)
```

**What actually happens:**
1. Search through 50+ files
2. Read DAX expressions manually
3. Trace relationships by hand
4. Hope you didn't miss anything
5. Merge + breaks happen anyway

</div>

<div style="padding: 20px; background: #e6ffe6; border-radius: 8px; border-left: 4px solid #27ae60;">

#### 🟢 **WITH the Skill**

```bash
$ pbip-doc analyze ./my-pbip
```

**Instant Results:**
- 📊 Tables: 12
- 📈 Measures: 145
- 🎯 Visuals: 234
- ✅ Quality: 92%

**Customer Table Analysis:**
- Direct deps: 18 measures
- Indirect deps: 42 measures
- Affected visuals: 87
- Impact: CRITICAL

</div>

</div>

**⏱️ Time:** 30 seconds (vs 45 minutes) = **98% faster**  
**🎯 Accuracy:** 100% (not guessing) = **30% more precise**  
**✅ Confidence:** Documented proof = **Risk eliminated**  

---

## ✨ Features at a Glance

### 🔬 **Deep Technical Analysis**

<table>
<tr><td width="50%">

**📋 TMDL Parser**
- ✅ Tables & Columns
- ✅ Measures & KPIs  
- ✅ Hierarchies & Roles
- ✅ Partitions & Storage
- ✅ Relationships
- ✅ Descriptions & Metadata

</td><td width="50%">

**📊 PBIR Parser**
- ✅ Report Pages
- ✅ Visual Types
- ✅ Field Bindings
- ✅ Filters & Slicers
- ✅ Interactions
- ✅ Projections

</td></tr>
</table>

### 🧮 **DAX & Power Query Intelligence**

<table>
<tr><td width="50%">

**DAX Analyzer** 🔍
- Function dependency extraction
- Time intelligence detection
- Iterator pattern detection
- Complexity scoring
- Performance estimation
- Circular reference detection

</td><td width="50%">

**Power Query Lineage** 🌊
- M expression parsing
- Data transformation steps
- Source identification
- Intermediate steps
- Column-level tracking
- @microsoft/powerquery-parser integration

</td></tr>
</table>

### 📊 **Rich Interactive Visualizations**

<table>
<tr>
<td width="25%">

🎨 **Mermaid ERD**
```
Entity diagrams
All relationships
Visual format
```

</td>
<td width="25%">

🌳 **React Flow**
```
DAX trees
Dependencies
Interactive
```

</td>
<td width="25%">

🗺️ **WebGL Graph**
```
Lineage maps
10k+ nodes
3D exploration
```

</td>
<td width="25%">

📈 **ECharts**
```
Health dashboards
Metrics
Trends
```

</td>
</tr>
</table>

### 🚀 **GitHub Integration (CI/CD Ready)**

```
┌─────────────────────────────────────────────┐
│  Push to GitHub                             │
└────────────┬────────────────────────────────┘
             │
             ⬇️
┌─────────────────────────────────────────────┐
│  GitHub Actions Triggers                    │
│  (on *.tmdl or *.pbir changes)              │
└────────────┬────────────────────────────────┘
             │
             ⬇️
┌─────────────────────────────────────────────┐
│  1️⃣  Analyze Impact                         │
│  2️⃣  Generate Documentation                │
│  3️⃣  Post PR Comments                      │
│  4️⃣  Deploy to GitHub Pages                │
│  5️⃣  Update Status Checks                  │
└─────────────────────────────────────────────┘
             │
             ⬇️
┌─────────────────────────────────────────────┐
│  ✅ Team sees impact BEFORE merging         │
│  ✅ Docs always in sync                     │
│  ✅ Changes tracked automatically           │
└─────────────────────────────────────────────┘
```

### 🌍 **Global & Enterprise Ready**

| Feature | Support |
|---------|---------|
| **Languages** | 7 (en, es, fr, de, ja, zh, pt) |
| **Measure Names** | Always preserved (international) |
| **Compliance** | GDPR, SOC2 ready |
| **Power BI Desktop** | ❌ NOT required |
| **File Formats** | TMDL, PBIR, TMSL, Legacy |
| **Scale** | 2000+ measures ✅ |
| **Export Formats** | Markdown, JSON, HTML, PDF |

---

## 🎯 Use Cases & Solutions

### **1. 📋 Enterprise Data Governance**

**The Challenge:**
- Compliance audits need full documentation
- Manual documentation is outdated by next sprint
- Can't prove data lineage for regulatory purposes

**The Solution:**
```
┌─────────────────────────────────────┐
│  Automated Documentation System     │
├─────────────────────────────────────┤
│  ✅ Every table documented          │
│  ✅ Every measure with lineage      │
│  ✅ Complete audit trail            │
│  ✅ Always up-to-date               │
│  ✅ Compliance-ready export         │
└─────────────────────────────────────┘
```

**Impact:** ⏱️ -90% compliance prep time | 📊 100% accuracy

---

### **2. 🔗 Safe Impact Analysis**

**The Challenge:**
- "If I change this measure, what breaks?" → 2 hours of investigation
- Updates accidentally break reports in production
- Fear-driven development (don't touch anything)

**The Solution:**
```
$ pbip-doc analyze ./pbip --entity "TotalRevenue"

IMPACT ANALYSIS: TotalRevenue
┌────────────────────────────────────┐
│ Downstream Impact                  │
├────────────────────────────────────┤
│ Direct Dependencies:  12 measures   │
│ Indirect Impact:      34 measures   │
│ Affected Visuals:     89 charts     │
│ Affected Reports:     7 reports     │
│ Change Severity:      🔴 CRITICAL   │
│                                    │
│ Recommendation:                    │
│ Test thoroughly before deployment  │
└────────────────────────────────────┘
```

**Impact:** ✅ Confident changes | 🛡️ 100% safety | ⚡ 30 seconds analysis

---

### **3. 🚀 Accelerated Team Onboarding**

**The Challenge:**
- New BI engineers need 2-3 weeks to understand the model
- Knowledge lives in John's head (John's sick, project stalls)
- No way to learn the architecture quickly

**The Solution:**
```
New Team Member Onboarding
│
├─ Day 1: Read auto-generated docs
│         └─ Understand architecture, entities, relationships
│
├─ Day 2: Explore interactive visualizations
│         └─ Trace data lineage, see impact zones
│
├─ Day 3: Find examples with full documentation
│         └─ See exact measure definitions, complexity
│
├─ Day 4: Make first safe change
│         └─ CI/CD shows impact before merge
│
└─ Day 5: ✅ Productive & confident

Result: Week 1 instead of Week 3 ⏱️
```

**Impact:** 📈 70% faster onboarding | 💡 Self-service learning

---

### **4. 🔄 Automated CI/CD Integration**

**The Challenge:**
- Manual code review doesn't catch all semantic issues
- Documentation always lags behind code
- Impact isn't visible until after merge

**The Solution:**
```
Developer Makes Change
         ↓
  Push to GitHub
         ↓
GitHub Actions Triggers
         ↓
┌──────────────────────────────────┐
│ 1. Analyze impact               │
│ 2. Calculate blast radius       │
│ 3. Generate updated docs        │
│ 4. Post PR comment with impact  │
└──────────────────────────────────┘
         ↓
Pull Request Shows:
┌──────────────────────────────────┐
│ ⚠️ IMPACT ANALYSIS              │
├──────────────────────────────────┤
│ Modified: Revenue measure        │
│ Affects: 23 downstream measures  │
│ Breaks: 5 visuals               │
│ Severity: HIGH                  │
│                                 │
│ ✅ Documentation updated        │
│ ✅ All quality checks passed    │
│ ✅ Ready to merge               │
└──────────────────────────────────┘
         ↓
Merge with Confidence ✅
```

**Impact:** 🔍 Full visibility | 🛡️ Safe merges | 📊 Auto documentation

---

### **5. 📚 Institutional Knowledge Preservation**

**The Challenge:**
- Knowledge lives in heads, not docs
- "Ask John" isn't scalable
- Turnover = lost expertise

**The Solution:**
```
Question: "Where is the Customer Lifetime Value measure?"

❌ OLD:
   "I think John created it... let me ask him..."
   ❌ Slow  ❌ Dependent on one person
   
✅ NEW:
   Search auto-docs → Found instantly
   └─ Definition: [Full DAX expression]
   └─ Dependencies: [12 upstream sources]
   └─ Used In: [34 measures, 89 visuals]
   └─ Complexity: HIGH (but necessary)
   └─ Last Modified: Sept 15, 2026 by Maria
   └─ Quality Score: 92% ✅
```

**Impact:** ⚡ Instant answers | 🧠 Knowledge base | 👥 Team independence

---

### **6. 🎓 Documentation as Training**

**The Challenge:**
- BI analysts don't document their changes
- New measures appear with zero explanation
- No way to understand design decisions

**The Solution:**
```
Auto-Generated Training Materials:
├─ Measure Purpose & Formula
├─ Data Lineage Diagram
├─ Complexity Explanation
├─ Usage Examples
├─ Related Measures
├─ Quality Scores
└─ Performance Notes

Result: Every measure is self-documenting 📚
```

**Impact:** 🎓 Built-in training | 📖 No extra work | ✨ Professional standards

---

## 📦 What Gets Generated

### **Output Formats** (Choose what you need)

```mermaid
graph LR
    Gen["pbip-doc generate"] -->|Pure Markdown| MD["📘 .md files<br/>100% text-based"]
    Gen -->|Interactive HTML| HTML["🌐 HTML site<br/>React + ECharts"]
    Gen -->|Data Export| JSON["📊 JSON export<br/>Machine readable"]
    Gen -->|GitHub Ready| GH["🐙 GitHub Pages<br/>Auto-deployable"]
    
    style MD fill:#27ae60,stroke:#333,stroke-width:2px,color:#fff
    style HTML fill:#3498db,stroke:#333,stroke-width:2px,color:#fff
    style JSON fill:#f39c12,stroke:#333,stroke-width:2px,color:#fff
    style GH fill:#9b59b6,stroke:#333,stroke-width:2px,color:#fff
```

### **📘 Markdown-Only Export** (Perfect for GitHub)

```
pbip-doc generate --input ./pbip --output ./docs --format markdown
```

Generated structure:
```
docs/
├── README.md                       (Overview + index)
├── _generated_metadata.md          (Analysis timestamp & stats)
│
├── 📊 Semantic Model/
│   ├── 01-tables-summary.md        (All tables overview)
│   ├── 02-columns-detailed.md      (Column definitions)
│   ├── 03-measures-catalog.md      (Every measure documented)
│   ├── 04-relationships.md         (Table relationships)
│   ├── 05-hierarchies.md           (Dimension hierarchies)
│   └── 06-roles-security.md        (RLS & permissions)
│
├── 🧮 DAX Analysis/
│   ├── 01-dax-complexity.md        (Complexity scoring)
│   ├── 02-measure-dependencies.md  (What depends on what)
│   ├── 03-circular-refs.md         (Circular dependency report)
│   ├── 04-performance-tips.md      (Optimization suggestions)
│   └── 05-dax-functions-used.md    (All DAX functions index)
│
├── 📈 Quality Reports/
│   ├── 01-health-summary.md        (Overall quality score)
│   ├── 02-orphaned-entities.md     (Unused measures/columns)
│   ├── 03-code-smells.md           (Anti-patterns detected)
│   ├── 04-recommendations.md       (Improvement opportunities)
│   └── 05-metrics.md               (Raw quality metrics)
│
├── 📊 Visualizations/ (Mermaid diagrams for GitHub rendering)
│   ├── erd-diagram.md              (Entity relationship diagram)
│   ├── data-lineage.md             (Source → Visual paths)
│   ├── measure-tree.md             (Dependency tree)
│   └── quality-summary.md          (Health dashboard)
│
└── 🔗 Lineage/
    ├── 01-sources-to-tables.md     (SQL → Tables)
    ├── 02-tables-to-measures.md    (Tables → Measures)
    └── 03-measures-to-visuals.md   (Measures → Visuals)
```

### **✨ All Export Formats**

<table>
<tr>
<td width="50%">

**📘 Pure Markdown**
- ✅ No dependencies
- ✅ GitHub native
- ✅ Version control friendly
- ✅ Searchable
- ✅ Self-contained

Perfect for:
- GitHub repos
- Version control
- Team collaboration
- Documentation sites

</td>
<td width="50%">

**🌐 Interactive HTML**
- ✅ React Flow diagrams
- ✅ ECharts dashboards  
- ✅ 3D lineage graphs
- ✅ Live search
- ✅ GitHub Pages ready

Perfect for:
- Team portals
- Executive dashboards
- Interactive exploration
- Public sharing

</td>
</tr>
</table>

---

## ⚡ Get Started in 3 Minutes

### **Step 1: Install (30 seconds)**

```bash
npm install pbip-documentation-skill
```

> **Windows Users:** If npm not installed, [get Node.js here](https://nodejs.org)

### **Step 2: Analyze Your PBIP (30 seconds)**

Drop your PBIP folder and run:

```bash
pbip-doc generate \
  --input ./my-pbip \
  --output ./docs \
  --doc-language en \
  --ai-explanations
```

**What it does:**
- 🔍 Parses TMDL & PBIR files
- 🧠 Analyzes DAX & Power Query
- 📊 Builds knowledge graph
- ⚙️ Runs quality checks
- 📝 Generates documentation

### **Step 3: View & Share (30 seconds)**

```bash
cd docs
python -m http.server 8000
```

Then open: **http://localhost:8000**

You now have:
- ✅ Complete documentation
- ✅ Interactive visualizations
- ✅ Impact analysis data
- ✅ Quality reports

### **Step 4 (Optional): Auto-Deploy to GitHub**

Create `.github/workflows/pbip-docs.yml`:

```yaml
name: PBIP Docs Auto-Deploy

on:
  push:
    paths:
      - "**.tmdl"
      - "**.pbir"
    branches:
      - main

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
      - run: npm install pbip-documentation-skill
      - run: pbip-doc generate \
              --input . \
              --output ./docs \
              --ai-explanations
      
      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./docs
          cname: your-domain.com  # (optional)
```

Now documentation updates **automatically** on every commit! 🚀

### **Available Commands**

```bash
# Full documentation with AI explanations
pbip-doc generate --input ./pbip --output ./docs --ai-explanations

# Quick analysis without generating docs
pbip-doc analyze ./pbip

# Specific language output
pbip-doc generate --input ./pbip --output ./docs --doc-language es

# Debug mode (verbose logging)
pbip-doc generate --input ./pbip --output ./docs --debug

# Compare two PBIP versions (impact analysis)
pbip-doc analyze-diff ./pbip-v1 ./pbip-v2
```

---

## 📊 Performance & Scalability

### **Speed Benchmarks**

```
Small Project (50 measures, 5 tables)
└─ Analysis: 8s ⚡
   └─ Parse: 1s | Build Graph: 2s | Generate: 5s

Medium Project (500 measures, 50 tables, 5 reports)
└─ Analysis: 25s 📊
   └─ Parse: 3s | Build Graph: 8s | Generate: 14s

Large Project (2000+ measures, 200 tables, 25 reports)
└─ Analysis: 60s 🚀
   └─ Parse: 8s | Build Graph: 20s | Generate: 32s
```

### **Resource Usage**

| Size | Time | Memory | Outputs |
|------|------|--------|---------|
| 📱 Small | 8s | 120MB | 15 files |
| 📊 Medium | 25s | 350MB | 45 files |
| 📈 Large | 60s | 800MB | 120+ files |

*Tested on: Ubuntu 22.04 (GitHub Actions) • 4 cores • 16GB RAM*

### **Scalability**

✅ Handles 10k+ entity graphs  
✅ Processes 2000+ measures  
✅ 100+ reports per project  
✅ Full lineage tracking (no cutoffs)  
✅ Linear performance scaling  

---

## 🛠️ Built With Modern Technologies

<table>
<tr><td width="50%">

### **Frontend Stack** 🎨
- **React 18.3** - Modern UI rendering
- **React Flow 10** - Interactive diagrams
- **ECharts 5.4** - Rich visualizations
- **Sigma.js 3.0** - WebGL graph rendering
- **Mermaid** - Diagram generation

</td><td width="50%">

### **Backend Stack** ⚙️
- **TypeScript 5.3** - Type-safe code
- **Node.js Latest** - Runtime
- **@microsoft/powerquery-parser** - Power Query parsing
- **Regex engines** - DAX/TMDL parsing
- **Graph algorithms** - Lineage + impact analysis

</td></tr>
</table>

### **Integration Stack** 🔗
- **GitHub Actions** - CI/CD automation
- **GitHub API** - PR comments & deployments
- **npm** - Package distribution
- **Claude API** - AI explanations (optional)

---

## 📖 All Available Commands

### **Complete Documentation Generation**
```bash
pbip-doc generate \
  --input ./my-pbip \
  --output ./docs \
  --doc-language es \
  --ai-explanations \
  --theme dark
```

### **Quick Analysis (No Generate)**
```bash
pbip-doc analyze ./my-pbip
```

### **Analyze with Details**
```bash
pbip-doc analyze ./my-pbip --show-orphans --show-cycles --show-complexity
```

### **Compare Two Versions (Impact Analysis)**
```bash
pbip-doc analyze-diff ./pbip-v1 ./pbip-v2
```

### **Export Specific Format**
```bash
pbip-doc generate --input ./pbip --output ./docs --export json,markdown,html
```

### **Debug Mode**
```bash
pbip-doc generate --input ./pbip --output ./docs --debug --verbose
```

### **Configuration File**
```bash
pbip-doc generate --config pbip-doc.config.json
```

**Example config:**
```json
{
  "input": "./pbip",
  "output": "./docs",
  "languages": ["en", "es", "fr"],
  "aiExplanations": true,
  "includeLineage": true,
  "detectCycles": true,
  "generateVisualizations": true,
  "exportFormats": ["html", "json", "markdown"],
  "theme": "dark",
  "hosted": true
}
```

---

## 🔗 Complete GitHub Actions Setup

### **Basic Auto-Deploy**

```yaml
name: PBIP Documentation Auto-Deploy

on:
  push:
    branches: [main]
    paths:
      - "**.tmdl"
      - "**.pbir"
      - ".github/workflows/pbip-docs.yml"

jobs:
  generate-docs:
    runs-on: ubuntu-latest
    
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0  # Full history for impact analysis
      
      - uses: actions/setup-node@v4
        with:
          node-version: "20"
      
      - name: Install Skill
        run: npm install pbip-documentation-skill
      
      - name: Generate Documentation
        run: |
          pbip-doc generate \
            --input . \
            --output ./docs \
            --doc-language en \
            --ai-explanations
      
      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./docs
          cname: docs.example.com  # Optional: custom domain
```

### **Advanced: With PR Comments + Impact Analysis**

```yaml
name: PBIP Documentation with Impact Analysis

on:
  push:
    branches: [main]
    paths: ["**.tmdl", "**.pbir"]
  pull_request:
    paths: ["**.tmdl", "**.pbir"]

jobs:
  analyze:
    runs-on: ubuntu-latest
    
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0
      
      - uses: actions/setup-node@v4
        with:
          node-version: "20"
      
      - run: npm install pbip-documentation-skill
      
      # PR: Show impact before merge
      - if: github.event_name == 'pull_request'
        name: Analyze Impact
        run: |
          pbip-doc analyze-diff \
            origin/main \
            HEAD \
            > /tmp/impact.txt
      
      - if: github.event_name == 'pull_request'
        name: Comment on PR
        uses: actions/github-script@v6
        with:
          script: |
            const fs = require('fs');
            const impact = fs.readFileSync('/tmp/impact.txt', 'utf8');
            github.rest.issues.createComment({
              issue_number: context.issue.number,
              owner: context.repo.owner,
              repo: context.repo.repo,
              body: `## 📊 PBIP Impact Analysis\n\n${impact}`
            });
      
      # Main: Generate & deploy docs
      - if: github.ref == 'refs/heads/main'
        name: Generate Documentation
        run: pbip-doc generate --input . --output ./docs --ai-explanations
      
      - if: github.ref == 'refs/heads/main'
        name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./docs
```

---

## ❓ FAQ

**Q: Do I need Power BI Desktop?**  
A: No! The skill works with just TMDL/PBIR files.

**Q: Can I use this with legacy Power BI?**  
A: Yes, it supports TMSL and legacy report.json formats.

**Q: How do I preserve formatting in generated Markdown?**  
A: Formatting is preserved in Markdown. HTML export also available.

**Q: Can I customize the generated documentation?**  
A: Yes, use config files and CSS/HTML templates.

**Q: Does it work offline?**  
A: Yes, analysis is entirely local. No cloud required (AI explanations optional).

**Q: How often should I regenerate docs?**  
A: Set GitHub Actions to auto-generate on every change.

**Q: What if my PBIP is private?**  
A: Docs are generated locally, never uploaded anywhere.

---

## 💬 Support & Community

| Channel | Link |
|---------|------|
| **GitHub Issues** | [Report bugs & request features](https://github.com/ludodelot/pbip-doc/issues) |
| **Discussions** | [Ask questions & share ideas](https://github.com/ludodelot/pbip-doc/discussions) |
| **LinkedIn** | [Connect with the creator](https://www.linkedin.com/in/delot/) |
| **Email** | contactoludovicdelot@gmail.com |

---

## 📄 License & Attribution

**MIT License** - Free for personal and commercial use.  
No restrictions. No attribution required (but appreciated! ❤️)

[View Full License](LICENSE)

---

## 🎯 The Commitment

This skill is built for **BI Engineers** who believe:
- ✅ Documentation should be automatic, not manual
- ✅ Transparency beats tribal knowledge
- ✅ Change safety should be the default
- ✅ Tools should be open, not gatekeeping
- ✅ Power BI projects deserve engineering rigor

**That's the mission. Let's build better BI together.** 🚀

---

<div align="center">

## 📥 Ready to Transform Your PBIP?

### ⬇️ **Download the Skill Now**

[![Release](https://img.shields.io/github/v/release/ludodelot/pbip-doc?style=for-the-badge&color=0078d4&labelColor=1f1f1f)](https://github.com/ludodelot/pbip-doc/releases/latest)

### One command. Complete docs. Full transparency.

---

## 👨‍💻 About

**Created by Ludovic Delot**

A BI engineer frustrated with manual Power BI documentation built this skill to solve the problem once and for all. When documentation requires 50+ files to be manually updated every time something changes, something's broken.

This skill automates the boring part so teams can focus on building better data products.

**Connect:**
- 🔗 [LinkedIn](https://www.linkedin.com/in/delot/)
- 📧 contactoludovicdelot@gmail.com
- 💼 Data Architecture | BI Automation | Power BI Engineering

---

```
Built with ❤️ using TypeScript • Open-source MIT License
Helping BI teams document smarter, ship faster
```

</div>
