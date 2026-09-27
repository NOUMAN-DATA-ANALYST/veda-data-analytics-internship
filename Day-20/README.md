# Day 20: Customer Order Count Analysis (Superstore Dataset)

## 📌 Project Overview
This task is part of the **Veda Technology Data Analytics Internship**. The primary goal is to analyze customer purchasing behavior by determining the total order count per customer using SQL on the **Sample Superstore** dataset.

## 🎯 Objectives
- Identify unique customers and their total order frequencies.
- Identify top repeat buyers (highest order counts).
- Resolve duplicate product line entries using `COUNT(DISTINCT order_id)`.
- Document key analytical insights and answer core interview questions regarding customer metrics.

---

## 🛠️ SQL Query Used

```sql
SELECT 
    customer_id,
    customer_name,
    COUNT(DISTINCT order_id) AS Total_Orders
FROM SampleSuperstore
GROUP BY customer_id, customer_name
ORDER BY Total_Orders DESC
LIMIT 10;
