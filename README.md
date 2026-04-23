# DataSense — Instant Data Intelligence

> Drop a CSV or Excel file. Instantly get stats, charts, correlations, outliers, and a baseline ML model — no code, no cloud, no install.

[![Live Demo](https://img.shields.io/badge/Live_Demo-Try_it_now-6366f1?style=for-the-badge)](https://bhaskar21-7.github.io/datasense)
[![No Install](https://img.shields.io/badge/No_Install-Open_in_Browser-22d3ee?style=for-the-badge)](https://bhaskar21-7.github.io/datasense)
[![Privacy](https://img.shields.io/badge/Privacy-Data_never_leaves_your_machine-10b981?style=for-the-badge)](#)
[![Version](https://img.shields.io/badge/Version-3.0-6366f1?style=for-the-badge)](#)

---

## ✦ Preview

<table>
  <tr>
    <td><img src="screenshots/01_landing.png" alt="Landing page with CSV upload" width="100%"/></td>
    <td><img src="screenshots/02_dataset_overview.png" alt="Dataset overview and data preview" width="100%"/></td>
  </tr>
  <tr>
    <td align="center"><sub>Drop any CSV/Excel — 4 sample datasets included</sub></td>
    <td align="center"><sub>Instant dataset overview + scrollable data preview</sub></td>
  </tr>
  <tr>
    <td><img src="screenshots/04_visualizations.png" alt="Auto-generated charts and histograms" width="100%"/></td>
    <td><img src="screenshots/05_correlation_matrix.png" alt="Color-coded Pearson correlation matrix" width="100%"/></td>
  </tr>
  <tr>
    <td align="center"><sub>Auto-generated histograms, scatter plots &amp; frequency charts</sub></td>
    <td align="center"><sub>Color-coded Pearson correlation matrix</sub></td>
  </tr>
  <tr>
    <td><img src="screenshots/07_baseline_model.png" alt="Baseline ML model results" width="100%"/></td>
    <td><img src="screenshots/06_statistical_insights.png" alt="Rule-based statistical insights" width="100%"/></td>
  </tr>
  <tr>
    <td align="center"><sub>One-click baseline model — kNN or Linear Regression</sub></td>
    <td align="center"><sub>Rule-based statistical insights, 100% offline</sub></td>
  </tr>
</table>

---

## What it does

Drop any CSV or Excel file and DataSense runs a full exploratory data analysis entirely in your browser — no server, no API key, no data upload.

**→ [Try the live demo](https://bhaskar21-7.github.io/datasense)**

---

## Features

**EDA (core strength)**
- Dataset overview — shape, types, missing value count
- Column-level stats — mean, std, min/max, median, IQR
- Correlation matrix — row-aligned Pearson r, color-coded heatmap
- Outlier detection — IQR method, flagged per column
- Custom interactive charts — build scatter, pie, line, or bar charts on the fly
- Distributions — auto-binned histograms (√n rule), scatter plots, frequency charts
- Live data preview — fast search filtering with sortable columns
- Key finding — auto-surfaces the single most important pattern in your data

**Statistical Insights** *(rule-based, 100% offline)*
- Missing value analysis with imputation recommendations
- Multicollinearity detection (|r| ≥ 0.90 pairs)
- Variance driver — identifies the column dominating data spread
- Skewness flags with transformation suggestions (log, √)
- High-cardinality column detection
- Binary column classification target suggestions
- Full preprocessing pipeline recommendation

**Baseline Model** *(quick benchmarking)*
- Auto-detects classification vs regression from target column
- Classification → k-Nearest Neighbors (k=5)
- Regression → Linear Regression (gradient descent, 200 epochs)
- StandardScaler fit on training set only — no data leakage
- Deterministic train/test split — same result every run
- Feature correlation with target (with honest disclaimer)
- Categorical columns excluded explicitly with note

**Export & Compatibility**
- **Excel support** — drag and drop `.xlsx` / `.xls` files (parsed locally via SheetJS)
- Export full analysis as a `.txt` report
- Download styled `.pdf` reports of the entire dashboard

---

## Tech stack

```
CSV/Excel parsing  →  PapaParse + SheetJS
Charts             →  Chart.js
ML                 →  Vanilla JS (implemented from scratch)
Stats              →  Rule-based engine (no external dependencies)
Typography         →  Inter + JetBrains Mono (Google Fonts)
Deploy             →  GitHub Pages
```

Zero backend. Zero dependencies to install. Everything runs client-side.

---

## Try it in 10 seconds

1. Open the [live demo](https://bhaskar21-7.github.io/datasense)
2. Sales data loads automatically — full analysis is instant
3. Or drop your own CSV/Excel, or click a sample chip

**Built-in samples:** 🌸 Iris · 📊 Sales · 🎓 Students · 🚢 Titanic

---

## Run locally

```bash
git clone https://github.com/bhaskar21-7/datasense
cd datasense
# open index.html in any browser
```

No build step. No `npm install`. One HTML file.

---

## What it's not

- Not an AI tool — insights are statistical and rule-based
- Not a production ML system — the model section is a quick baseline, not a deployment pipeline
- Not a data storage service — your files never leave your browser

---

## Roadmap

- [ ] Additional baseline models (Naive Bayes, Decision Tree)
- [ ] Natural language column querying

---

## Built by

**Bhaskar Jha** — Statistics undergraduate, MS 2027

[![GitHub](https://img.shields.io/badge/GitHub-bhaskar21--7-181717?style=flat&logo=github)](https://github.com/bhaskar21-7)

---

*If this saved you time, a ⭐ helps others find it.*
