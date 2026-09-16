<div align="center">

# 📊 PBIP Documentation Skill

> **Transform Power BI Projects into Interactive, AI-Powered Documentation**

[![Release](https://img.shields.io/github/v/release/ludodelot/pbip-doc?style=for-the-badge&color=0078d4&labelColor=1f1f1f)](https://github.com/ludodelot/pbip-doc/releases)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge&labelColor=1f1f1f)](LICENSE)
[![Downloads](https://img.shields.io/npm/dm/pbip-documentation-skill?style=for-the-badge&labelColor=1f1f1f)](https://www.npmjs.com/package/pbip-documentation-skill)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black&labelColor=1f1f1f)](https://powerbi.microsoft.com)

### 🚀 The Missing Link Between Power BI & Software Engineering

**Automatic documentation. Impact analysis. Full lineage tracking. No Power BI Desktop required.**

[📥 Download Now](#-quick-start) • [📖 See Features](#-what-it-does) • [🎯 Use Cases](#-use-cases) • [💬 Support](#-support)

</div>

---

## 🎯 What It Does

<table>
<tr>
<td width="50%">

### 📈 **Transform Your PBIP**

```
Your PBIP Files
    ↓
Automatic Analysis
    ↓
Interactive Docs
    ↓
Deployed to GitHub Pages
```

</td>
<td width="50%">

### ⚡ **Key Benefits**

✅ **Full Lineage** - SQL → Measures → Visuals  
✅ **Impact Analysis** - See what breaks before you change it  
✅ **Quality Reports** - Orphans, cycles, complexity  
✅ **7 Languages** - Measure names preserved  
✅ **GitHub Ready** - Auto PR comments + Pages deploy  
✅ **No Desktop Needed** - Pure file-based  

</td>
</tr>
</table>

---

## 🔄 How It Works

### **The Magic Pipeline**

```
┌─────────────────────────────────────────────────────────────┐
│  Your PBIP Project                                          │
│  ├── definition.pbism          (semantic model config)      │
│  ├── definition/model.tmdl     (tables, columns)            │
│  ├── definition/tables/*.tmdl  (measures, hierarchies)      │
│  └── definition.pbir           (report layer)               │
└─────────────────────────────────────────────────────────────┘
                         ⬇️  PARSING
┌─────────────────────────────────────────────────────────────┐
│  PBIP Documentation Skill                                   │
│  🔍 TMDL Lexer       → Tables, columns, measures           │
│  🔍 PBIR Parser      → Pages, visuals, projections         │
│  🔍 DAX Analyzer     → Dependencies, complexity            │
│  🔍 Power Query      → M expressions, lineage              │
└─────────────────────────────────────────────────────────────┘
                         ⬇️  BUILD GRAPH
┌─────────────────────────────────────────────────────────────┐
│  Knowledge Graph                                            │
│  📊 11 Entity Types (Table, Measure, Visual, etc.)         │
│  🔗 Full Lineage     (SQL → Measures → Visuals)            │
│  ✅ Quality Checks   (Orphans, cycles, complexity)         │
└─────────────────────────────────────────────────────────────┘
                         ⬇️  GENERATE
┌─────────────────────────────────────────────────────────────┐
│  Interactive Documentation                                  │
│  📘 Markdown Docs    (Tables, measures, relationships)     │
│  📊 React Flow       (ERD, DAX trees)                      │
│  📈 ECharts          (Health dashboards)                    │
│  🌐 GitHub Pages     (Deployed automatically)               │
└─────────────────────────────────────────────────────────────┘
```

---

## 💡 Real-World Example

### **Before: Manual & Opaque**

```
Q: "What measures depend on the Customer table?"
A: *looks through 50+ files* "Uh, I think Revenue and Customer 
   Acquisition, but let me check with the person who built it..."

Result: ⏱️ 30 minutes wasted, tribal knowledge risk
```

### **After: Automatic & Transparent**

```bash
$ pbip-doc analyze ./my-pbip
```

**Instant Output:**
```
✅ Tables: 12
✅ Measures: 145
✅ Visuals: 234
✅ Customer Table Dependencies: 12 measures, 45 visuals
✅ Quality: No orphans, no cycles, avg complexity: MEDIUM
```

**Generated Docs:**
- Interactive ERD showing all relationships
- Each measure documented with DAX complexity score
- Full impact analysis (what breaks if you change Customer)
- GitHub Pages site deployed automatically

Result: ⚡ 2 minutes, full transparency, 100% coverage

---

## ✨ Key Features

<table>
<tr>
<td>

### 🔍 **Deep Analysis**
- TMDL parsing (tables, columns, measures)
- PBIR parsing (pages, visuals, projections)
- DAX complexity scoring
- Power Query lineage
- Automatic quality linting

</td>
<td>

### 📊 **Rich Visualizations**
- Entity Relationship Diagrams (ERD)
- DAX Dependency Trees
- Data Lineage Graphs (10k+ nodes)
- Model Health Dashboards
- Interactive Markdown Reports

</td>
</tr>
<tr>
<td>

### 🚀 **GitHub Integration**
- Auto PR comments on changes
- Impact analysis on merge
- Automatic Pages deployment
- Quality reports in CI/CD
- Semantic diff tracking

</td>
<td>

### 🌍 **Global Ready**
- 7 languages (en, es, fr, de, ja, zh, pt)
- Measure names preserved
- Customizable output
- Configuration file support
- No Power BI Desktop needed

</td>
</tr>
</table>

---

## 📈 Use Cases

### **1. 📋 Data Governance**
Document your entire Power BI ecosystem for compliance audits.

```
PBIP Project → Auto Docs → Audit Trail ✅
```

---

### **2. 🔗 Impact Analysis**
Before changing a measure, know exactly what breaks.

```
Change Total Revenue → 
  ↳ Affects 12 downstream measures
  ↳ Breaks 7 visuals
  ↳ Impacts 2 reports
  ↳ Severity: HIGH ⚠️
```

---

### **3. 🚀 Team Onboarding**
New engineers read auto-generated docs instead of asking questions.

```
New BI Engineer → Reads Auto Docs → Productive in 1 day ✅
```

---

### **4. 🔄 CI/CD Integration**
Automatic PR comments show impact before merge.

```
Developer ↓ Push to GitHub
    ↓ GitHub Action triggered
    ↓ Analysis complete in 30 seconds
    ↓ PR comment: "⚠️ Impact: 7 visuals, HIGH severity"
    ↓ Developer reviews before merging
```

---

### **5. 📚 Institutional Knowledge**
Stop relying on tribal knowledge. Everything documented.

```
Question: "Where is the revenue measure?"
Answer: Auto-docs (always up to date) ✅

Benefit: No more "ask John, he built it"
```

---

## 🎯 What Gets Generated

<table>
<tr><th>Output</th><th>Format</th><th>Example</th></tr>
<tr><td>Semantic Model Docs</td><td>Markdown</td><td>Table schemas, column definitions</td></tr>
<tr><td>Measure Catalog</td><td>Markdown + DAX</td><td>Every measure with complexity score</td></tr>
<tr><td>Entity Diagram</td><td>Mermaid ERD</td><td>Visual of all tables & relationships</td></tr>
<tr><td>DAX Trees</td><td>React Flow</td><td>Interactive measure dependencies</td></tr>
<tr><td>Lineage Map</td><td>WebGL Graph</td><td>SQL source → Visual (10k+ nodes)</td></tr>
<tr><td>Quality Report</td><td>JSON</td><td>Orphans, cycles, complexity metrics</td></tr>
<tr><td>Health Dashboard</td><td>ECharts</td><td>Model stats & metrics</td></tr>
<tr><td>GitHub Pages</td><td>Static Site</td><td>Interactive documentation hosted</td></tr>
</table>

---

## ⚡ Quick Start

### **1️⃣ Install**
```bash
npm install pbip-documentation-skill
```

### **2️⃣ Generate Docs**
```bash
pbip-doc generate --input ./my-pbip --output ./docs
```

### **3️⃣ View Results**
```bash
cd docs
python -m http.server 8000
# Visit http://localhost:8000
```

### **4️⃣ Deploy to GitHub Pages** (Optional)
```bash
# Setup in .github/workflows/pbip-docs.yml
# Auto-deploys on every push
```

---

## 📊 Performance

| Project Size | Analysis Time | Memory |
|---|---|---|
| **Small** (50 measures) | 8s | 120MB |
| **Medium** (500 measures, 5 reports) | 25s | 350MB |
| **Large** (2000+ measures, 25 reports) | 60s | 800MB |

*Benchmarks on GitHub Actions (Ubuntu 22.04, 4 cores, 16GB)*

---

## 🎨 Supported Formats

| Format | Status | Details |
|--------|--------|---------|
| **TMDL** | ✅ Full Support | Modern semantic model format |
| **PBIR** | ✅ Full Support | Modern report format |
| **Power Query (M)** | ✅ Via @microsoft/powerquery-parser | Expression lineage |
| **DAX** | ✅ Custom Parser | Complexity analysis |
| **Legacy PBIR** | ✅ Fallback | report.json format |
| **TMSL** | ✅ Fallback | v1.0 compatibility |

---

## 📖 Commands

### **Generate Full Documentation**
```bash
pbip-doc generate \
  --input ./my-pbip \
  --output ./docs \
  --doc-language es \
  --ai-explanations
```

### **Quick Project Analysis**
```bash
pbip-doc analyze ./my-pbip
```

### **With Debug Logging**
```bash
pbip-doc generate --input . --output ./docs --debug
```

---

## 🔗 GitHub Actions Integration

Auto-deploy documentation on every push:

```yaml
name: PBIP Documentation

on:
  push:
    branches: [main]
    paths: ['**.tmdl', '**.pbir']

jobs:
  docs:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
      - run: npm install pbip-documentation-skill
      - run: pbip-doc generate --input . --output ./docs
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./docs
```

---

## 💬 Support

| Channel | Link |
|---------|------|
| **Issues** | [Report a bug](https://github.com/ludodelot/pbip-doc/issues) |
| **Discussions** | [Ask questions](https://github.com/ludodelot/pbip-doc/discussions) |
| **Email** | ludovicdelot99@gmail.com |

---

## 📄 License

**MIT License** - Free for personal and commercial use.

[View Full License](LICENSE)

---

<div align="center">

## 🚀 Get Started Now

[![Download Skill](https://img.shields.io/badge/📥%20Download%20v20260916-blue?style=for-the-badge&labelColor=1f1f1f)](https://github.com/ludodelot/pbip-doc/releases/latest)

### Made for BI Engineers Who Want Their Power BI Projects to be as Maintainable as Software

**Automatic documentation. Full transparency. No more guessing.**

</div>
