#  Customer Churn Analysis (SQL + Power BI)

##  Project Overview
This project focuses on analyzing customer churn behavior using SQL Server and Power BI. It involves building a complete ETL pipeline, performing data cleaning and transformation, and creating an interactive dashboard to uncover key business insights.

---

##  Tech Stack
- SQL Server (SSMS)
- Power BI
- SQL
- Excel

---

##  Project Workflow

### 1. ETL Process (SQL Server)
- Created database: `db_Churn`
- Imported raw CSV data into staging table (`stg_Churn`)
- Handled data quality issues:
  - Replaced NULL values using `ISNULL`
  - Standardized categorical fields
- Loaded clean data into production table (`prod_Churn`)
- Created views:
  - `vw_ChurnData` → Churned & Stayed customers
  - `vw_JoinData` → New customers

---

### 2. Data Exploration (SQL)
- Analyzed:
  - Gender distribution
  - Contract types
  - State-wise churn
  - Revenue contribution
- Calculated percentages using SQL aggregations
- Performed null value analysis across all columns

---

### 3. Data Transformation (Power BI)
- Created calculated columns:
  - Churn Status (0/1)
  - Monthly Charge Range
- Built mapping tables:
  - Age Groups
  - Tenure Groups
- Unpivoted service columns for better analysis

---

### 4. DAX Measures
- Total Customers
- New Joiners
- Total Churn
- Churn Rate %

---

### 5. Dashboard Insights

####  Key KPIs
- Total Customers
- Total Churn
- Churn Rate
- New Joiners

####  Analysis Areas
- Demographics (Age, Gender)
- Account Information (Contract, Payment Method)
- Geography (Top states by churn)
- Services (Internet type, service usage)
- Churn Reasons (with tooltip drill-down)

---

## Key Insights
- Customers with shorter tenure show higher churn rates
- Month-to-month contracts have higher churn compared to long-term contracts
- Certain states contribute disproportionately to churn
- Higher monthly charges correlate with increased churn probability

---
