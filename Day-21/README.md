# Veda Technology Internship - Day 21: Basic SQL SELECT Queries

This repository contains the completed deliverables for **Day 21** of the Veda Technology Data Analytics Internship. The primary focus of this task is executing basic SQL operations, filtering data, and sorting results using SQLite on the **Chinook Database**.

---

## 📋 Task Overview
* **Database:** Chinook Database (SQLite)
* **Environment:** SQLite Online (`sqliteonline.com`)
* **Focus Areas:** `SELECT`, `WHERE`, `AND`, `IN`, `ORDER BY`, `LIMIT`
* **Deliverables:** 10 SQL Queries with logic explanations and core SQL interview question answers.

---

## 🛠️ Executed SQL Queries & Logic

| Query # | Category | Objective | SQL Query | Logic & Explanation |
| :---: | :--- | :--- | :--- | :--- |
| **Query 1** | Basic SELECT | Fetch all customer details | `SELECT * FROM Customer;` | Retrieves all columns and rows from the `Customer` table using the `*` wildcard. |
| **Query 2** | Column Selection | Fetch specific customer fields | `SELECT FirstName, LastName, Email FROM Customer;` | Selects specific contact columns to optimize query performance and data transfer. |
| **Query 3** | Basic SELECT | Retrieve track names & prices | `SELECT Name, UnitPrice FROM Track;` | Fetches track titles and unit prices from the `Track` table. |
| **Query 4** | WHERE Filtering | Filter customers in USA | `SELECT FirstName, LastName, Country FROM Customer WHERE Country = 'USA';` | Filters records where `Country` strictly matches `'USA'`. |
| **Query 5** | WHERE Filtering | Find premium tracks (> $0.99) | `SELECT Name, UnitPrice FROM Track WHERE UnitPrice > 0.99;` | Filters tracks priced above `$0.99` using comparison operators. |
| **Query 6** | WHERE + AND | Filter customers in New York, USA | `SELECT FirstName, LastName, City, Country FROM Customer WHERE Country = 'USA' AND City = 'New York';` | Applies dual conditions (`Country = 'USA'` AND `City = 'New York'`). |
| **Query 7** | WHERE + IN | Customers in USA or Canada | `SELECT FirstName, LastName, Country FROM Customer WHERE Country IN ('USA', 'Canada');` | Uses `IN` operator to match multiple discrete country values. |
| **Query 8** | ORDER BY (ASC) | Sort customers A-Z by Last Name | `SELECT FirstName, LastName, Country FROM Customer ORDER BY LastName ASC;` | Sorts records alphabetically by `LastName` in ascending order. |
| **Query 9** | ORDER BY (DESC) | Sort tracks High-to-Low by price | `SELECT Name, UnitPrice FROM Track ORDER BY UnitPrice DESC;` | Arranges tracks in descending price order. |
| **Query 10** | ORDER BY + LIMIT | Top 5 most expensive tracks | `SELECT Name, UnitPrice FROM Track ORDER BY UnitPrice DESC LIMIT 5;` | Combines `ORDER BY DESC` and `LIMIT 5` to isolate the top 5 highest-priced tracks. |

---

## ❓ Interview Questions & Answers

### **Q1: What does `SELECT` do in SQL?**
> **Answer:** The `SELECT` statement is the primary SQL command used to retrieve and query data from one or more database tables. It allows users to filter and view specific columns without modifying or altering the underlying raw data.

### **Q2: What does `ORDER BY` do in SQL?**
> **Answer:** The `ORDER BY` clause sorts the result set returned by a query in ascending (`ASC`, default) or descending (`DESC`) order based on specified columns. It is crucial for ranking data, sorting text alphabetically, or arranging numeric values chronologically/sequentially.

---

## 📁 Files Included
* `Veda_Internship_Day21_SQL_Report.xlsx` — Full Excel report containing queries, explanations, and interview prep.
* `README.md` — Project summary and SQL query documentation.
