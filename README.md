# 🚭 Body Signal Smoking Prediction

An end-to-end Machine Learning pipeline designed to automatically detect smoking habits and analyze physiological damage using objective health screening markers from **55,692 individuals**.

## 📌 Project Overview
This project shifts the focus from self-reported survey datasets to objective clinical testing metrics. By evaluating **27 core bio-signals** (including blood profiles, lipid counts, and metabolic liver enzymes), we mapped out how smoking triggers internal organ stress and built a framework to automate lifestyle risk prediction.

### 🏆 Key Milestone
* Successfully implemented and visualized **ROC-AUC Analysis** across all models to benchmark class-separation authority.
* **Random Forest** emerged as the optimal architecture, securing a **0.917 ROC-AUC score** and **83% general classification accuracy**.

---

## 🛠️ Data Pipeline & Workflow

1. **Data Sanitization:** Audited 55,692 patient records. Dropped zero-variance data points like `oral` and identity indexes (`ID`). Verified 0% missing or duplicate rows.
2. **Exploratory Data Analysis (EDA):** Plotted Age distributions, Cholesterol bells, and correlation matrices to examine data patterns. Identified distinct data rounding biases within manual Systolic Blood Pressure inputs.
3. **Feature Engineering:** Implemented Categorical Encoding for textual signals (`gender`, `tartar`) and deployed `StandardScaler` to realign numerical feature weights.
4. **Validation Mapping:** Engineered a clean **80/20 train-test partition** to maximize unbiased evaluation.
5. **Model Exploration:** Rigorously trained and validated `Logistic Regression`, `XGBoost`, and `Random Forest` models.

---

## 📊 Performance Benchmark Summary

| Model Framework | General Accuracy | Misclassification (False Positives) | ROC-AUC Score |
| :--- | :---: | :---: | :---: |
| **Random Forest Classifier** | **83.0%** | **818 (Lowest Error)** | **0.917 (Excellent)** |
| XGBoost Architecture | 81.2% | 1,125 | 0.861 (Moderate) |
| Logistic Regression | 76.4% | 1,881 | 0.804 (Baseline) |

---

## 🔍 Critical Findings
* **The Younger Demographic Trend:** Boxplot mapping reveals active smokers have a lower median age group, pointing towards critical metabolic exposure risks in the younger demographic.
* **Hepatic & Blood Anomalies:** Smokers exhibit prominent spikes in **Hemoglobin** (thickened blood structure) and purification enzymes like **Gtp** and **ALT**, visually displaying the high toxic filtration stress placed on the liver.
* **Connected Internal Stress:** The correlation heatmap verified powerful ties between body dimensions (Weight vs Waist: 0.82) and cardiovascular tracks (Cholesterol vs LDL: 0.74). Smoking activates systemic stress across these connected pathways.
