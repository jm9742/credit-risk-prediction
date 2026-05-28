Credit Risk Prediction

Machine learning project for predicting borrower default risk using borrower demographics, loan characteristics, and engineered financial indicators.

Project Overview

This project develops and evaluates machine learning models for credit risk assessment using structured lending data.

The objective is to predict whether a borrower is likely to default on a loan based on financial characteristics, employment history, credit history, and loan information.

The project follows a complete end-to-end data science workflow:

* Data cleaning and preprocessing
* Exploratory data analysis (EDA)
* Feature engineering
* Machine learning modeling
* Model evaluation
* Feature importance analysis

⸻

Dataset

The dataset contains borrower-level lending information, including:

* Borrower age
* Annual income
* Employment length
* Loan amount
* Interest rate
* Loan grade
* Home ownership status
* Loan purpose
* Credit history length

Target Variable

loan_status

* 0 = Non-default
* 1 = Default

After cleaning:

* 31,521 borrower records
* 24 engineered and transformed features

⸻

Project Structure

credit-risk-prediction/
├── README.md
├── 01_data_cleaning_eda.ipynb
├── 02_feature_engineering.ipynb
├── 03_modeling_evaluation.ipynb
└── feature_importance.png

⸻

Data Cleaning

Key preprocessing steps included:

* Removal of unrealistic borrower ages
* Removal of unrealistic employment lengths
* Duplicate record removal
* Missing value treatment
* Data quality assessment

⸻

Exploratory Data Analysis

Key findings:

* Default rate ≈ 22%
* Non-default rate ≈ 78%
* Lower-income borrowers exhibit higher default rates
* Poorer loan grades show substantially higher default probabilities
* Higher interest rates are associated with elevated default risk

⸻

Feature Engineering

Several borrower-level risk indicators were created:

Income-to-Loan Ratio

Measures borrower affordability.

Income / Loan Amount

Higher values generally indicate stronger repayment capacity.

⸻

Credit History Ratio

Measures credit maturity relative to borrower age.

Credit History Length / Age

⸻

Employment Stability

Measures employment experience relative to borrower age.

Employment Length / Age

⸻

Interest Burden

Measures repayment burden relative to borrower income.

Interest Rate / Income

⸻

Models

Logistic Regression

Used as a baseline classification model.

Results:

* Accuracy: 80.8%
* Recall (Default Borrowers): 17%

Although overall accuracy was reasonable, the model struggled to identify default borrowers.

⸻

Random Forest

Used to capture non-linear borrower risk patterns.

Results:

* Accuracy: 87.4%
* Recall (Default Borrowers): 62%

The Random Forest model significantly outperformed Logistic Regression in identifying high-risk borrowers.

⸻

Model Comparison

Model	Accuracy	Recall (Default Borrowers)
Logistic Regression	80.8%	17%
Random Forest	87.4%	62%

⸻

Feature Importance

The most important predictive features were:

1. Income-to-Loan Ratio
2. Loan Percent Income
3. Loan Grade
4. Interest Burden
5. Loan Interest Rate

These results suggest that borrower repayment capacity is one of the strongest drivers of default risk.

⸻

Key Findings

* Random Forest substantially outperformed Logistic Regression.
* Borrower affordability metrics were the strongest predictors of default.
* Loan burden relative to income plays a critical role in repayment performance.
* Feature engineering significantly improved model interpretability and predictive power.

⸻

Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

⸻

Future Improvements

Potential future enhancements include:

* XGBoost and Gradient Boosting models
* Hyperparameter optimization
* Cross-validation
* Probability calibration
* SHAP explainability analysis
* Production deployment pipeline
* Real-world lending datasets
