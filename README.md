# Credit Card Fraud Detection

## Overview
Machine Learning project focused on detecting fraudulent credit card transactions in a highly imbalanced dataset containing over 6 million transactions with only 0.17% fraud cases.

The project benchmarks multiple machine learning algorithms and deploys the best-performing model through an interactive Streamlit web application.

---

## Problem Statement

Credit card fraud detection is a challenging classification problem due to severe class imbalance, where fraudulent transactions represent a very small fraction of the data.

The objective was to build a model capable of maximizing fraud detection while minimizing false positives.

---

## Dataset

- Transactions: 6M+
- Fraud Cases: 0.17%
- Type: Binary Classification
- Target Variable: `isFraud`

---

## Methodology

### Data Preprocessing
- Missing value handling
- One-Hot Encoding
- Feature Scaling
- Cost-Sensitive Learning

### Models Evaluated
- Logistic Regression
- Random Forest
- XGBoost

### Validation Strategy
- Stratified Train-Test Split
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC

---

## Results

| Model | Precision | Recall | F1 Score |
|---------|---------|---------|---------|
| Logistic Regression | 0.022 | 0.947 | 0.044 |
| Random Forest | 0.080 | 0.993 | 0.148 |
| XGBoost | 0.312 | 0.994 | 0.475 |

### Best Model: XGBoost

- Recall: 99.4%
- ROC-AUC: 0.999
- PR-AUC: 0.938

---

## Deployment

The final XGBoost model was deployed using Streamlit, allowing users to enter transaction details and receive fraud predictions in real time.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Streamlit
- Matplotlib
- Seaborn

---

## Future Improvements

- Hyperparameter Optimization
- SHAP Explainability
- Real-time API Deployment
- Model Monitoring
