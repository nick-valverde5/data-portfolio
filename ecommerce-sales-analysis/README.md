# Ecommerce Sales Analysis

## Overview
This project analyzes ecommerce sales performance to identify revenue trends, top-performing products, regional sales performance, and business opportunities. The goal of this analysis was to transform raw sales data into actionable insights that support strategic business decision-making.

## Business Problem
Ecommerce businesses rely heavily on sales performance data to optimize profitability, improve product strategy, and identify high-performing regions. This project focuses on uncovering key revenue drivers and operational insights using SQL, Python, and Tableau.

## Tools Used
- SQL
- Python (Pandas, Matplotlib)
- Tableau
- Excel

## Dataset
The dataset contains ecommerce order information including:
- Product categories
- Sales revenue
- Profit
- Regions
- Customer segments
- Order dates
- Shipping information

## Key Questions
- Which regions generate the highest revenue?
- Which products perform best?
- Which categories are the most profitable?
- How do sales trends change over time?
- Which customer segments contribute the most revenue?

## Data Cleaning
The dataset was cleaned and prepared by:
- Removing duplicate records
- Handling missing values
- Standardizing column names
- Converting sales and profit columns to numeric data types
- Formatting dates for trend analysis

## SQL Analysis
Key SQL techniques used:
- Aggregate functions
- GROUP BY analysis
- ORDER BY ranking
- Revenue calculations
- Profitability analysis

Example query:

```sql
SELECT 
    Region,
    ROUND(SUM(Sales), 2) AS total_sales,
    ROUND(SUM(Profit), 2) AS total_profit
FROM orders
GROUP BY Region
ORDER BY total_sales DESC;
```

## Tableau Dashboard
The interactive Tableau dashboard includes:
- Total sales KPI
- Total profit KPI
- Regional sales comparison
- Monthly sales trends
- Top-performing products
- Category performance breakdown

## Key Insights
- The West region generated the highest overall revenue
- Technology products produced the strongest profit margins
- Sales increased significantly during holiday periods
- A small number of products contributed a large percentage of total revenue
- Some categories generated high sales but low profitability

## Business Recommendations
- Increase marketing investment in high-performing regions
- Focus inventory planning on top-performing products
- Improve profitability strategies for low-margin categories
- Use seasonal trends to optimize promotional campaigns

## What I Learned
- How to clean and prepare ecommerce sales data
- How to analyze revenue and profitability trends using SQL
- How to build interactive dashboards in Tableau
- How to communicate business insights through data visualization

## Project Files
- SQL queries
- Tableau dashboard
- Python analysis notebook
- Dataset
- Dashboard screenshots

## What I Actually Did
- Cleaned ecommerce sales data using Python and pandas
- Checked for missing values and inconsistent formatting
- Converted the sales column into numeric format for analysis
- Identified top-performing products and regions
- Used pandas groupby functions to analyze category performance
- Created visualizations to compare revenue trends
- Built charts showing sales performance across product categories
- Summarized which products contributed most to revenue
- Practiced explaining findings in business terms instead of only technical results

## Challenges
- The sales column initially imported as text instead of numeric values
- Some charts produced incorrect results until I cleaned the data types
- I had to learn how pandas aggregation functions worked
- Choosing the right chart types for dashboard readability took multiple revisions
- Interpreting the business meaning behind the numbers was harder than writing the code itself

## What I Learned
- Improved my SQL and Tableau skills through hands-on practice
- Learned how to communicate technical findings in business terms
- Practiced building dashboards that focus on clarity and usability
- Became more comfortable troubleshooting data and visualization issues