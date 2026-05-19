# Stroke Risk Analysis

A machine learning project that analyzes risk factors associated with stroke using a dataset of 5,110 patient records. Multiple classification models were built, tuned, and compared to identify the best predictor of stroke risk.

## Overview

Stroke is one of the leading causes of death and disability worldwide. This project explores which health and lifestyle factors are most associated with stroke risk, and builds predictive models to classify patients as stroke or non-stroke cases.

## Dataset

- 5,110 patient records
- Source: loaded via Google Drive
- Features include: age, gender, hypertension, heart disease, marital status, work type, residence type, average glucose level, BMI, and smoking status
- Target variable: stroke (0 = No, 1 = Yes)

## Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (KNN, Logistic Regression, Random Forest, SVC)

## Project Workflow

1. **Data Examination** — explored shape, data types, and summary statistics
2. **Data Cleaning** — handled missing BMI values using imputation
3. **Preprocessing** — scaled features with StandardScaler, encoded categorical variables
4. **Baseline Models** — trained and evaluated KNN, Logistic Regression, Random Forest, and SVC
5. **Model Tuning** — tuned hyperparameters to improve recall for stroke cases
6. **Model Comparison** — compared accuracy, precision, recall, and F1 scores across all models using classification reports and confusion matrices

## Key Finding

Most baseline models achieved high accuracy but failed to detect actual stroke cases due to class imbalance. After tuning, **Logistic Regression** was selected as the final model because it achieved the highest recall for stroke cases while maintaining strong overall performance.

## How to Run

1. Clone the repo
   ```
   git clone https://github.com/yourusername/stroke-risk-analysis
   ```
2. Install dependencies
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open the notebook
   ```
   jupyter notebook Stroke_Risk_Analysis_Report_Group_2_CIS9660.ipynb
   ```
