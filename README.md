# AtliQ Hardware Sales Insights Dashboard

## Project Overview

This project focuses on building a Power BI dashboard for AtliQ Hardware, a company that supplies computer hardware and peripherals across India.

The Sales Director was facing difficulty in tracking business performance because sales insights were shared verbally by regional managers or through multiple Excel files. This made it difficult to understand the real reason behind declining sales.

The goal of this project was to build an automated Power BI dashboard connected to MySQL data, so the business could track revenue, sales quantity, profit margin, customer performance, market performance, and revenue trends in one place.

## Problem Statement

AtliQ Hardware operates across multiple regions in India. The company was experiencing a decline in sales, but the Sales Director did not have a clear, data-driven view of the business.

The main challenges were:

- Sales insights were shared verbally without supporting data
- Regional performance was difficult to compare
- Data was spread across multiple files
- Manual reporting was time-consuming
- Business leaders needed a dashboard to make faster decisions

## Project Objectives

- Build an automated sales dashboard in Power BI
- Connect Power BI to MySQL database
- Clean and transform messy sales data
- Track revenue, sales quantity, and profit margin
- Identify top-performing markets, customers, and products
- Help stakeholders make data-driven decisions

## Tools and Technologies Used

- Power BI
- MySQL
- Power Query
- DAX
- SQL
- Data Modelling
- Data Cleaning
- Data Visualisation

## Project Planning: AIMS Grid

### Purpose

To unlock sales insights that were previously not visible and automate manual reporting for the sales team.

### Stakeholders

- Sales Director
- Marketing Team
- Customer Service Team
- Data Analytics Team
- IT Team

### End Result

An automated Power BI dashboard that provides quick and updated sales insights to support business decision-making.

### Success Criteria

- Dashboard provides clear sales order insights
- Sales team can make better business decisions
- Manual data gathering time is reduced
- Business performance can be monitored using real data

## Data Exploration using MySQL

The dataset was first explored using MySQL queries.

Example queries used:

```sql
SELECT * FROM sales.customers;

SELECT * FROM sales.transactions;

SELECT * FROM sales.markets;
