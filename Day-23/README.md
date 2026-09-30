# Day 23: SQL Aggregation Basics

## 📌 Project Overview
This project focuses on mastering SQL aggregate functions (`COUNT`, `SUM`, `AVG`, `MIN`, `MAX`) and understanding how they interact with `GROUP BY`, `HAVING`, and `NULL` values. The practical exercises were executed using SQLite/MySQL.

---

## 🛠️ Data Setup
A custom `Employees` table was constructed with deliberate `NULL` values in `Salary` and `Bonus` columns to analyze edge-case behaviors of SQL aggregations.

```sql
CREATE TABLE Employees (
    EmpID INT PRIMARY KEY,
    EmpName VARCHAR(50),
    Department VARCHAR(50),
    Salary DECIMAL(10, 2),
    Bonus DECIMAL(10, 2)
);
