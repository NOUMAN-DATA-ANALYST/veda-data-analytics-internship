# VEDA Data Analytics Internship - Day 22: SQL Filtering Practice

## 📌 Overview
This repository contains the deliverables for **Day 22** of the VEDA Data Analytics Internship. The primary focus of this task is practicing core SQL filtering techniques using different conditional operators to query relational database tables efficiently.

---

## 🎯 Objectives
- Implement foundational to advanced SQL filtering clauses.
- Practice data filtering using `WHERE`, `IN`, `BETWEEN`, and `LIKE` operators.
- Analyze query behavior on relational schemas (Northwind Database).

---

## 🛠️ Tools & Environment
- **Database Engine:** SQLite / SQLiteOnline
- **Dataset:** Northwind Traders Database
- **Documentation:** Microsoft Excel (`VEDA_Day22_SQL_Filtering_Practice.xlsx`)

---

## 📊 Summary of Queries & Deliverables

| Query No. | Filtering Concept | SQL Operator Used | Focus / Objective |
| :--- | :--- | :--- | :--- |
| **Query 1** | Exact Matching | `=` | Filter customers located in Germany |
| **Query 2** | Greater Than Evaluation | `>` | Filter products with price exceeding $30 |
| **Query 3** | Inequality Evaluation | `<>` | Exclude products belonging to Category 1 |
| **Query 4** | Logical Combination | `AND` | Multi-condition filtering on Category & Price |
| **Query 5** | Multiple Set Inclusion | `IN` | Filter customers from Germany, France, or UK |
| **Query 6** | Multiple Set Exclusion | `NOT IN` | Exclude products from Categories 1, 3, and 5 |
| **Query 7** | Numeric Range | `BETWEEN` | Retrieve items priced between $10 and $20 |
| **Query 8** | Date Range | `BETWEEN` | Retrieve orders placed in July 1996 |
| **Query 9** | Prefix Matching | `LIKE 'A%'` | Retrieve companies starting with letter 'A' |
| **Query 10** | Substring Matching | `LIKE '%Sales%'` | Retrieve job titles containing 'Sales' |
| **Query 11** | Fixed Length Matching | `LIKE 'A____'` | Retrieve 5-character IDs starting with 'A' |
| **Query 12** | Complex Filtering | `IN` + `LIKE` | Combined set comparison and pattern search |

---

## ❓ Conceptual Key Learnings (Interview Q&A)

### 1. `LIKE` vs `=`
- **`=` Operator:** Used for exact literal comparisons (e.g., `WHERE Country = 'Germany'`).
- **`LIKE` Operator:** Used for flexible pattern matching using wildcards:
  - `%`: Represents zero or multiple characters.
  - `_`: Represents a single character.

### 2. When to use `BETWEEN`
- Best suited for filtering continuous numeric or chronological ranges inclusive of both start and end boundaries (e.g., salary bands, product prices, date intervals).

---

## 📁 Repository Structure
