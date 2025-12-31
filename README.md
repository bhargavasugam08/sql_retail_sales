# Retail Sales Analysis SQL Project

## Project Overview

**Project Title**: Retail Sales Analysis  
**Level**: Beginner  

This is a beginner-level SQL project created to practice basic to intermediate SQL concepts.  
In this project, I work with a retail sales dataset to learn how to create tables, clean data, and write SQL queries to analyze sales information.

The main goal of this project is to improve my understanding of SQL and how it is used in real-world data analysis scenarios.

---

## Objectives

- Create a retail sales database and table
- Clean the data by removing NULL values
- Explore the dataset using basic SQL queries
- Answer simple business-related questions using SQL
- Practice aggregation, filtering, grouping, and window functions

---

## Project Structure

### 1. Database Setup

- A database named `sql_project_p1` is created.
- A table named `retail_sales` is created to store sales data such as transaction details, customer information, product category, and sales amount.

```sql
CREATE DATABASE sql_project_p1;

DROP TABLE IF EXISTS retail_sales;

CREATE TABLE retail_sales 
(
    transactions_id INT PRIMARY KEY,	
    sale_date DATE,
    sale_time TIME,
    customer_id INT,
    gender VARCHAR(15),
    age INT,
    category VARCHAR(15),	
    quantiy INT,
    price_per_unit FLOAT,
    cogs FLOAT,
    total_sale FLOAT
);

