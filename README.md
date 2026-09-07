# 🛍️ Customer Shopping Behavior Analysis

### 🛠️ Tools Used
**Python** • **Pandas** • **PostgreSQL** • **SQL** • **Power BI** • **GitHub**

---

## 1. Title

### Customer Shopping Behavior Analysis

An end-to-end data analytics project analyzing customer shopping behavior to uncover purchasing patterns, customer segments, product preferences, discount behavior, subscription trends, and revenue drivers.

---

## 2. Executive Summary

This project analyzes customer shopping behavior using a dataset containing **3,900 purchase transactions and 18 features**.

The goal is to transform raw customer data into actionable business insights that can help a retail company improve **sales, customer engagement, customer satisfaction, and long-term loyalty**.

The project follows an end-to-end data analytics workflow:

**Python → PostgreSQL → SQL Analysis → Power BI → Business Recommendations**

The analysis focuses on customer demographics, purchasing behavior, product performance, discounts, customer loyalty, subscription behavior, shipping preferences, and revenue contribution.

---

## 3. Business Problem

A leading retail company wants to better understand its customers' shopping behavior in order to improve sales, customer satisfaction, and long-term loyalty.

Management has noticed changes in purchasing patterns across different demographics, product categories, and customer behaviors. The company is particularly interested in understanding factors such as **discounts, product reviews, purchase frequency, subscription status, and shipping preferences**.

### Business Question

> **How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

### Key Business Questions

- Which gender generates more revenue?
- Which customers use discounts but still spend above average?
- Which products receive the highest customer ratings?
- Do Express shipping customers spend more than Standard shipping customers?
- Do subscribers generate more revenue than non-subscribers?
- Which products are most dependent on discounts?
- How are customers distributed across New, Returning, and Loyal segments?
- What are the top 3 most purchased products within each category?
- Are customers with more than 5 purchases more likely to subscribe?
- Which age groups contribute the most revenue?

---

## 4. Methodology

### 🐍 Data Preparation & Cleaning — Python

Python and Pandas were used to clean, transform, and prepare the raw dataset for analysis.

Key steps included:

- Loading the dataset using Pandas
- Exploring the dataset using `df.info()` and `df.describe()`
- Checking for missing values
- Handling **37 missing values** in the `Review Rating` column
- Imputing missing review ratings using the median rating of each product category
- Standardizing column names using `snake_case`
- Creating an `age_group` feature
- Creating a `purchase_frequency_days` feature
- Checking the relationship between `discount_applied` and `promo_code_used`
- Removing the redundant `promo_code_used` column
- Loading the cleaned dataset into PostgreSQL

### 🗄️ SQL Analysis — PostgreSQL

PostgreSQL was used to store and analyze the cleaned dataset.

SQL queries were developed to investigate:

- Revenue by gender
- High-spending discount users
- Top 5 products by rating
- Shipping type comparison
- Subscribers vs. non-subscribers
- Discount-dependent products
- Customer segmentation
- Top 3 products within each category
- Repeat buyers and subscription behavior
- Revenue by age group

SQL techniques used include:

- `GROUP BY`
- `ORDER BY`
- `SUM()`
- `AVG()`
- `COUNT()`
- `CASE`
- Subqueries
- Common Table Expressions (CTEs)
- Window Functions
- `ROW_NUMBER()`
- `PARTITION BY`

### 📊 Data Visualization — Power BI

An interactive Power BI dashboard was created to communicate the analysis and make the results easier for business stakeholders to understand.

The dashboard highlights:

- Customer behavior
- Revenue performance
- Customer segments
- Product performance
- Subscription behavior
- Discount usage
- Age-group revenue
- Shipping behavior

### 🔄 Project Workflow

```text
Raw Customer Data
        ↓
Python Data Cleaning
        ↓
Feature Engineering
        ↓
PostgreSQL Database
        ↓
SQL Business Analysis
        ↓
Power BI Dashboard
        ↓
Business Insights
        ↓
Recommendations
