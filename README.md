# Customer-Trends-Data-Analysis
Customer Trends Data Analysis using postgreSQL, python and powerBI 

Copy everything inside this box directly into your GitHub `README.md`:

````markdown
# Customer Shopping Behavior Analysis

### 🛠️ Tools Used

**Python** • **Pandas** • **PostgreSQL** • **SQL** • **Power BI** • **GitHub**

---

## 1. Executive Summary

This project analyzes customer shopping behavior using a dataset of **3,900 purchase transactions across 18 features**. The objective is to identify purchasing patterns, customer segments, product preferences, discount behavior, subscription trends, and revenue drivers.

The project follows an end-to-end data analytics workflow:

**Python → PostgreSQL/SQL → Power BI → Business Recommendations**

The analysis provides insights that can help the retail company improve customer engagement, strengthen customer loyalty, optimize promotions, and make more data-driven marketing and product decisions.

---

## 2. Business Problem

A leading retail company wants to better understand its customers' shopping behavior in order to improve sales, customer satisfaction, and long-term loyalty.

Management has observed changes in purchasing patterns across different demographics, product categories, and customer behaviors. The company is particularly interested in understanding factors such as discounts, product reviews, purchase frequency, subscription status, and shipping preferences.

### Business Question

> **How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

### Key Questions

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

### Data Preparation & Cleaning — Python

Python was used to clean, transform, and prepare the raw dataset for analysis.

Key steps included:

- Loading the dataset using Pandas
- Exploring the dataset using `df.info()` and `df.describe()`
- Checking for missing values
- Handling 37 missing values in `Review Rating`
- Imputing missing review ratings using the median rating of each product category
- Standardizing column names using snake_case
- Creating an `age_group` feature
- Creating a `purchase_frequency_days` feature
- Checking for redundancy between `discount_applied` and `promo_code_used`
- Removing the redundant `promo_code_used` column

The cleaned dataset was then connected to PostgreSQL for further analysis.

### SQL Analysis — PostgreSQL

SQL was used to perform structured business analysis on the cleaned dataset.

The analysis included:

- Revenue by gender
- High-spending discount users
- Top-rated products
- Shipping type comparison
- Subscriber vs. non-subscriber spending
- Discount-dependent products
- Customer segmentation
- Top 3 products within each category
- Repeat buyers and subscription behavior
- Revenue by age group

### Data Visualization — Power BI

The results were presented through an interactive Power BI dashboard to make the findings easier for stakeholders to understand and explore.

The dashboard visualizes:

- Customer behavior
- Revenue performance
- Customer segments
- Product performance
- Subscription behavior
- Discount usage
- Age-group revenue
- Shipping behavior

### Project Workflow

```text
Raw Dataset
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
Insights & Recommendations
````

---

## 4. Skills

### Data Analysis

* Python
* Pandas
* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering

### Database & SQL

* PostgreSQL
* SQL
* CTEs
* Subqueries
* Window Functions
* Data Aggregation
* Customer Segmentation

### Data Visualization

* Power BI
* Interactive Dashboards
* Data Visualization
* Data Storytelling

### Business Analytics

* Customer Behavior Analysis
* Revenue Analysis
* Product Analysis
* Customer Segmentation
* Business Problem Solving
* Data-Driven Decision Making

---

## 5. Results & Business Recommendations

### Customer Loyalty

Customers were segmented into **New, Returning, and Loyal** groups based on their purchase history.

**Recommendation:**
Develop loyalty programs that reward repeat customers and encourage Returning customers to become Loyal customers through points, exclusive rewards, and repeat-purchase incentives.

### Subscription Strategy

The analysis compared purchasing behavior between subscribers and non-subscribers and examined the relationship between repeat purchases and subscription status.

**Recommendation:**
Introduce exclusive subscriber benefits such as member-only discounts, loyalty rewards, and shipping benefits to encourage high-value customers to subscribe.

### Discount Strategy

The analysis identified products with a high percentage of discounted purchases.

**Recommendation:**
Review the discount strategy for highly discount-dependent products to ensure promotions increase sales without unnecessarily reducing profit margins.

### Product Performance

Top-rated and most frequently purchased products were identified through SQL analysis.

**Recommendation:**
Feature highly rated and best-selling products more prominently in marketing campaigns, product recommendations, and promotional activities.

### Targeted Marketing

Revenue was analyzed across different customer age groups.

**Recommendation:**
Focus marketing efforts on high-revenue age groups and tailor campaigns according to their purchasing behavior and preferences.

### Shipping Preferences

The analysis compares purchasing behavior between Standard and Express shipping customers.

**Recommendation:**
Use shipping preferences as an additional customer segmentation factor and consider premium shipping benefits as part of subscription or loyalty programs.

---

## 6. Next Steps

### Predictive Analytics

Future versions of the project could use machine learning to predict:

* Customer churn
* Subscription likelihood
* Future purchasing behavior
* Customer lifetime value

### Personalized Product Recommendations

A recommendation system could be developed to suggest products based on:

* Previous purchases
* Product categories
* Purchase frequency
* Customer preferences

### Advanced Power BI Dashboard

The dashboard could be expanded with:

* Customer-level filtering
* Interactive customer segmentation
* Product performance drill-downs
* Time-based purchasing trends
* Additional KPIs
* Profitability analysis

### Profitability Analysis

Future analysis could incorporate product cost and profit-margin data to evaluate whether discounts and promotions are generating profitable growth.

---

## 7. GitHub Repository

### Project Structure

```text
customer-shopping-behavior-analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── python/
│   └── data_cleaning.py
│
├── sql/
│   └── customer_behavior_sql_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── Customer_Shopping_Behavior_Analysis.pdf
│
└── README.md
```

---

### Project Outcome

This project demonstrates an end-to-end approach to transforming raw customer transaction data into actionable business insights.

By combining **Python, SQL, PostgreSQL, and Power BI**, the project provides a data-driven view of customer behavior and identifies opportunities to improve **customer engagement, sales performance, marketing strategies, and long-term customer loyalty**.

```
```
