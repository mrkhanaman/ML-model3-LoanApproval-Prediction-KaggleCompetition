# 🏦 Machine Learning Model 3: Loan Approval Prediction - Kaggle Competition

**Competition Link:** [Loan Approval Prediction - Playground Series S4E10](https://www.kaggle.com/competitions/playground-series-s4e10/overview)

---

## 📖 Overview

This repository contains the solution for the Kaggle competition *Playground Series - Season 4, Episode 10*. The project focuses on predicting **loan approval statuses** using machine learning techniques based on demographic, financial, and credit history data.

---

## 🛠️ Data Preparation

### 1. **Data Wrangling and EDA**
- Identified and separated **categorical features** (e.g., `person_home_ownership`, `loan_intent`) and **numerical features** (e.g., `person_age`, `loan_amnt`).
- Processed the **target variable (`loan_status`)** into a binary format (0, 1).

### 2. **Cleaning Steps**
- Converted categorical features to numeric types for machine learning compatibility.
- Checked for missing values (none found) and handled potential outliers.

### 3. **Cleaned Data Outputs**
- Exported processed datasets for modeling as:
  - `train_cleaned_data.csv`
  - `test_cleaned_data.csv`

---

## ⚙️ Models Used

### 1. **Linear Regression**
- A baseline model used to evaluate the dataset's potential for prediction using RMSE as the evaluation metric.

### 2. **XGBoost**
- A gradient boosting algorithm that provided excellent performance with:
  - Validation **ROC AUC of 0.9584**, indicating strong classification capabilities.

### 3. **Ridge Regression**
- A regularized linear regression model used for comparison with XGBoost.

---

## 📊 Evaluation and Metrics

- **RMSE (Root Mean Squared Error):**  
  Used to measure the accuracy of the Linear Regression baseline model.

- **ROC-AUC (Receiver Operating Characteristic - Area Under Curve):**  
  - Primary metric for classification performance.
  - **Key Result:** XGBoost achieved a **ROC AUC of 0.9584**, showcasing its effectiveness in loan approval prediction.

---

## 🔑 Results and Insights

- **XGBoost** emerged as the best-performing model, delivering a superior AUC compared to Ridge Regression.
- The cleaned dataset and feature engineering steps were pivotal in achieving robust results.
- ROC curves and AUC values highlighted the clear advantage of XGBoost for this dataset.

---

## 📁 Repository Content

1. **Data Preparation Scripts:** Includes steps for cleaning and exporting train/test datasets.
2. **Model Training Scripts:** Implementations of:
   - Linear Regression
   - Ridge Regression
   - XGBoost
3. **Evaluation Scripts:** Metrics like RMSE, AUC, and ROC curve plots.

---

## 📌 Kaggle Reference

This project is based on the Kaggle competition hosted at [Kaggle.com](https://www.kaggle.com). You can explore the competition details here: [Playground Series - Season 4, Episode 10](https://www.kaggle.com/competitions/playground-series-s4e10/overview).

---

Let me know if you'd like to make further adjustments or add repository-specific links or badges!

> **Note:** Explore the repository to access the code, cleaned datasets, and evaluation results.
>
> Training Dataset: tain.csv
> Testing Dataset = test.csv
>
> Test Dataset after EDA: cleaned_test_data.csv
> Training Dataset after EDA: cleaned_train_data.csv
>
> Predicted Dataset by models: submission.csv
