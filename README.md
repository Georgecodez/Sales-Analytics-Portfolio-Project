# Sales-Analytics-Portfolio-Project
## Project Overview 
This project conducts a detailed analysis of a sales database to unravel valuable insights about products, customers, and overall business performance. We leverage SQL to explore, aggregate and segment data from multiple dimensions such as demographics, product categories, and purchasing behavior. The outcome depicts detailed and actionable reports that could aid strategic decision-making. 
## Objectives
The objectives that guided the project are as follows:

i.	Generate key business metrics such as total sales, revenue, average price, etc. to evaluate overall business performance. 

ii.	Classify customers into VIP, Regular, and New segments based on lifetime value and activity span to enable targeted engagement strategies.

iii.	Rank products based on sales volume and revenue to identify the high performers, mid-range, and underperformers as well as revenue drivers across categories.

iv.	Perform time-based trend analysis to track sales, customer growth, and order activity across monthly and yearly timeframes to unravel seasonality and long-term trends. 

v.	Develop reusable SQL views summarizing key KPIs like recency, average monthly spend, product lifespan, and order frequency for reporting. 

## Project Structure 
### Database and Dimensions exploration: 
Step 1: Database Exploration 
Explore all objects in the database 

```sql

SELECT*
FROM INFORMATION_SCHEMA.TABLES

```
SELECT*
FROM INFORMATION_SCHEMA.TABLES
--Explore all columns in the database 
SELECT*
FROM INFORMATION_SCHEMA.columns 
WHERE table_name = 'dim_products'
Step 2: Dimensions exploration 
Explore all countries our customers came from 
SELECT DISTINCT country 
FROM dbo.[gold.dim_customers]
Explore all product and subcategories (Major divisions). 
SELECT DISTINCT category, subcategory, product_name 
FROM dbo.[gold.dim_products]


