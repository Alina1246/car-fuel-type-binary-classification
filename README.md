# Car Fuel Type Binary Classification

Machine Learning project for binary classification of car fuel type (Gasoline vs Diesel).

---

## Project Overview

The objective of this project is to compare multiple supervised learning models in order to identify the most effective approach for predicting vehicle fuel type.

The classification task was simplified to a **binary problem** by filtering the dataset to include only:
- Gasoline
- Diesel

---

## Models Implemented

The following models were trained and evaluated:

- **Logistic Regression** (with GridSearchCV hyperparameter tuning)
- **Random Forest** (with GridSearchCV hyperparameter tuning)
- **XGBoost** (optimized using Optuna)

---

## Methodology

The following techniques were applied:

- Data filtering and preprocessing
- OneHot Encoding for categorical features
- Stratified train/test split
- Stratified K-Fold cross-validation
- Hyperparameter tuning:
  - GridSearchCV (Logistic Regression, Random Forest)
  - Optuna optimization (XGBoost)
- Model evaluation using:
  - Accuracy
  - F1-macro score
  - Confusion Matrix
  - Classification Report

---

## Final Results

XGBoost optimized with Optuna and including the `name` feature achieved the best overall performance, obtaining:

- Highest **F1-macro (test)**
- Highest **Test Accuracy**
- Strong cross-validation performance

Random Forest showed stable results, while Logistic Regression was more sensitive to feature removal.

Overall, **XGBoost proved to be the most suitable model for this task.**
