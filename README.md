# 📊 Customer Churn Analysis Dashboard | Power BI

## 📌 Project Overview

This Power BI dashboard analyzes customer churn data to identify the main factors influencing customer attrition. It provides interactive insights into customer demographics, contract types, service usage, charges, and churn reasons, helping businesses understand why customers leave and where retention efforts should be focused.

<img width="1266" height="692" alt="Screenshot 2026-07-31 144827" src="https://github.com/user-attachments/assets/659d6bb2-262a-4701-bc3f-e773920aef24" />


## 🎯 Objectives

- Analyze customer churn behavior.
- Calculate the churn rate.
- Identify the most common churn reasons.
- Compare churn across customer demographics.
- Discover the impact of contracts, age, customer service calls, and monthly charges on churn.
- Build an interactive dashboard for business decision-making.

---

## 🛠️ Tools Used

- Power BI Desktop
- Power Query
- DAX
- Excel Dataset

---

## 📂 Data Preparation

The dataset was cleaned and prepared before visualization by:

- Checking data types.
- Creating calculated columns.
- Creating DAX measures.
- Formatting numeric fields.
- Building business KPIs.

---

## 📐 DAX Measures

The project includes several custom measures, including:

```DAX
Total Customer =
COUNT(Data[Customer ID])

True Churned =
SUM(Data[Churned])

Churn Rate =
DIVIDE([True Churned],[Total Customer])

Average Age =
AVERAGE(Data[Age])

Total Charge =
SUM(Data[Total Charges])
```

---

## 🧮 Calculated Columns

Examples include:

```DAX
Churned =
IF(Data[Churn Label]="Yes",1,0)

Contract Category =
SWITCH(
Data[Contract Type],
"One Year","Yearly",
"Two Year","Yearly",
"Month-to-Month","Monthly"
)
```

---

## 📈 Dashboard Features

The dashboard provides:

- Total Customers KPI
- Total Churned Customers KPI
- Churn Rate KPI
- Average Customer Age
- Total Revenue
- Top 10 Churn Reasons
- Churn Distribution by Category
- Geographic Analysis by State
- Churn Rate by Customer Service Calls
- Monthly Charge Analysis
- Age Distribution Analysis
- Contract Type Analysis
- Gender Comparison
- Interactive Filters

---

## 📊 Key Insights

- Month-to-month contracts have the highest churn rate.
- Competitor-related reasons represent the largest percentage of customer churn.
- Customers with more service calls are significantly more likely to churn.
- Older customers tend to have higher churn rates in some age groups.
- Churn varies noticeably across different states.

---

## 📷 Dashboard Preview

> Dashboard screenshot

<img src="Dashboard.png" width="100%">

---

## 📁 Project Structure

```
Customer-Churn-Dashboard
│
├── Customer Churn.pbix
├── Customer Churn.xlsx
├── Dashboard.png
└── README.md
```

---

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Modeling
- DAX
- Calculated Columns
- Measures
- KPI Design
- Interactive Dashboard Development
- Business Intelligence
- Data Visualization
- Customer Churn Analysis

---

## 📬 Contact

If you have any feedback or suggestions, feel free to connect with me on GitHub.

