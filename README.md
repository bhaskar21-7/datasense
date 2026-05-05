# DataSense — Offline Data Intelligence System

> From raw data to decisions — fully in your browser. No backend. No uploads.

DataSense is a **client-side data analysis engine** that combines EDA, statistical testing, and baseline machine learning with a guided decision layer.

---

## 🔗 Live Demo

👉 https://bhaskar21-7.github.io/datasense

---

## 🚀 What It Does

Upload a CSV or Excel file and DataSense will:

* Profile your dataset (types, missing values, distributions)
* Generate statistical summaries (mean, std, skewness, IQR)
* Detect outliers using IQR method
* Compute correlation matrix + multicollinearity (VIF)
* Run hypothesis tests (t-test, ANOVA, chi-square)
* Build cross-validated ML models
* Show feature importance
* Recommend cleaning steps and next actions
* Export analysis as PDF, text, or Python code

Everything runs **100% locally in your browser**.

---

## 🧠 Core Idea

Most tools either:

* require coding (pandas, R), or
* require uploading data (cloud tools)

DataSense removes both.

It is designed to:

* understand data quickly
* guide decisions (not just visualize)
* stay fully private

---

## ⚙️ Features

### 📊 Exploratory Data Analysis

* Column profiling (type, missing %, unique)
* Mean, median, std, min/max
* Skewness detection
* Dataset quality scoring

---

### 🔗 Correlation & Multicollinearity

* Pearson correlation matrix
* Color-coded strength visualization
* VIF (Variance Inflation Factor)
* Detection of redundant features

---

### 📐 Hypothesis Testing

* Independent t-test
* One-way ANOVA
* Chi-square test
* Pearson correlation significance

Includes:

* p-values
* effect size indicators
* automatic interpretation (significant vs not)

---

### ⚠️ Outlier Analysis

* IQR-based detection
* Outlier percentage per column
* Range diagnostics

---

### 📈 Visualization

* Auto-generated:

  * histograms
  * scatter plots
  * categorical distributions
* Custom chart builder:

  * bar / line / scatter / pie
  * aggregation support

---

### 🤖 Machine Learning (Baseline)

* Automatic task detection:

  * classification / regression
* Models:

  * k-NN
  * linear regression
* Cross-validation (k-fold)
* Feature importance (correlation + impact)
* Metrics:

  * accuracy
  * R²
  * RMSE

> Designed for quick benchmarking — not production ML.

---

### 🧹 Data Cleaning Assistant

* Detects:

  * missing values
  * outliers
  * high-cardinality columns
* Suggests:

  * imputation
  * winsorization
  * column removal
* Can apply fixes directly

---

### 🧠 Insight & Decision Layer

* Prioritized insights (high / medium / low importance)
* Dataset quality score
* “What to do next” recommendations
* Target column suggestions

---

### 💬 Query Interface (Rule-Based)

* Ask questions about your dataset
* Generates responses using statistical computations
* Works fully offline (no external AI)

---

### 📄 Export

* Text report
* PDF dashboard
* Python code (reproducible analysis)

---

## 🔒 Privacy

* No API calls
* No uploads
* No tracking

Your data stays on your machine.

---

## 🧱 Tech Stack

* Parsing → PapaParse, SheetJS
* Charts → Chart.js
* ML → Vanilla JavaScript
* Stats → Custom implementation
* UI → HTML + CSS
* Deployment → GitHub Pages

---

## ⚡ Performance

* Optimized for small to medium datasets (~10K–100K rows)
* Fully in-memory processing
* No streaming yet

---

## ❗ Limitations

* Not a replacement for pandas / R / production ML
* Limited model variety
* No advanced hyperparameter tuning
* Query system is rule-based (not true LLM AI)
* Large datasets may affect performance

---

## 🛣️ Roadmap

* [ ] Decision tree & Naive Bayes models
* [ ] Better feature importance (permutation-based)
* [ ] Scenario simulation (what-if analysis)
* [ ] Time-series detection
* [ ] Improved query reasoning engine

---

## 🧪 Use Cases

* Quick dataset understanding
* Pre-ML data inspection
* Learning statistics interactively
* Privacy-sensitive analysis
* Rapid prototyping

---

## 🧑‍💻 Run Locally

```bash
git clone https://github.com/bhaskar21-7/datasense
cd datasense
open index.html
```

No install. No dependencies.

---

## 👤 Author

Bhaskar Jha
Statistics Undergraduate

GitHub: https://github.com/bhaskar21-7

---

## ⭐ If This Helps

Star the repo — it improves visibility.

---

## Final Note

This project demonstrates how far **client-side data analysis** can go without backend infrastructure.

It prioritizes:

* speed
* privacy
* accessibility

over complexity.
