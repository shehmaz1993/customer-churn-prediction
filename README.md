# Customer Churn Prediction Using Machine Learning

**Author:** Kazi Shehmaz Islam  
**Date:** September 2026  
**Repository:** [github.com/shehmaz1993/customer-churn-prediction](https://github.com/shehmaz1993/customer-churn-prediction)

---

## 📌 Project Overview
This repository contains an end-to-end machine learning study predicting subscriber churn on the Telco dataset (7,043 records). The primary objective is to evaluate multiple supervised classification algorithms, identify high-risk churn indicators, and deliver actionable retention strategies to protect customer lifetime value.

---

## 📄 Key Deliverables
- **Research Paper:** [`paper.md`](paper.md) — Full study including abstract, methodology, results, discussion, and Zotero-formatted references.
- **Jupyter Notebook:** [`notebook.ipynb`](notebook.ipynb) — Executed data cleaning, model training, evaluation, and feature extraction code.
- **Presentation Deck:** [`slides.md`](slides.md) — 6-slide presentation covering the problem, methodology, benchmark results, and strategic takeaways.
- **Figures & Charts:** [`figures/`](figures/) — Visualizations of model comparison benchmarks and XGBoost feature importance distributions.

---

## 📊 Model Evaluation Benchmark

Evaluated four supervised classification models across a stratified 80/20 train-test holdout split:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Logistic Regression** | **0.8055** | **0.6572** | **0.5588** | **0.6040** | **0.8419** |
| XGBoost | 0.7963 | 0.6390 | 0.5348 | 0.5822 | 0.8369 |
| Support Vector Machine (SVM) | 0.7913 | 0.6418 | 0.4840 | 0.5518 | 0.7905 |
| Random Forest | 0.7779 | 0.6034 | 0.4759 | 0.5321 | 0.8162 |

> **Key Finding:** **Logistic Regression** achieved superior performance with an ROC-AUC of **0.8419**, demonstrating that linear decision boundaries are highly effective following standard feature scaling.

---

## 🔑 Primary Churn Drivers
Tree-based feature attribution identified two critical subscriber risk factors accounting for **>74% of predictive churn weight**:
1. **Contract Type:** `Month-to-month` (46.3% relative importance)
2. **Internet Service:** `Fiber Optic` (28.0% relative importance)

---

## 💡 Strategic Takeaway
To mitigate churn effectively, telecommunications providers should deploy targeted multi-month contract conversion incentives and bundle value-added services (such as online security) specifically for high-tier Fiber Optic subscribers before critical renewal windows.
