# **Predicting Loan Repayment**

## **Overview**
This project aims to predict whether a customer will fully repay their loan or default based on various financial and behavioral features. Using machine learning models, we identify high-risk customers and provide actionable insights for financial institutions to optimize their credit risk management.

## **Problem Statement**
Loan defaults can lead to significant losses for financial institutions. This project focuses on predicting customer repayment behavior using machine learning to:
- Reduce loan default rates
- Improve risk assessment and loan approval processes
- Offer better incentives for low-risk customers

## **Dataset**
The dataset consists of two primary sources:
1. **Application Train**: Customer information at the time of loan application.
2. **Previous Application**: History of past loan applications.

Key features used in modeling:
- `NAME_CONTRACT_STATUS`: Status of previous loan applications (Approved, Canceled, Refused, Unused Offer).
- `AMT_CREDIT`: Loan amount requested.
- `AMT_INCOME_TOTAL`: Customer's total income.
- `CREDIT_TO_INCOME_RATIO`: Ratio of requested credit to total income.
- `COUNT_REFUSED`: Number of previously refused loan applications.
- `TARGET`: Loan repayment status (1: Default, 0: Fully Paid).

## **Exploratory Data Analysis (EDA) Insights**
### **Insight 1: Customers with More Rejected Loan Applications Have a Higher Risk of Default**
- Customers with multiple previously refused applications show a significantly higher probability of default.
- **Actionable Steps:**
  - Implement a **risk-based scoring system** considering past loan rejections.
  - Provide **financial literacy programs** for customers with frequent refusals.

### **Insight 2: Customers with a High Credit-to-Income Ratio Are More Likely to Default**
- Borrowers with a credit-to-income ratio above **50%** are at a higher risk of default.
- **Actionable Steps:**
  - Set a **maximum credit-to-income ratio threshold**.
  - Adjust interest rates based on credit-to-income risk levels.

## **Machine Learning Models**
We implemented the following models:
1. **XGBoost**
2. **Random Forest**
3. **Logistic Regression**
