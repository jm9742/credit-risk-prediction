Credit Risk Prediction

Machine learning project for predicting borrower default risk using borrower demographics, loan characteristics, and engineered financial indicators.

Project Overview

This project develops machine learning models to predict whether a borrower will default on a loan.

The workflow includes:

* Data cleaning
* Exploratory data analysis (EDA)
* Feature engineering
* Logistic Regression
* Random Forest
* Model evaluation

Dataset

The dataset contains borrower-level information including:

* Age
* Income
* Employment length
* Loan amount
* Interest rate
* Loan grade
* Credit history

Target variable:

* loan_status
    * 0 = Non-default
    * 1 = Default

Project Structure

* 01_data_cleaning_eda.ipynb
* 02_feature_engineering.ipynb
* 03_modeling_evaluation.ipynb

Model Results

Model	Accuracy
Logistic Regression	80.8%
Random Forest	87.4%

Key Findings

Random Forest outperformed Logistic Regression and achieved higher accuracy while capturing substantially more default borrowers.

The most important predictive features were:

1. Income-to-loan ratio
2. Loan percent income
3. Loan grade
4. Interest burden
5. Interest rate

These results suggest that borrower repayment capacity is one of the strongest drivers of default risk.
