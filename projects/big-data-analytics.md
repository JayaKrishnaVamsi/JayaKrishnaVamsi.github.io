---
layout: default
title: Indian Personal Finance & Spending Habits
permalink: /projects/big-data-analytics/
---

# Indian Personal Finance & Spending Habits

## 📌 Project Overview
This project was carried out as part of the **Big Data Analytics** course during my MBA in Business Analytics. The main goal was to analyze the spending, saving, and financial behaviour of **20,000 individuals** using large-scale distributed data processing tools.

By leveraging the **Hadoop ecosystem** (HDFS, Hive, Pig, MapReduce, Sqoop) along with **PySpark MLlib**, we built an end-to-end pipeline for **data preprocessing, analytics, machine learning, and recommendations**.

---

## 🎯 Objectives
- Understand **spending patterns** across different city tiers and occupations.  
- Identify categories with the **highest potential savings**.  
- Predict **disposable income** using machine learning models.  
- Build a **rule-based financial recommendation system**.  

---

## 📂 Dataset
The dataset contained demographic, financial, and behavioral attributes such as:
- **Demographics**: Age, Income, Dependents, Occupation, City Tier  
- **Expenses**: Rent, Groceries, Utilities, Transport, Education, Entertainment, etc.  
- **Savings**: Desired savings percentage, disposable income, expense ratios  
- **Derived Features**: Essential vs. discretionary spending, savings gap, potential savings  

---

## ⚙️ Tools & Technologies
- **HDFS (Hadoop Distributed File System)** for distributed storage  
- **Hive & Pig** for SQL-like queries and data aggregation  
- **MapReduce** for custom distributed computations  
- **PySpark (MLlib)** for machine learning (linear regression for disposable income prediction)  
- **Sqoop** for integrating Hadoop outputs with MySQL  
- **Recommendation System** built using RDDs in Spark  

---

## 📊 Key Insights
- **City-wise**:  
  - Tier 3 cities surprisingly showed the **highest average disposable income**, due to lower cost of living.  
  - Tier 1 cities had the **highest expense ratio**, reflecting lifestyle-driven spending.  

- **Spending Behaviour**:  
  - Groceries, Transport, and Utilities showed the **highest savings potential**.  
  - Tier 1 users spent more on **Education**, while Tier 2 and 3 showed high **miscellaneous expenses**.  

- **Financial Stress**:  
  - 18.6% of Tier 1 users were “high spenders” (spending >90% of income).  
  - All city tiers showed a **negative savings gap**, meaning actual savings fell short of targets.  

- **Occupational Trends**:  
  - Professionals dominated across all city tiers.  
  - Students and retirees showed lower expense ratios compared to professionals.  

---

## 🤖 Machine Learning
- Built a **PySpark Linear Regression model** to predict **disposable income**.  
- Achieved reasonable accuracy measured by **RMSE** and **R²** metrics.  
- Exported predictions into MySQL for use in **dashboards (Tableau/Power BI)**.  

---

## 💡 Recommendation System
- Implemented using **Spark RDDs** with rule-based logic.  
- Generated personalized advice like:  
  - “Cut discretionary expenses”  
  - “Consider financial planning”  
  - “Reduce lifestyle spending”  

---

## 📈 Real-World Relevance
The project demonstrates how **Big Data tools** can drive **financial intelligence**:
- Helps **banks and fintechs** design better financial products.  
- Enables **governments** to target financial literacy programs.  
- Provides **individuals** with actionable advice for saving and planning.  

---

