# Lithium-Ion-Battery-Health-Analytics
An end-to-end Python data pipeline and machine learning regression model to predict operational degradation patterns in Lithium-ion batteries.
# 📊 Machine Learning-Based State-of-Health (SoH) Estimation of Lithium-Ion Batteries Using a Dual-Model Approach

**Author:** Jana Abdelrehim  
**Institution:** University of the West of England (UWE Bristol) — Mechatronics Engineering  

---

## 📌 1. Project Overview

This repository implements a complete, self-contained end‑to‑end machine learning pipeline for estimating the **State‑of‑Health (SoH)** and forecasting degradation curves in lithium‑ion batteries using the benchmark **NASA B0005 dataset**. 

The entire workflow—encompassing structural data extraction, data cleaning, feature engineering, statistical visualization, and predictive model training—is compiled cleanly within a single deployment file (`Confrence_Letter.ipynb`).

### 🤖 Dual-Model Architecture Strategy
To provide comprehensive battery analytics, the framework splits tasks across two distinct algorithms:
1. **Multiple Linear Regression (MLR):** Deployed for continuous, real-time capacity degradation and SoH prediction.
2. **Random Forest Classifier (RF):** Deployed as a predictive safety gate to handle discrete **End‑of‑Life (EoL)** anomaly detection the moment capacity drops below the critical 1.4 Ah threshold.

---

## 💻 2. Environment & Technical Requirements

To ensure full reproducibility of the analytical results, verify your local environment satisfies the following baseline specifications:

* **Python Version:** `3.10.x` (Backward compatible with `3.9+`)
* **Core Dependencies Stack:**
  * `pandas` — High-performance data loading, multi-index manipulation, and data wrangling.
  * `numpy` — Multi-dimensional vector operations and direct mathematical regression fitting.
  * `matplotlib` — Technical publication-quality plotting and schematic figure generation.
  * `seaborn` — Advanced statistical visualizations (correlation heatmaps, distribution histograms, and boxplots).
  * `scikit-learn` — Pipeline management (Train/Test split architectures, Standard Scalers, MLR, Random Forest evaluation metrics).
  * `os` — Internal system directory and file checking during chronological cycle extraction.

### 📦 Installation
Initialize your virtual environment and install all dependencies via `pip`:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
