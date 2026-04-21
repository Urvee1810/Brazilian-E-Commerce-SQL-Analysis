# 🛒 Brazilian E-Commerce SQL Analysis 

![SQL](https://img.shields.io/badge/SQL-PostgreSQL%20%7C%20MySQL-blue?style=for-the-badge&logo=postgresql)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-Business%20Intelligence-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Dataset: https://www.kaggle.com/datasets/urveeshrivastava/1-brazilian-ecommerce-sql-analysis 

## 📌 Project Overview
This repository contains a comprehensive, **3-tier SQL analysis** of the [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). 

Bypassing standard "follow-along" tutorials, this project was built entirely from scratch to answer real-world business questions. It is structured to demonstrate progressive SQL mastery, moving from foundational data exploration to highly complex, multi-layered business queries.

**The ultimate goal?** To transform raw, disconnected relational data into actionable insights for marketing, logistics, and inventory management.

---

## 🛠️ Tech Stack & Skills Highlighted
- **Database Engine:** SQLite / PostgreSQL (Syntax compatible)
- **Environment:** Jupyter Notebook (`.ipynb`)
- **Tier 1 (Foundations):** `SELECT`, `WHERE`, `LIKE`, `IS NULL`, `GROUP BY`, `ORDER BY`, `COUNT()`, `SUM()`, `AVG()`
- **Tier 2 (Relational Logic):** `INNER JOIN`, `LEFT JOIN`, `HAVING`, Scalar Subqueries, `IN` Subqueries, Date Parsing
- **Tier 3 (Advanced Business Logic):** Common Table Expressions (`CTE`s), Multi-Table Chaining, Window Functions (`RANK()`, `ROW_NUMBER()`, `LEAD()`, `LAG()`), Data Pivoting & Performance Optimization

---

## 📂 Project Structure: The 3 Tiers of Analysis

The analysis is broken down into three distinct tiers of difficulty to simulate real-world data requests:

### 🟢 Tier 1: Data Exploration & Foundations
*Answering immediate, single-table business questions to audit data quality and establish baselines.*
* **The Logistics Audit:** Filtering for recent, successfully delivered orders with non-null delivery dates.
* **The Geo-Targeting Filter:** Pinpointing customers in high-value states (SP, RJ, MG) for localized marketing campaigns using wildcard pattern matching.
* **The Revenue Pulse:** Aggregating total transactions, average ticket sizes, and record-high payments grouped by payment method.
* **The Inventory Check:** Auditing mid-weight inventory categories.

### 🟡 Tier 2: The Relational Sandbox (Medium)
*Connecting the dots across the database schema using relational logic and subqueries.*
* **The Basic Bridge:** Joining orders to payment methods to map the customer transaction journey.
* **The Orphan Hunt:** Identifying discrepancies between datasets (e.g., customers without orders, products without categories) using `LEFT JOIN` and `IS NULL`.
* **The High-Value Filter:** Using `HAVING` and dynamic Scalar Subqueries to identify above-average order values and high-performing cohorts.

### 🔴 Tier 3: Advanced Business Logic (Hard)
*Structuring complex reporting pipelines using CTEs and Window Functions.*
* **Multi-Step Funnel Analysis:** Utilizing CTEs to isolate clean data before running heavy aggregations.
* **Seller Leaderboards:** Using `RANK()` and `DENSE_RANK()` to stack-rank top sellers based on revenue and fulfillment speed.
* **Customer Retention Tracking:** Applying Window Functions like `LAG()` and `LEAD()` to map days between purchases for returning customers.

---

## 📊 Key Business Insights Discovered
*(Highlights from the query results)*

1. **Payment Preferences:** Credit cards dominate total revenue generation, but *Boleto* (invoices) represents a massive chunk of transaction volume, emphasizing the need for flexible payment gateways.
2. **Logistics Bottlenecks:** Analysis of the shipping limit dates vs. actual delivery dates revealed specific seller cohorts consistently missing fulfillment SLAs during peak 2017 months.
3. **Geo-Concentration:** A vast majority of the high-value customers are heavily concentrated in São Paulo ('SP') and Rio de Janeiro ('RJ'), validating a targeted regional ad-spend strategy.

---

## 🚀 How to Run the Code
1. Clone this repository to your local machine.
2. Download the original dataset from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) and place the CSV files in the working directory.
3. Open the `1_Brazilian_ECommerce_SQL_Analysis.ipynb` notebook.
4. Run the setup cells to load the CSVs into a local in-memory SQL database (using `sqlite3` and `pandas`).
5. Execute the query blocks progressively from Tier 1 to Tier 3.

---

## 🏆 Background: The 90-Hour SQL Sprint
This project is the capstone achievement of my **90-Hour SQL Mastery Sprint**. Over the course of 14 days, I treated my technical upskilling as a "study debt," drilling multi-table Joins, CTEs, and Window Functions, and solving over 150+ medium-to-hard SQL interview questions before building this end-to-end analysis.

**Status:** Open for Technical Data Analyst & Data Scientist roles! Let's talk data. 
