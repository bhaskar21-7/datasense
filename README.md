# DataSense — Offline Data Intelligence Engine

> Analyze any dataset directly in your browser. No backend. No uploads. No dependencies.

DataSense is a **fully client-side data analysis system** that performs exploratory data analysis (EDA), statistical diagnostics, and baseline machine learning — instantly.

---

## 🔗 Live Demo

👉 https://bhaskar21-7.github.io/datasense

---

## 🚀 What This Actually Does

Drop a CSV or Excel file and DataSense will:

* Profile your dataset (types, missing values, distributions)
* Generate statistical summaries (mean, std, IQR, skew hints)
* Detect outliers using IQR method
* Compute correlation matrix (Pearson r)
* Generate interactive charts (histogram, scatter, bar, pie)
* Provide rule-based insights and data quality signals
* Train a baseline ML model (classification or regression)
* Export results as text or PDF

Everything runs **100% locally in your browser**.

---

## 🧠 Why This Exists

Most tools either:

* require coding (pandas, R), or
* require uploading sensitive data (cloud dashboards)

DataSense removes both constraints.

It is designed for:

* quick dataset understanding
* early-stage analysis
* learning and experimentation
* privacy-sensitive workflows

---

## ⚙️ Core Features

### 📊 Exploratory Data Analysis

* Column-level statistics (mean, std, median, min/max)
* Missing value analysis with percentages
* Unique counts and data type detection
* Distribution estimation via histogram binning

---

### 🔗 Correlation Analysis

* Full Pearson correlation matrix
* Color-coded strength visualization
* Detection of highly correlated feature pairs

---

### ⚠️ Outlier Detection

* IQR-based detection (Q1, Q3, 1.5×IQR rule)
* Outlier counts per column
* Range diagnostics for anomaly inspection

---

### 📈 Visualization Engine

* Auto-generated:

  * Histograms (numeric columns)
  * Frequency charts (categorical columns)
  * Scatter plots (feature relationships)
* Custom chart builder:

  * Bar / Line / Scatter / Pie
  * Aggregation support (mean grouping)

---

### 🤖 Baseline Machine Learning

* Automatic task detection:

  * Classification → k-NN
  * Regression → Linear Regression
* Train/test split (deterministic)
* Feature normalization (no leakage)
* Performance metrics:

  * Accuracy (classification)
  * R² and RMSE (regression)

> ⚠️ This is a baseline model for quick evaluation — not production-grade ML.

---

### 💡 Insight Engine (Rule-Based)

* Missing data warnings
* Skewness detection and transformation hints
* High-cardinality column detection
* Multicollinearity signals (via correlation)
* Variance-dominant feature identification

---

### 📄 Export

* Download analysis as `.txt`
* Export full dashboard as `.pdf`

---

## 🔒 Privacy by Design

* No API calls
* No data uploads
* No tracking

Your data **never leaves your device**.

---

## 🧱 Tech Stack

* Parsing → PapaParse, SheetJS
* Visualization → Chart.js
* ML → Vanilla JavaScript (custom implementation)
* UI → HTML, CSS (no frameworks)
* Deployment → GitHub Pages

---

## ⚡ Performance Notes

* Optimized for small to medium datasets (~10K–100K rows depending on width)
* Entire dataset is processed in-memory
* No streaming or chunking (yet)

---

## ❗ Limitations (Honest)

* Not a replacement for pandas, R, or production ML pipelines
* No advanced statistical inference (yet)
* No categorical encoding in ML pipeline
* No hyperparameter tuning
* Insight engine is rule-based (not true AI)

---

## 🛣️ Roadmap

Planned improvements:

* [ ] Hypothesis testing (t-test, chi-square, ANOVA)
* [ ] Feature importance and explainability
* [ ] Additional models (decision tree, naive bayes)
* [ ] Data preprocessing pipeline generation
* [ ] Smarter query engine (beyond keyword matching)
* [ ] Time-series detection

---

## 🧪 Use Cases

* Quick dataset sanity check before modeling
* Exploratory analysis without coding
* Teaching statistics concepts interactively
* Privacy-safe data inspection
* Rapid prototyping before moving to Python/R

---

## 🧑‍💻 Local Setup

```bash
git clone https://github.com/bhaskar21-7/datasense
cd datasense
open index.html
```

No install. No build. No dependencies.

---

## 👤 Author

Bhaskar Jha
Statistics Undergraduate (MS 2027)

GitHub: https://github.com/bhaskar21-7

---

## ⭐ If This Helps

Star the repo. It helps others discover it.

---

## Final Note

This project is intentionally built with **zero backend and zero dependencies** to demonstrate how far client-side data analysis can go.

It is not meant to replace professional tools — but to make data understanding faster, simpler, and private.
