## Credit Risk Prediction

Credit default prediction is a core component of consumer lending risk management. Accurate identification of high-risk borrowers directly impacts loan loss reserves, portfolio risk exposure, and regulatory capital requirements. This project simulates a risk analyst workflow applicable to retail banking, credit risk model validation, and financial institution risk management.

⸻

## Project Objective

The objective of this project is to predict whether a borrower will default on a loan using demographic, financial, and credit-related information.

This project demonstrates a complete end-to-end machine learning workflow commonly used in financial risk analytics.

⸻

## Workflow

- Data Cleaning

- Exploratory Data Analysis (EDA)

- Feature Engineering

- Logistic Regression

- Random Forest

- Cross Validation

- Permutation Importance

- SHAP Explainability

- Model Comparison Dashboard

⸻

## Project Structure

01 — Data Cleaning & EDA

* Data cleaning
* Missing value analysis
* Outlier treatment
* Target distribution analysis
* Correlation analysis

02 — Feature Engineering

* Missing value treatment
* Categorical encoding
* Engineered financial indicators
* Correlation evaluation

03 — Model Development

* Train-test split
* Logistic Regression
* Random Forest
* Model evaluation

04 — Model Explainability

* Cross Validation
* Permutation Importance
* SHAP Analysis
* Feature Interpretation

05 — Model Comparison Dashboard

* Accuracy comparison
* Recall comparison
* Precision comparison
* F1-score comparison

⸻

## Feature Engineering

The following engineered features were created:

Feature	Description
Income-to-Loan Ratio	Measures borrower affordability
Credit History Ratio	Measures credit maturity relative to age
Employment Stability	Measures employment consistency
Interest Burden	Measures repayment burden relative to income

⸻

## Model Performance

Model	Accuracy	Recall	Precision	F1 Score
Logistic Regression	0.81	0.17	0.70	0.28
Random Forest	0.87	0.62	0.75	0.68

⸻

## Cross Validation

Random Forest achieved:

* Mean Accuracy: 85.2%
* Standard Deviation: 1.2%

This indicates stable performance across multiple data splits.

⸻

## Most Important Features

According to Permutation Importance and SHAP Analysis:

1. Loan Grade
2. Income-to-Loan Ratio
3. Interest Burden
4. Loan Percent Income
5. Borrower Income

⸻

## SHAP Explainability

SHAP analysis was used to explain how individual features influence default predictions.

Key findings:

* Higher loan grades (riskier borrowers) increase default probability.
* Higher income-to-loan ratios reduce default probability.
* Larger loan burdens increase default probability.
* Engineered features significantly improved model performance.

⸻

## Key Results

* Random Forest outperformed Logistic Regression across all major metrics.
* Feature engineering substantially improved predictive power.
* Cross validation confirmed model stability.
* SHAP provided interpretable explanations for model behavior.

⸻

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* SHAP
* Jupyter Notebook

⸻

## Future Improvements

* XGBoost
* Hyperparameter Tuning
* ROC-AUC Optimization
* Streamlit Deployment
* Real-Time Credit Risk Dashboar
