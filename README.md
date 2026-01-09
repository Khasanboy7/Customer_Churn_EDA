# Customer Churn EDA

## Overview
This project performs **Exploratory Data Analysis (EDA)** on a customer churn dataset to understand why customers leave a company.  
The goal is to identify **key patterns and insights** that can help predict churn and improve customer retention strategies.

---

## Dataset
The dataset includes information about:
- **Customer demographics**: Gender, SeniorCitizen, Partner, Dependents
- **Services**: InternetService, OnlineSecurity, StreamingTV, etc.
- **Billing & Contracts**: Contract type, PaymentMethod, MonthlyCharges, TotalCharges
- **Target variable**: Churn (Yes/No)

> Note: Dataset should be available as `customer_churn.csv` in the repository or downloaded from [source].

---

## Steps Performed

1. **Data Overview**
   - Checked dataset shape, column types, and missing values.
   - Summarized numeric features.

2. **Categorical Feature Analysis**
   - Explored churn rates for each categorical column.
   - Key findings:
     - Month-to-month contracts have the highest churn.
     - Customers paying via electronic check churn more.
     - Fiber optic users churn more than DSL users.

3. **Numerical Feature Analysis**
   - Analyzed `tenure`, `MonthlyCharges`, and `TotalCharges`.
   - Key findings:
     - Customers with shorter tenure are more likely to churn.
     - Higher monthly charges are associated with higher churn.
   
4. **Visualizations**
   - Boxplots for numerical features vs churn.
   - Bar charts for categorical features vs churn.
   - Correlation heatmap for numeric features.

5. **Insights Summary**
   - Short tenure, month-to-month contracts, high monthly charges, and certain payment methods are the main drivers of churn.
   - Gender and senior citizen status have less impact on churn.

---

## Key Findings

| Feature                  | Observation |
|---------------------------|------------|
| Contract type             | Month-to-month contracts churn the most |
| Tenure                    | Short-tenure customers are more likely to churn |
| MonthlyCharges            | Higher monthly charges increase churn probability |
| PaymentMethod             | Electronic check customers churn more |
| InternetService           | Fiber optic users churn more |

---

## Next Steps
- Encode categorical features for machine learning models.
- Split dataset into train/test sets.
- Apply classification models (Logistic Regression, Random Forest, XGBoost) to predict churn.
- Evaluate models and identify the most important features.

---

## Repository Structure

