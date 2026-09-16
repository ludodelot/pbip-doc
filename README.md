# 📊 PBIP Documentation Skill

> **The Ultimate AI-Powered Power BI Project Documentation Generator**

[![Downloads](https://img.shields.io/github/downloads/ludodelot/pbip-doc/total?style=flat-square)](https://github.com/ludodelot/pbip-doc/releases)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)
[![Latest Release](https://img.shields.io/github/v/release/ludodelot/pbip-doc?style=flat-square)](https://github.com/ludodelot/pbip-doc/releases/latest)

<div align="center">

### Transform Power BI Projects into Interactive Documentation Automatically

[📥 Download](#-download) • [🚀 Quick Start](#-quick-start) • [📖 Full Docs](#-documentation) • [💬 Support](#-support)

</div>

---

## 🎯 What It Does

Automatically generates professional documentation for Power BI Projects (PBIP):

- 📊 **Full Data Lineage** - SQL sources → Measures → Visuals
- 📈 **Impact Analysis** - See what breaks before you change it
- 🔍 **Semantic Analysis** - Deep parsing of TMDL, PBIR, DAX, Power Query
- 📚 **Auto Documentation** - Markdown + visualizations
- 🌍 **7 Languages** - English, Spanish, French, German, Japanese, Chinese, Portuguese
- 🚀 **GitHub Integration** - Automatic PR comments, Pages deployment
- ✅ **Quality Reports** - Orphan detection, circular dependencies
- 🤖 **AI Explanations** - Claude-powered summaries (optional)

---

## 📥 Download

### Latest Release: **v20260916**

**👇 Click to download the latest .skill file:**

[![Download](https://img.shields.io/badge/Download%20Skill-v20260916-blue?style=for-the-badge&logo=github)](https://github.com/ludodelot/pbip-doc/releases/download/v20260916/pbip-documentation.skill.md)

Or via npm:
```bash
npm install pbip-documentation-skill
```

---

## 🚀 Quick Start

### 1. Install
```bash
npm install pbip-documentation-skill
```

### 2. Generate Documentation
```bash
pbip-doc generate --input ./my-pbip --output ./docs
```

### 3. View Results
```bash
cd docs
python -m http.server 8000
# Visit http://localhost:8000
```

---

## 💡 Common Commands

```bash
# Generate docs in Spanish
pbip-doc generate --input ./my-pbip --output ./docs --doc-language es

# Quick analysis
pbip-doc analyze ./my-pbip

# With AI explanations
pbip-doc generate --input ./my-pbip --output ./docs --ai-explanations

# Debug mode
pbip-doc generate --input ./my-pbip --output ./docs --debug
```

---

## 📚 Documentation

| Resource | Link |
|----------|------|
| **Full Guide** | [pbip-documentation.skill.md](pbip-documentation.skill.md) |
| **Installation** | See above |
| **GitHub Integration** | See .skill file for GitHub Actions setup |
| **Examples** | Included in .skill documentation |
| **Support** | See [Support](#-support) below |

---

## ✨ Features at a Glance

| Feature | Details |
|---------|---------|
| **TMDL Parsing** | Tables, columns, measures, relationships |
| **PBIR Parsing** | Pages, visuals, projections |
| **DAX Analysis** | Complexity scoring, dependency tracking, patterns |
| **Power Query** | M expression lineage via @microsoft/powerquery-parser |
| **Knowledge Graph** | Full lineage with orphan & cycle detection |
| **Visualizations** | Interactive React Flow, ECharts, Sigma.js |
| **GitHub Actions** | Auto-analysis, PR comments, Pages deployment |
| **Quality Linting** | Orphan measures, circular dependencies, complexity |
| **Multi-language** | 7 languages with preserved measure names |
| **AI Mode** | Claude API integration (optional) |

---

## 🎯 Use Cases

### 📋 Data Governance
Document your entire Power BI ecosystem for compliance and audit trails.

### 🔗 Impact Analysis
Before changing a measure, know exactly which reports and visuals are affected.

### 🚀 Team Onboarding
New engineers can read auto-generated docs instead of asking questions.

### 🔄 CI/CD Integration
Automatic PR comments show impact of PBIP changes before merge.

### 📚 Institutional Knowledge
Stop relying on tribal knowledge. Everything is documented.

---

## 🌍 Supported Formats

- ✅ **TMDL** - Semantic model (modern format)
- ✅ **PBIR** - Report layer (modern format)
- ✅ **Power Query (M)** - Data transformations
- ✅ **DAX** - All expressions supported
- ✅ **Legacy PBIR** - report.json format
- ✅ **TMSL** - v1.0 compatibility

---

## 📊 Performance

| Project Size | Time | Memory |
|--------------|------|--------|
| Small (50 measures) | 8s | 120MB |
| Medium (500 measures) | 25s | 350MB |
| Large (2000+ measures) | 60s | 800MB |

*Benchmarks on GitHub Actions (Ubuntu 22.04, 4 cores, 16GB)*

---

## 💬 Support

### Having Issues?
- **GitHub Issues**: [Report a bug](https://github.com/ludodelot/pbip-doc/issues)
- **Discussions**: [Ask questions](https://github.com/ludodelot/pbip-doc/discussions)
- **Email**: ludovicdelot99@gmail.com

### Want to Contribute?
See documentation in the .skill file for contribution guidelines.

---

## 📄 License

MIT License - Free for personal and commercial use.

See [LICENSE](LICENSE) for details.

---

## 🙌 Credits

Built for BI engineers who want their Power BI Projects to be as maintainable as software.

**Created by Ludovic Delot** | [GitHub](https://github.com/ludodelot)

---

<div align="center">

### Get Started Now

[![Download Skill](https://img.shields.io/badge/Download-Latest%20Skill-blue?style=for-the-badge)](https://github.com/ludodelot/pbip-doc/releases/latest)

**Questions?** [Check the documentation](pbip-documentation.skill.md) or [open an issue](https://github.com/ludodelot/pbip-doc/issues)

</div>
