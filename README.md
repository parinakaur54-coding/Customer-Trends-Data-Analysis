# 🛍️ Customer Shopping Behavior Analysis

### 🛠️ Tools Used
**Python** • **Pandas** • **PostgreSQL** • **SQL** • **Power BI** • **GitHub**

---

## 1. Executive Summary

This project analyzes customer shopping behavior using a dataset containing **3,900 purchase transactions and 18 features**.

The objective is to transform raw customer data into actionable business insights that can help a retail company improve **sales, customer engagement, customer satisfaction, and long-term loyalty**.

The project follows an end-to-end data analytics workflow:

**Python → PostgreSQL → SQL Analysis → Power BI → Business Recommendations**

The analysis focuses on customer demographics, purchasing behavior, product categories, customer reviews, discounts, subscription status, shipping preferences, customer loyalty, and revenue contribution.

---

## 2. Business Problem

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

## 3. Methodology

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
- Top-rated products
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

The cleaned and analyzed data was visualized through an interactive Power BI dashboard.

The dashboard includes:

- **Number of Customers** KPI
- **Average Purchase Amount** KPI
- **Average Review Rating** KPI
- Customer subscription status
- Sales by product category
- Revenue by product category
- Sales by age group
- Revenue by age group
- Subscription status analysis

Interactive filters allow users to explore the data by:

- Subscription Status
- Gender
- Category
- Shipping Type

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

---

## 4. Skills

### Data Analysis

- Python
- Pandas
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering

### SQL & Database

- PostgreSQL
- SQL
- Common Table Expressions (CTEs)
- Subqueries
- Window Functions
- Data Aggregation
- Customer Segmentation

### Data Visualization

- Power BI
- Interactive Dashboards
- Data Visualization
- Data Storytelling

### Business Analytics

- Customer Behavior Analysis
- Revenue Analysis
- Product Analysis
- Customer Segmentation
- Business Problem Solving
- Data-Driven Decision Making

---

## 5. Results & Business Recommendations

### 👥 Customer Loyalty

Customers were segmented into **New, Returning, and Loyal** groups based on their purchase history.

**Recommendation:**

Develop loyalty programs that reward repeat customers and encourage Returning customers to become Loyal customers through points, exclusive rewards, and repeat-purchase incentives.

### ⭐ Subscription Strategy

The dashboard provides a breakdown of customers based on their subscription status, allowing the company to compare subscriber and non-subscriber behavior.

The SQL analysis also examines whether customers with more than five purchases are more likely to subscribe.

**Recommendation:**

Introduce exclusive subscriber benefits such as member-only discounts, loyalty rewards, and shipping benefits to encourage high-value customers to subscribe.

### 🏷️ Discount Strategy

The analysis identifies products with a high percentage of discounted purchases and examines customers who use discounts while still spending above the average purchase amount.

**Recommendation:**

Review the discount strategy for highly discount-dependent products to ensure promotions increase sales without unnecessarily reducing profit margins.

### 🛍️ Product & Category Performance

Sales and revenue were analyzed across different product categories through the Power BI dashboard.

Top-rated and most frequently purchased products were also identified through SQL analysis.

**Recommendation:**

Feature high-performing and highly rated products more prominently in marketing campaigns, product recommendations, and promotional activities.

### 🎯 Customer Demographics

The dashboard provides both **sales and revenue analysis by age group**, helping identify differences in purchasing behavior and revenue contribution across customer segments.

**Recommendation:**

Focus marketing efforts on high-revenue age groups and tailor campaigns according to their purchasing behavior and preferences.

### 🚚 Shipping Preferences

Shipping type was analyzed using SQL and incorporated as an interactive dashboard filter.

**Recommendation:**

Use shipping preferences as an additional customer segmentation factor and consider premium shipping benefits as part of subscription or loyalty programs.

---

## 6. Next Steps

### 🤖 Predictive Analytics

Future versions of the project could incorporate machine learning models to predict:

- Customer churn
- Subscription likelihood
- Future purchasing behavior
- Customer lifetime value

### 🎯 Personalized Product Recommendations

A recommendation system could be developed to suggest products based on:

- Previous purchases
- Product categories
- Purchase frequency
- Customer preferences

### 📊 Advanced Power BI Dashboard

The dashboard could be expanded with:

- Customer-level filtering
- Interactive customer segmentation
- Product performance drill-downs
- Time-based purchasing trends
- Additional KPIs
- Profitability analysis
