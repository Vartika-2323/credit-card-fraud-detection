# credit-card-fraud-detection
End-to-end ML pipeline for detecting fraudulent credit card transactions (284K+ real-world transactions, 0.17% fraud rate) using Logistic Regression, Random Forest, and Balanced Random Forest — 99.96% accuracy.
# Credit Card Fraud Detection — Predictive Analytical Model

End-to-end machine learning pipeline for detecting fraudulent credit card transactions.

## Overview
- **Dataset:** 284,807 real-world anonymized credit card transactions (0.17% fraud rate)
- **Goal:** Build a reliable classification model to flag fraudulent transactions while minimizing false negatives (the higher-priority metric in fraud risk management)

## Approach
- Data wrangling, feature engineering, normalization, and stratified train/test splits for reproducibility
- Compared 3 classification models: Logistic Regression, Random Forest, Balanced Random Forest

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Random Forest | 99.96% | 0.94 | 0.83 | 0.88 |

**Key insight:** Minimizing false negatives (missed fraud cases) is more operationally critical than overall accuracy — informing which model and threshold to prioritize for deployment.

## Data
Full dataset (150MB): [Kaggle source](https://www.kaggle.com/datasets/vartikasri1112/credit-card-fraud-detection)
This repo includes `creditcard_sample.csv` — a stratified 40,000-row sample preserving the original 0.17% fraud ratio, for quick exploration without downloading the full file.

## Tools
Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
