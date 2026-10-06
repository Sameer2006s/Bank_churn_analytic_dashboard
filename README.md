# 🏦 Bank Customer Churn Analysis — Power BI

An interactive Power BI project focused on analyzing customer churn and identifying customer segments that are more likely to leave a bank.

The dashboard explores customer demographics, financial characteristics, account activity, and banking behavior to understand the major patterns behind customer churn.

---

## 📌 Project Overview

Customer churn is an important challenge for banks because losing existing customers can directly impact revenue and long-term growth.

In this project, I analyzed **10,000 customer records** and created a **3-page interactive Power BI dashboard** to understand churn patterns and generate business-focused insights.

The project includes data transformation, calculated columns, DAX measures, data modeling, visualization, and customer segmentation.

---

## 🎯 Objectives

- Analyze the overall customer churn rate
- Identify customer segments with higher churn
- Understand churn patterns across demographics
- Analyze financial and account-related factors
- Compare churn across different customer segments
- Create meaningful KPIs using DAX
- Provide recommendations that can support customer retention

---

## 📊 Dashboard

### 1️⃣ Customer Churn Overview

This page provides a high-level view of customer churn.

**Key KPIs:**
- Total Customers: **10K**
- Active Customers: **7.963K**
- Churned Customers: **2.037K**
- Average Credit Score: **650.5**
- Churn Rate: **20.37%**

**Analysis includes:**
- Churned Customers by Country
- Churned Customers by Gender
- Churned Customers by Member Status
- Churned Customers by Age Group
- Churned Customers by Credit Card Status
- Churned Customers by Number of Bank Products

---

### 2️⃣ Churn & Customer Risk Analysis

This page focuses on financial and account-related factors associated with customer churn.

**Analysis includes:**
- Churned Customers by Balance Group
- Churn Rate by Credit Score Group
- Churned Customers by Tenure Group
- Churned Customers by Salary Group

These segments help identify customer groups that may require closer monitoring.

---

### 3️⃣ Key Insights & Retention Recommendations

The final page summarizes the major findings from the analysis and converts them into business recommendations.

**Key areas:**
- High-risk customer segments
- Inactive customer behavior
- Age-related churn patterns
- Bank product usage
- High-value customers
- Geographic churn patterns
- Customer retention strategies

---

## 🧮 Calculated Columns

Created multiple calculated columns in Power BI to make the raw data easier to analyze:

- **Age Group**
- **Balance Group**
- **Credit Score Group**
- **Tenure Group**
- **Salary Group**
- **Credit Card Status**
- **Active/Inactive Member Status**

These columns were used for customer segmentation and dashboard analysis.

---

## 📐 DAX Measures

Created DAX measures for dynamic KPI calculations, including:

- Total Customers
- Active Customers
- Churned Customers
- Churn Rate (%)
- Average Credit Score

Example:

```DAX
Churn Rate =
DIVIDE(
    SUM('Bank Customer Churn'[churn]),
    COUNTROWS('Bank Customer Churn),
    0
)
