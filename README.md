# Chronic-Kidney-Disease-CKD-Prediction-
End-to-end CKD prediction project using machine learning. Covers data cleaning, EDA, feature importance, and high-recall models, along with an interactive Power BI dashboard for clinical insights.


Project Overview

This project focuses on predicting Chronic Kidney Disease (CKD) using machine learning techniques. The goal is to assist in early diagnosis, which is critical in healthcare to prevent severe complications.

The project covers:

Data cleaning & preprocessing
Exploratory Data Analysis (EDA)
Feature engineering
Model building (Logistic Regression & Random Forest)
Model evaluation
Dashboard creation (Power BI)
Dataset Information
Total Records: 400 patients
Total Features: 26
Includes:
Demographic data (age, blood pressure)
Lab test results (hemoglobin, creatinine, etc.)
Medical conditions (hypertension, diabetes)
 
 Data Preprocessing

Key steps performed:

Handled missing values:
Numerical → filled using median
Categorical → filled using mode
Converted data types
Replaced invalid values (?) with NaN
Encoded categorical variables
Target encoding:
ckd → 1
notckd → 0

Exploratory Data Analysis (EDA)
Key Insights:
CKD patients tend to have:
Lower hemoglobin levels
Higher serum creatinine levels
Clear separation observed between CKD and non-CKD patients
Visualizations Used:
Distribution plots
Boxplots (for outliers & comparison)
Count plots (categorical features)
Correlation heatmap

Models Used
1. Logistic Regression
Applied with standardization
Hyperparameter tuning using GridSearchCV
2. Random Forest
Used for:
Prediction
Feature importance analysis

Feature Importance (Top Predictors)

Important features identified:

PCV (Packed Cell Volume)
Hemoglobin
Serum Creatinine
Specific Gravity
Albumin

These features play a crucial role in detecting CKD.

Model Performance
Metric	Logistic Regression
Accuracy	98%
Recall	96%
Precision	High

Key Insight:

Recall is very important in medical diagnosis.
The model ensures minimal false negatives, meaning CKD patients are not missed.

Confusion Matrix Insight
Very few misclassifications
Strong ability to distinguish CKD vs Non-CKD

Dashboard (Power BI)

The dashboard provides:

Total patients overview
CKD vs Non-CKD distribution
Risk score distribution
Feature relationship visualization
Filters for:
Age
Diabetes
Hypertension

Dashboard Insights:
CKD patients show higher risk scores
Hemoglobin and creatinine are strong indicators
Model performs reliably for early detection

Tools & Technologies
Python (Pandas, NumPy, Scikit-learn)
Matplotlib & Seaborn
Power BI
Jupyter Notebook
