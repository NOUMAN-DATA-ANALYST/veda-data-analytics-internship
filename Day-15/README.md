# 📊 Day 15: Product Count Analysis

## 🎯 Overview
This task focuses on analyzing product distribution across different categories using Microsoft Excel. The goal is to perform a product count analysis using criteria-based aggregation formulas to identify the largest product category.

---

## 🛠️ Tools Used
- **Tool:** Microsoft Excel
- **Functions:** `COUNTIF`, `Data Cleansing / Remove Duplicates`

---

## 📈 Summary & Key Results

| Category | Product Count |
| :--- | :--- |
| **Office Supplies** | **6,026** (Top Category) |
| **Furniture** | 2,121 |
| **Technology** | 1,847 |

- **Top Category:** **Office Supplies** with **6,026** products.

---

## ❓ Interview Questions & Concepts

### 1. What is the difference between `COUNTIF` and `COUNTIFS`?
- **`COUNTIF`:** Counts cells within a range that meet a **single specified criterion**.
  - *Syntax:* `=COUNTIF(range, criteria)`
- **`COUNTIFS`:** Counts cells within multiple ranges that meet **multiple criteria simultaneously**.
  - *Syntax:* `=COUNTIFS(criteria_range1, criteria1, [criteria_range2, criteria2], ...)`

### 2. Why is it important to count unique products?
- **Catalog Variety:** In transactional data, items repeat across orders. Counting unique products identifies the actual variety/catalog size rather than order volume.
- **Inventory Management:** Helps evaluate portfolio diversity and spot slow-moving or obsolete SKUs.

---

## 📂 Deliverables
- `Veda_Task15_Product_Count_Analysis.xlsx` — Excel workbook containing raw data, summary table, and interview answers.
