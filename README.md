**Customer Shopping Behavior Analysis
This project examines how customers shop across different product categories using a dataset of 3,900 transactions. The goal was to understand spending patterns, customer types, product performance, and subscription behavior so that a business could make more informed decisions on marketing, loyalty, and product strategy.

**Project Overview
The analysis combines three layers of work:
Data preparation and exploratory analysis in Python
Business-focused SQL analysis in PostgreSQL
An interactive Power BI dashboard to present findings
The workflow reflects how an end-to-end analytics project is carried out in a real environment, from raw data to insights that support decision-making.

**Dataset Summary
Total rows: 3,900
Columns: 18
Includes customer demographics, purchase details, behavioral indicators, and product attributes
Missing data: 37 null values in the Review Rating column, handled during cleaning
Key fields include age, gender, subscription status, item purchased, category, amount spent, discount usage, shipping type, and previous purchase indicators.

**Data Preparation and Exploration (Python)

Work in Python focused on ensuring the dataset was reliable, consistent, and ready for deeper analysis.
Initial steps:
Loaded data with pandas
Reviewed structure using info() and describe()
Explored distributions and basic statistics
Cleaning and transformations:
Imputed missing review ratings using the median rating within each product category
Standardized all column names to snake_case
Created new features, including
age_group (binned ranges)
purchase_frequency_days (derived from purchase history)
Removed the promo_code_used column after confirming it overlapped with discount indicators
Database integration:
Connected Python to PostgreSQL and wrote the cleaned dataset into the database for SQL-based analysis.

**Business Analysis Using SQL

SQL queries were used to answer structured questions about customer behavior, product performance, and revenue drivers.
Examples of the analyses performed include:
Comparing total revenue between male and female customers
Identifying customers who used discounts but still spent above the average purchase amount
Listing top-rated products based on average review rating
Comparing average purchase amounts across different shipping types
Analyzing spending patterns of subscribers vs. non-subscribers
Finding products that depend heavily on discounts
Segmenting customers into new, returning, and loyal groups
Identifying the top three most-purchased products within each category
Testing whether customers with more than five purchases are more likely to subscribe
Calculating revenue contributions by age group
This section of the project demonstrates applied SQL for behavioral analytics, segmentation, and revenue modeling.

**Power BI Dashboard

The Power BI dashboard brings the analysis together visually.
It summarizes patterns in revenue, customer groups, purchase behavior, product categories, and subscription metrics.
This makes the insights easier for non-technical stakeholders to understand and act upon.
![Screenshot 2025-12-16 220338](https://github.com/user-attachments/assets/bec3fa0d-90ec-49cd-a49e-2ff1ea704852)



**Key Business Recommendations

Based on the combined insights from Python, SQL, and Power BI:
Strengthen subscription programs by emphasizing member-only benefits
Introduce or enhance loyalty programs to encourage repeat purchasing
Reevaluate discount strategy to reduce unnecessary margin loss
Highlight top-performing and top-rated products in marketing efforts
Target marketing and promotional campaigns toward high-revenue age groups and express-shipping customers

**Technologies Used
Python (pandas, numpy, matplotlib)
PostgreSQL
SQLAlchemy (for Python-to-database integration)
Power BI

**Why This Project Matters

This project reflects an end-to-end analytics workflow: cleaning and transforming data, performing business-oriented SQL analysis, and presenting insights in a dashboard that supports decision-making.
It demonstrates practical skills in data quality improvement, feature engineering, querying, and storytelling with data—all essential in real-world analyst roles.
