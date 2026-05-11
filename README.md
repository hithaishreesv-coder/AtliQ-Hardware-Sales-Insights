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
