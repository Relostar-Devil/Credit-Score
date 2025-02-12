# Classification - Credit Score

## Overview

This repository contains a comprehensive data science project aimed at classifying credit scores based on individuals’ financial profiles. It demonstrates an end-to-end workflow—from data ingestion and cleaning to feature engineering, model building, hyperparameter tuning, and evaluation—using various machine learning algorithms such as Logistic Regression, Decision Trees, and Random Forest.

## Problem Statement

Manual classification of credit scores in large-scale finance settings can be time-consuming and error-prone. This project provides an intelligent system that automatically classifies individuals into credit score brackets (e.g., Poor, Standard, Good) based on their credit-related information, thereby reducing manual efforts and increasing efficiency.

## Dataset Information

- **Records:** 100,000 entries
- **Features:** 22 columns including:
  - `Month`
  - `Age`
  - `Occupation`
  - `Annual_Income`
  - `Monthly_Inhand_Salary`
  - `Num_Bank_Accounts`
  - `Num_Credit_Card`
  - `Interest_Rate`
  - `Num_of_Loan`
  - `Delay_from_due_date`
  - `Num_of_Delayed_Payment`
  - `Changed_Credit_Limit`
  - `Num_Credit_Inquiries`
  - `Credit_Mix`
  - `Outstanding_Debt`
  - `Credit_Utilization_Ratio`
  - `Payment_of_Min_Amount`
  - `Total_EMI_per_month`
  - `Amount_invested_monthly`
  - `Payment_Behaviour`
  - `Monthly_Balance`
  - **Target:** `Credit_Score`


## Methodology

- **Data Preprocessing:**
  - Importing libraries (`pandas`, `numpy`, `matplotlib`, etc.).
  - Cleaning data by replacing special characters, converting data types, and handling missing values.
  - Feature engineering, including one-hot encoding for categorical variables and feature selection based on Variance Inflation Factor (VIF).

- **Modeling:**
  - **Logistic Regression:** Baseline model achieving ~61.8% accuracy.
  - **Decision Tree:** Initial accuracy around 69.7%, improved to ~70.93% with hyperparameter tuning using GridSearchCV.
  - **Random Forest:** Demonstrated superior performance with ~79.7% accuracy.

- **Evaluation:**
  - Splitting data into training and testing sets.
  - Assessing models based on accuracy scores and other performance metrics.

## Results and Insights

Using robust data cleaning and feature selection techniques, the Random Forest model in this project achieves the highest accuracy (~79.7%) for credit score classification. These insights underline the importance of model selection and hyperparameter tuning in building reliable predictive systems for finance applications.
