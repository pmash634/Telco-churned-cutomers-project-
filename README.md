# Telco Customer Churn Analysis

An end-to-end analysis of customer churn for a telecom company, from data cleaning in Python to an interactive Power BI dashboard.

## Problem Statement
Customer churn is costly for telecom companies, because acquiring a new customer often costs more than keeping an existing one. In this dataset, about 27% of customers left. The business needs to know **which customers are leaving, when they leave, and what drives it**, so it can act before more customers are lost.

## Objective
Analyse customer data to identify the groups most at risk of churning, and present the findings in an interactive dashboard that supports retention decisions.

## Dataset
Telco Customer Churn dataset ([ Kaggle]), with 7,043 customers and details on contracts, internet services, payment methods, tenure and charges.

## Tools
- **Python** (Pandas, NumPy) in Google Colab for data cleaning and exploration
- **Power BI** for the dashboard, DAX measures and visuals

## Process
1. **Data cleaning (Python):** [.fixed the TotalCharges data type, handled missing values, removed duplicates, standardised categories]
2. **Exploratory analysis (Python):** [churn across contract types, tenure and charges]
3. **Dashboard (Power BI):**
   - Loaded the cleaned CSV and checked data types in Power Query
   - Created DAX measures: Total Customers, Churned Customers, Churn Rate and Avg Monthly Charges
   - Created a calculated column, Tenure Group, to group customers by months of tenure
   - Built KPI cards, charts and slicers

## Dashboard Contents
**KPI cards:** Total Customers, Churned Customers, Churn Rate, Avg Monthly Charges

**Charts:**
- Churn Rate by Contract Type
- Churn Rate by Internet Service
- Churn Rate by Payment Method
- Churn Rate by Tenure Group
- Churned vs Retained Customers (donut)

**Slicers:** Contract, Internet Service, Gender

## Key Findings
- **Overall churn rate is about 27%** (1,869 of 7,043 customers).
- **Month-to-month contracts churn the most** (about 42%), compared with about 3% for two-year contracts.
- **New customers are most at risk:** customers in their first 12 months churn at about 48%.
- **Electronic check users churn at about 45%**, far above other payment methods (about 15-19%).
- **Fibre optic customers churn more than DSL customers.**

## Recommendations
- Offer incentives to move month-to-month customers onto longer contracts.
- Improve onboarding and early support for customers in their first year.
- Encourage electronic check customers to switch to automatic payment.
- Investigate pricing and service quality for fibre optic customers.

## Limitations
- The findings show relationships, not proven causes. For example, electronic check users may also be mostly on month-to-month contracts.
- The analysis is descriptive and does not include a predictive model.

## Repository Structure
```
telco-churn-analysis/
├── README.md
├── data/
│   └── telco_churn_cleaned.csv
├── notebook/
│   └── telco_churn_cleaning.ipynb
├── dashboard/
│   ├── Telco_Churn_Dashboard.pbix
│   └── dashboard.pdf
└── images/
    └── dashboard.png
```

## How to Use
1. Open the notebook in Google Colab to see the data cleaning steps.
2. Open the `.pbix` file in Power BI Desktop to explore the dashboard.
3. Use the slicers to filter by contract, internet service and gender.

## Author
**Purity Wanjiku Macharia**
BSc Applied Statistics with Programming | Aspiring Data and BI Analyst
[LinkedIn](https://www.linkedin.com/in/purity-wanjiku-11581b200) | [GitHub](https://github.com/pmash634) | puritymacharia111@gmail.com
