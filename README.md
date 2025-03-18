# Loan Prediction Model

## Project Overview
This project implements a machine learning model to predict loan approval status for a financial company. The goal is to automate the loan eligibility process based on customer details provided in the application form.

## Problem Statement
Dream Housing Finance company deals with all home loans. They have a presence across all urban, semi-urban, and rural areas. Customer-first applies for a home loan, after which the company validates the customer's eligibility. The company wants to automate the loan eligibility process based on customer details provided in the online application form.

These details include:
- Gender
- Marital Status
- Education
- Number of Dependents
- Income
- Loan Amount
- Credit History
- and others

To automate this process, they have provided a dataset to identify the customer segments eligible for loan amounts to target these customers specifically.

## Dataset
The dataset contains the following features:
- **Loan_ID**: Unique Loan ID
- **Gender**: Male/Female
- **Married**: Applicant married (Y/N)
- **Dependents**: Number of dependents
- **Education**: Applicant Education (Graduate/Not Graduate)
- **Self_Employed**: Self-employed (Y/N)
- **ApplicantIncome**: Applicant income
- **CoapplicantIncome**: Coapplicant income
- **LoanAmount**: Loan amount in thousands
- **Loan_Amount_Term**: Term of the loan in months
- **Credit_History**: Credit history meets guidelines (1=Yes, 0=No)
- **Property_Area**: Urban/Semi-Urban/Rural
- **Loan_Status**: Loan approved (Y/N) - Target variable

## Project Structure
The project is structured as follows:
1. Data Exploration & Visualization
2. Data Preprocessing
   - Missing value imputation
   - Feature encoding
   - Feature transformation
3. Feature Engineering
4. Model Building
   - Logistic Regression
   - Random Forest
   - Gradient Boosting
5. Model Evaluation
   - Cross-validation
   - Performance metrics
6. Feature Importance Analysis
7. Prediction on Test Data

## Key Insights from Exploratory Data Analysis
- Credit history plays a crucial role in loan approval (customers with a good repayment history have higher approval rates)
- Property location affects loan approval (semi-urban properties have higher approval rates)
- Married applicants have a higher loan approval rate
- Total income (applicant + co-applicant) affects loan approval rates
- There's no significant difference in approval rates based on gender

## Model Performance
The Gradient Boosting model achieved the best performance with:
- Accuracy: ~83%
- Precision: ~84%
- Recall: ~94%
- F1-Score: ~89%

## Important Features
The top predictors for loan approval are:
1. Credit History
2. Total Income (Applicant + Co-applicant)
3. Loan Amount
4. Property Area

## Requirements
- Python 3.6+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Usage
1. Clone the repository:
```bash
git clone https://github.com/yourusername/loan-prediction.git
cd loan-prediction
