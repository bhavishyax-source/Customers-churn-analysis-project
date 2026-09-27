# Customers-churn-analysis-project
End-to-end Customer Churn Analysis using Excel, Python, Pandas, NumPy, SQL Server, and Power BI to identify churn patterns and generate actionable business insights.

# Customer Churn Analysis 📊

## 📌 Project Overview

This project analyzes customer churn data to identify the key factors associated with customer attrition and uncover actionable business insights.

The project follows a complete end-to-end Data Analyst workflow, starting with raw and unclean data and progressing through data cleaning, feature engineering, SQL analysis, and Power BI visualization.

The objective is to answer an important business question:

> **Why are customers leaving, and which customer segments are most likely to churn?**

---

## 🎯 Business Objectives

The analysis aims to:

* Calculate the overall customer churn rate
* Identify customer segments with high churn
* Analyze churn by contract type
* Analyze churn by tenure
* Analyze churn by payment method
* Investigate the relationship between charges and churn
* Identify important customer characteristics associated with churn
* Calculate potential revenue impact from churn
* Provide actionable recommendations for customer retention

---

## 🛠️ Tools & Technologies

* **Excel** – Initial data exploration and validation
* **Python** – Data cleaning and analysis
* **Pandas** – Data manipulation and transformation
* **NumPy** – Numerical calculations
* **MS SQL Server** – Database storage and SQL analysis
* **SQL** – Business analysis and aggregations
* **Power BI** – Interactive dashboard and visualization
* **GitHub** – Project documentation and version control

---

## 🔄 Project Workflow

```text
Raw Customer Churn Data
          ↓
Excel - Initial Exploration
          ↓
Python / Pandas
          ↓
Data Cleaning
          ↓
Feature Engineering
          ↓
Clean Dataset
          ↓
MS SQL Server
          ↓
SQL Business Analysis
          ↓
Power BI Dashboard
          ↓
Business Insights & Recommendations
```

---

## 📂 Project Structure

```text
Customer-Churn-Analysis/
│
├── data/
│   ├── raw_customer_churn.xlsx
│   └── clean_customer_churn.csv
│
├── excel/
│   └── initial_exploration.xlsx
│
├── python/
│   └── customer_churn_analysis.ipynb
│
├── sql/
│   └── churn_analysis.sql
│
├── powerbi/
│   └── customer_churn_dashboard.pbix
│
├── screenshots/
│   └── dashboard.png
│
├── README.md
└── requirements.txt
```

---

## 1️⃣ Excel - Initial Data Exploration

The raw dataset was first examined in Excel to understand its structure and identify potential data-quality issues.

The initial inspection included:

* Number of rows and columns
* Column names
* Missing values
* Duplicate records
* Data consistency
* Unusual values
* Basic customer and churn distributions

Excel was used for initial investigation rather than performing the complete cleaning process.

---

## 2️⃣ Python - Data Cleaning

Python was used to perform the main data-cleaning process.

### Cleaning steps included:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing categorical values
* Checking invalid values
* Investigating potential outliers
* Validating numerical columns

Main libraries:

```python
import pandas as pd
import numpy as np
```

---

## 3️⃣ Feature Engineering

New analytical features were created to make the dataset more useful for business analysis.

Potential engineered features include:

* Tenure Group
* Age Group
* Annual Charges
* Service Count
* Revenue-related metrics

Example:

```python
df["AnnualCharges"] = df["MonthlyCharges"] * 12
```

The final features used in the project are documented in the Python notebook.

---

## 4️⃣ Clean Dataset

After cleaning and feature engineering, the processed dataset was exported for further analysis.

```python
df.to_csv("clean_customer_churn.csv", index=False)
```

The cleaned dataset was then imported into MS SQL Server.

---

## 5️⃣ MS SQL Server

The cleaned customer data was stored in a SQL Server database.

SQL was used to perform business-focused analysis, including:

* Total customer count
* Churned customer count
* Churn rate
* Churn by contract
* Churn by tenure
* Churn by payment method
* Average monthly charges
* Revenue associated with churned customers
* Customer segment analysis

Example:

```sql
SELECT
    Churn,
    COUNT(*) AS Customers
FROM CustomerChurn
GROUP BY Churn;
```

---

## 6️⃣ Power BI Dashboard

Power BI was used to create an interactive customer churn dashboard.

### Dashboard KPIs

* Total Customers
* Churned Customers
* Churn Rate
* Monthly Revenue
* Revenue Lost

### Dashboard Analysis

The dashboard analyzes:

* Churn by contract type
* Churn by tenure
* Churn by payment method
* Churn by customer segment
* Churn by monthly charges
* Service usage and churn

### Dashboard Preview

*Add Power BI screenshot here.*

---

## 📈 Key Insights

The final insights will be added after completing the analysis.

Examples of questions investigated:

1. Which customer segment has the highest churn?
2. Which contract type has the highest churn rate?
3. Does customer tenure affect churn?
4. Does monthly spending correlate with churn?
5. Which payment methods are associated with higher churn?
6. How much revenue is potentially lost due to churn?

> **Note:** Insights will be based on the actual analysis rather than assumptions.

---

## 💡 Business Recommendations

Based on the final analysis, recommendations will focus on:

* Improving retention of high-risk customer segments
* Encouraging longer-term contracts
* Improving early-stage customer engagement
* Identifying customers with unusually high churn risk
* Improving customer support and service adoption
* Developing targeted retention strategies

Recommendations will be supported by the analysis and dashboard findings.

---

## 🧠 Skills Demonstrated

This project demonstrates practical experience with:

* Data Cleaning
* Exploratory Data Analysis
* Excel
* Python
* Pandas
* NumPy
* Feature Engineering
* SQL Server
* SQL
* Data Visualization
* Power BI
* Business Intelligence
* Business Problem Solving
* GitHub Documentation

---

## 👤 Author

**Gopal**

Data Analyst focused on Python, SQL, Excel, Power BI and Business Analytics.

The project is currently being developed from raw data through the complete data analytics pipeline.
