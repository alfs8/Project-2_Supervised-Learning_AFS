# Project II – MobileNOW Churn Prediction 📱📉

This repository contains the work for **Project II** of the Data Science Master’s thesis at Nuclio Digital School. The focus of this project is on **supervised churn prediction modelling** for the telecommunications company MobileNOW, identifying customers at risk of leaving.

## 🎯 Objective

The goal of this project is to develop a **comprehensive classification model** to predict customer churn probability for the next month. This includes data preprocessing, feature engineering, model training, evaluation, and interpretation of key drivers.

## 📂 Dataset

- **Name:** `telecom_churn_TRAINTEST.csv` & `telecom_churn_PREDICT.csv`
- **Origin:** SQL export from MobileNOW’s corporate database
- **Entries:** Approx. 20,000 rows (train/test), plus prediction set
- **Format:** CSV (tabular data)
- **Main variables:** `customer_id`, `customer_type`, `age`, `tenure_months`, `monthly_usage`, `num_products`, `contract_type`, `has_complaints`, `churn`, etc.

## ⚙️ Project Scope

All steps were implemented within three Jupyter Notebooks and include:

- **Data preprocessing (`ML 1 - Preprocessing.ipynb`):**
  - Initial exploration and statistics
  - Handling missing values and outliers
  - Encoding categorical variables
- **Model development (`ML 2 - Model.ipynb`):**
  - Feature selection and splitting data
  - Training multiple models (Logistic Regression, Random Forest)
  - Hyperparameter tuning and cross-validation
- **Prediction workflow (`ML 3 - Predict.ipynb`):**
  - Loading the final model and scaler
  - Generating churn probability scores for new data
  - Exporting results to `predictions/churn_scores.csv`

## 📊 Results Summary

The final deliverables include:

- A **trained classification model** with evaluation metrics (AUC-ROC, F1-score, Precision@Top5%)
- **Insights** into the top factors driving churn
- **`predictions/churn_scores.csv`** containing `customer_id` and `churn_probability`

All transformations and modelling decisions are documented and justified to ensure reproducibility and clarity.

## 📄 Repository Contents

- `ML 1 - Preprocessing.ipynb`  
  Notebook documenting data cleaning and preprocessing steps.

- `ML 2 - Model.ipynb`  
  Notebook covering model training, validation, and selection.

- `ML 3 - Predict.ipynb`  
  Notebook for loading the model and generating final predictions.

- `DATA/telecom_churn_TRAINTEST.csv`  
  Historical data used for training and testing the model.

- `DATA/telecom_churn_PREDICT.csv`  
  Data set for which churn probabilities are to be predicted.

- `data/cleaned/`  
  Cleaned datasets produced by preprocessing.

- `models/churn_model.pkl` & `models/scaler.pkl`  
  Serialized model and scaler objects.

- `predictions/churn_scores.csv`  
  Output file with churn predictions.

- `requirements.txt`  
  List of Python dependencies.

- `README.md`  
  This file.

## 🗓️ Delivery Info

- **Deadline:** June 30, 2025, 23:59 CEST  
- **Submission format:** PDF report and Jupyter Notebooks  
- **Notebook filenames:** `ML 1 - Preprocessing.ipynb`, `ML 2 - Model.ipynb`, `ML 3 - Predict.ipynb`

## 🚀 How to Run

1. Install dependencies:  
   ```bash
   pip install -r requirements.txt
