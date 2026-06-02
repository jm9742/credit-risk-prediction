Credit Risk Prediction

A machine learning project for predicting borrower default risk using demographic, financial, and credit-related information.

Project Overview

This project develops and evaluates machine learning models for credit risk assessment using structured lending data.

The workflow includes:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Logistic Regression
* Random Forest
* Cross Validation
* Permutation Importance
* SHAP Explainability
* Model Comparison Dashboard

Dataset

The dataset contains borrower-level lending information including:

* Age
* Income
* Employment Length
* Loan Amount
* Interest Rate
* Loan Grade
* Credit History

Target Variable

loan_status

* 0 = Non-default
* 1 = Default

After cleaning, the dataset contains 31,521 borrower records.

Project Structure

01_data_cleaning_eda.ipynb

* Data cleaning
* Missing value analysis
* Outlier detection
* Exploratory data analysis
* Correlation analysis

02_feature_engineering.ipynb

* Categorical encoding
* Feature engineering
* Engineered feature evaluation
* Correlation heatmap

03_modeling_evaluation.ipynb

* Train-test split
* Logistic Regression
* Random Forest
* Model evaluation
* Feature importance analysis

04_shap_explainability.ipynb

* Cross validation
* Permutation importance
* SHAP explainability
* Model interpretation

05_model_comparison_dashboard.ipynb

* Model comparison
* Accuracy comparison
* Recall comparison
* Precision comparison
* F1-score comparison

Feature Engineering

Several financial risk indicators were created:

Income-to-Loan Ratio

Measures borrower affordability.

Income / Loan Amount

Credit History Ratio

Measures credit maturity relative to borrower age.

Credit History Length / Age

Employment Stability

Measures employment experience relative to borrower age.

Employment Length / Age

Interest Burden

Measures repayment burden relative to borrower income.

Interest Rate / Income

Model Performance

Model	Accuracy	Recall	Precision	F1 Score
Logistic Regression	0.81	0.17	0.70	0.28
Random Forest	0.87	0.62	0.75	0.68

Cross Validation

Random Forest achieved a mean cross-validation accuracy of approximately 85.2% with low variance across folds, indicating stable model performance.

Permutation Importance Findings

Permutation importance confirmed that engineered financial features contributed significantly to model performance.

The most important features included:

1. Income-to-Loan Ratio
2. Loan Grade
3. Borrower Income
4. Loan Percent Income
5. Employment Length

SHAP Findings

SHAP analysis confirmed that the most influential drivers of borrower default risk were:

1. Loan Grade
2. Income-to-Loan Ratio
3. Interest Burden
4. Loan Percent Income

The results validated the effectiveness of the feature engineering process and provided interpretable explanations for model predictions.

Key Findings

* Random Forest significantly outperformed Logistic Regression.
* Borrower affordability is one of the strongest predictors of default risk.
* Feature engineering improved predictive performance.
* Cross validation demonstrated stable model performance.
* SHAP analysis provided interpretable explanations for model behavior.

Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* SHAP
* Jupyter Notebook

Future Improvements

Potential future enhancements include:

* XGBoost implementation
* Hyperparameter tuning
* ROC-AUC analysis
* Precision-Recall optimization
* Streamlit dashboard deployment
* Real-time credit risk scoring
* Alternative explainability methods
* Model monitoring and drift detection

