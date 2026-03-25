# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview

This project focuses on analyzing customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The objective is to uncover actionable insights related to spending patterns, customer segmentation, product preferences, and subscription behavior to support data-driven business decisions.

-----

## 📊 Dataset Summary

Total Rows: 3,900

Total Columns: 18

### 🔑 Key Features:

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Shopping Behavior:

Discount Applied

Promo Code Used

Previous Purchases

Frequency of Purchases

Review Rating

Shipping Type

Missing Values:

37 missing values in Review Rating column

### 🧹 Data Preprocessing & EDA (Python)

✔️ Steps Performed:

Data Loading: Imported dataset using pandas

Initial Exploration: Used .info() and .describe() for structure and statistics

Missing Value Handling:

Imputed missing values in Review Rating using median rating per category

Column Standardization:

Renamed columns to snake_case for consistency

Feature Engineering:

Created age_group using age binning

Generated purchase_frequency_days

Data Consistency Check:

Dropped promo_code_used (redundant with discount_applied)

Database Integration:

Loaded cleaned data into PostgreSQL for SQL analysis

----

## 🧠 Data Analysis (SQL)

Performed business-driven queries in PostgreSQL:

Revenue by Gender – Compared total revenue across genders

High-Spending Discount Users – Customers using discounts but spending above average

Top 5 Products by Rating – Based on average review ratings

Shipping Type Analysis – Standard vs Express purchase comparison

Subscribers vs Non-Subscribers – Revenue & average spend comparison

Discount-Dependent Products – Top 5 products with highest discount usage

Customer Segmentation – Classified into:

New

Returning

Loyal

Top 3 Products per Category

Repeat Buyers vs Subscriptions – Correlation analysis

Revenue by Age Group

----

## 📊 Dashboard (Power BI)

Built an interactive Power BI dashboard to visualize:

Customer segments

Revenue trends

Product performance

Purchase behavior insights

----

## 💡 Business Recommendations

Increase Subscriptions: Offer exclusive benefits

Loyalty Programs: Convert repeat buyers into loyal customers

Optimize Discounts: Maintain balance between sales and profit margins

Product Positioning: Promote high-rated & best-selling products

Targeted Marketing: Focus on high-value customer segments

----

## 🛠️ Tech Stack

Python: Pandas, NumPy

Database: PostgreSQL

Visualization: Power BI

Data Processing: Feature Engineering, EDA

----

## 🚀 Key Outcomes

Identified high-value customer segments

Uncovered product-level insights

Built a scalable pipeline from Python → SQL → BI 

Delivered business-ready recommendations
