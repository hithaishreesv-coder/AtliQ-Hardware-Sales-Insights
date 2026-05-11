# AtliQ Hardware Sales Insights Dashboard

## Project Overview

This project focuses on building a Sales Insights Dashboard for AtliQ Hardware using Power BI and MySQL.

AtliQ Hardware is a company that supplies computer hardware and peripherals to clients across India. The Sales Director was facing difficulty in tracking sales performance because the business was growing dynamically and overall sales were declining.

Previously, sales updates were shared verbally by regional managers or through multiple Excel files. This made it difficult for the Sales Director to understand the complete business picture and make data-driven decisions.

The goal of this project was to create an automated Power BI dashboard connected to MySQL data, allowing stakeholders to track sales performance, revenue, profit margin, customer performance, market performance, and sales trends in one place.

---

## Problem Statement

AtliQ Hardware operates across multiple regions in India, including North India, South India, and Central India.

The Sales Director was facing the following challenges:

- Overall sales were declining
- Sales insights were shared verbally without proper data proof
- Regional managers provided limited information over phone calls
- Business data was spread across multiple Excel files
- Manual reporting was time-consuming
- There was no central dashboard to track real-time business performance
- The company needed clear insights to make better sales decisions

To solve this problem, a Power BI dashboard was developed to provide clear, automated, and data-driven sales insights.

---

## Project Objectives

The main objectives of this project were:

- Connect Power BI to a MySQL database
- Explore sales data using SQL queries
- Clean and transform raw sales data
- Build a data model in Power BI
- Create useful DAX measures
- Develop an interactive sales dashboard
- Track revenue, sales quantity, and profit margin
- Analyse sales performance by market, customer, and product
- Help business users make data-driven decisions

---

## Tools and Technologies Used

- Power BI
- MySQL
- SQL
- Power Query
- DAX
- Data Modelling
- Data Cleaning
- Data Visualisation

---

## Project Planning using AIMS Grid

### Purpose

To unlock sales insights that were not visible before and automate the reporting process for the sales team.

The dashboard helps reduce manual time spent on data gathering and supports better decision-making.

### Stakeholders

The main stakeholders involved in this project are:

- Sales Director
- Regional Sales Managers
- Marketing Team
- Customer Service Team
- Data Analytics Team
- IT Team

### End Result

The final output is an automated Power BI dashboard that provides quick and updated sales insights.

The dashboard helps stakeholders understand business performance and take data-driven decisions.

### Success Criteria

The success of this project is measured by:

- Dashboard showing clear sales insights
- Sales team being able to make better decisions
- Reduction in manual data gathering
- Identification of declining sales areas
- Improved visibility into market, customer, and product performance

---

## Data Exploration using MySQL

The dataset was first imported into MySQL and explored using SQL queries.

Some of the SQL queries used were:

```sql
SELECT * FROM sales.customers;

SELECT * FROM sales.transactions;

SELECT * FROM sales.markets;

During data exploration, the following data quality issues were identified:

- Some sales amount values were zero or negative, which were invalid for sales analysis.
- Some transactions were recorded in USD and needed to be converted into INR.
- Markets such as New York and Paris were present, although the main business focus was India.
- Currency values had formatting inconsistencies such as `INR` and `INR\r`.
- Data cleaning was required before building the dashboard.

Data Cleaning and Transformation

Data cleaning was performed in Power BI using Power Query.

The main cleaning steps included:

Removed invalid sales amounts such as 0 and negative values
Removed markets outside India, such as New York and Paris
Converted USD currency values into INR
Cleaned duplicate currency values
Created a normalised sales amount column
Converted date format into month-year format for better visualisation
Prepared clean data for dashboard reporting
Data Modelling

After cleaning the data, relationships were created between the required tables in Power BI.

The main tables used in the project were:

Customers
Transactions
Markets
Products
Date

The data model helped connect sales transactions with customer, product, market, and date information.

DAX Measures

The following DAX measures were created for analysis:

Revenue
Revenue = SUM('sales transactions'[norm_sales_amount])
Sales Quantity
Sales Qty = SUM('sales transactions'[sales_qty])
Total Profit Margin
Total Profit Margin = SUM('sales transactions'[Profit_Margin])
Profit Margin Percentage
Profit Margin % = DIVIDE([Total Profit Margin], [Revenue], 0)
Revenue Contribution Percentage
Revenue Contribution % =
DIVIDE(
    [Revenue],
    CALCULATE(
        [Revenue],
        ALL('sales products'),
        ALL('sales customers'),
        ALL('sales markets')
    )
)
Profit Margin Contribution Percentage
Profit Margin Contribution % =
DIVIDE(
    [Total Profit Margin],
    CALCULATE(
        [Total Profit Margin],
        ALL('sales products'),
        ALL('sales customers'),
        ALL('sales markets')
    )
)
Dashboard Features

The Power BI dashboard includes the following visuals and KPIs:

Total Revenue
Total Sales Quantity
Total Profit Margin
Revenue by Market
Sales Quantity by Market
Top 5 Customers
Top 5 Products
Revenue Trend
Profit Margin Analysis
Market-level sales performance
Key Insights

The dashboard helps answer important business questions such as:

Which market is generating the highest revenue?
Which market is underperforming?
Which customers are contributing the most revenue?
Which products are performing best?
Is revenue increasing or declining over time?
Which region needs more business attention?
How much profit margin is generated from sales?
Business Impact

This dashboard helps the Sales Director and other stakeholders monitor business performance using real data.

Instead of depending on verbal updates or multiple Excel files, the dashboard provides a clear view of sales performance in one place.

The project supports:

Faster decision-making
Better sales tracking
Improved visibility into business performance
Reduced manual reporting time
Data-driven business planning
Files in this Repository

This repository may include:

Power BI dashboard file
SQL queries used for data exploration
Dashboard screenshots
README documentation
How to Use This Project
Download or clone this repository.
git clone https://github.com/your-username/AtliQ-Hardware-Sales-Insights.git
Import the sales dataset into MySQL.
Open Power BI Desktop.
Connect Power BI to the MySQL database.
Load the required tables.
Apply data cleaning steps in Power Query.
Create DAX measures.
Build and view the dashboard.
Conclusion

The AtliQ Hardware Sales Insights Dashboard provides a clear and interactive view of business performance.

By using Power BI, MySQL, Power Query, SQL, and DAX, this project shows how raw sales data can be cleaned, transformed, and visualised into meaningful insights.

The dashboard helps identify declining sales trends, high-performing markets, top customers, and product-level performance, allowing the business to make better data-driven decisions.

Author

Hithaishree Salur Vijay

Data Analyst | Power BI | SQL | Python | Machine Learning
