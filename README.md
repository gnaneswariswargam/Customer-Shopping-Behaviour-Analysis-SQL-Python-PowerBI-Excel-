# Customer-Shopping-Behaviour-Analysis-SQL-Python-PowerBI-Excel-
🛒 Customer Shopping Behavior Analysis

Tools Used: Excel | SQL (PostgreSQL) | Python (Pandas, Matplotlib, Seaborn) | Power BI
Duration: September 2025

📘 Project Overview

This project focuses on understanding customer shopping behavior through data-driven insights. Using a dataset of 3,900+ retail transactions, the analysis explores how demographic and behavioral factors—like gender, age, subscription, and discounts—influence spending patterns and product preferences.

The goal was to derive business strategies to improve customer retention and profitability through loyalty programs, targeted campaigns, and subscription offers.

📊 Objectives

Clean and preprocess raw retail transaction data for accurate analysis.

Perform exploratory data analysis (EDA) to uncover trends in customer spending.

Use SQL for revenue and segmentation analysis.

Visualize insights and KPIs using Power BI dashboards.

Recommend actionable strategies to boost profitability and engagement.

🧹 Data Cleaning & Preprocessing

Cleaned 3,900+ rows with 18 features (age, gender, product category, discount, subscription, etc.).

Handled missing values using median imputation for numerical fields.

Standardized data formats and removed duplicates to ensure consistency.

Verified data accuracy using Excel pivot summaries.

🧠 Exploratory Data Analysis (EDA)

Performed in Python using Pandas, Matplotlib, and Seaborn:

Identified high-spending customer segments and loyalty-driven buyers.

Discovered that discount-sensitive customers contribute significantly to revenue.

Found that subscribed customers spend on average 30% more than non-subscribed ones.

Analyzed spend trends by gender and age group.

🗃️ SQL Analysis (PostgreSQL)

Key SQL insights include:

-- Revenue by gender
SELECT gender, SUM(total_amount) AS total_revenue
FROM transactions
GROUP BY gender;

-- Revenue by subscription status
SELECT subscription_status, SUM(total_amount) AS total_revenue
FROM transactions
GROUP BY subscription_status;

-- Age group segmentation
SELECT
  CASE
    WHEN age BETWEEN 18 AND 25 THEN '18-25'
    WHEN age BETWEEN 26 AND 35 THEN '26-35'
    WHEN age BETWEEN 36 AND 45 THEN '36-45'
    ELSE '46+'
  END AS age_group,
  SUM(total_amount) AS total_revenue
FROM transactions
GROUP BY age_group;

📈 Power BI Dashboard

Built an interactive Power BI dashboard showcasing:

Total Revenue & Average Spend per Customer

Customer Segmentation by Gender, Age, and Subscription

Discount vs Revenue Trend

Loyalty-based Buying Patterns

The dashboard allows decision-makers to filter by demographics and identify profitable customer groups for targeted marketing.

💡 Key Insights

Loyalty programs can enhance retention of high-value customers.

Targeted campaigns for discount and subscription users can increase engagement.

Implementing these strategies could potentially improve profitability by 25%.
