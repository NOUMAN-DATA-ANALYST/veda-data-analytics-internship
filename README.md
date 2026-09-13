# 🚢 Day 1 Task: Data Cleaning and Preprocessing (Titanic Dataset)

## 📌 Project Overview
This project is part of the **Veda Technology Data Analytics Internship**. The goal of Day 1 is to clean, preprocess, and standardize the raw **Titanic Dataset** using Python and Pandas in Kaggle Notebooks to prepare it for exploratory data analysis and visual modeling.

---

## 🛠️ Tech Stack & Tools
- **Language:** Python 3
- **Libraries:** Pandas, NumPy, OS
- **Environment:** Kaggle Notebooks / Jupyter Notebooks
- **Version Control:** Git & GitHub

---

## 🧹 Key Preprocessing Steps Applied

1. **Standardization:**
   - Standardized column names by converting them to lowercase and removing unwanted leading/trailing whitespaces.

2. **Handling Missing Values (Imputation):**
   - Imputed missing values in the `age` column using the **median** age value to avoid skewness.
   - Filled missing categorical values in `embarked` using the **mode** (most frequent entry).

3. **Feature Elimination:**
   - Dropped the `cabin` column due to a high percentage of missing values (low quality / sparse data).

4. **Deduplication:**
   - Checked and removed any duplicate rows across the dataset.

5. **Data Export:**
   - Exported the fully processed and standardized dataset as `cleaned_titanic.csv`.
  
6. # 📊 Day 4 Task: Interactive Sales Data Visualization Dashboard

## 📌 Project Overview
This project is part of the **Veda Technology Data Analytics Virtual Internship** (Day 4 Task). The objective is to analyze the Superstore sales dataset and present actionable business insights using an interactive, 4-page Power BI dashboard.

---

## 🚀 Key Features & Dashboard Pages

1. **Page 1: Sales vs Profit Analysis**
   - High-level KPIs tracking overall revenue and profit margins.
   - Category and Sub-category wise profit distribution.
   - Identification of core growth drivers and loss-making product segments.

2. **Page 2: Regional Performance**
   - Geographic sales breakdown across Regional zones (East, West, Central, South).
   - Analysis of regional profitability and sales volume trends.

3. **Page 3: Discount Impact Analysis**
   - Deep dive into how high discount rates correlate with negative profit margins.
   - Visualizing profit loss thresholds based on discount tiers.

4. **Page 4: Strategic Recommendations & Action Plan**
   - Proposed a **15% strict discount ceiling cap** to protect profit margins without sacrificing sales volume.
   - Resource allocation advice for underperforming product categories.

---

## 🛠️ Tools & Technologies Used
- **Power BI Desktop:** Dashboard design, DAX measures, and data modeling.
- **Data Source:** Sample Superstore Dataset.
- **Export Format:** PDF report documentation (`VEDA-DATA-VISUALIZATION-TASK-D4.pdf`).



# Day 5 Task: Excel Data Analysis & Business Reporting

## 📌 Project Overview
This repository contains the deliverables for **Day 5** of the **Veda Tec Data Analytics Internship**. The objective was to analyze the **Sample Superstore** dataset using **Excel for the Web** by applying data structuring best practices, key performance indicators (KPIs), dynamic conditional formulas (`SUMIFS`), multi-dimensional PivotTables, and executive business summaries.

---

## 🛠️ Data Architecture & Workflow

1. **Workbook Structure:**
   - `RAW-DATA`: Original unaltered dataset.
   - `WORKING-DATA`: Cleaned data formatted as a dynamic Excel Table (`Table1`) with frozen headers for easy navigation.
   - `SUMMARY`: Dedicated executive reporting sheet containing KPI cards, PivotTables, and findings.

2. **Core KPIs & Aggregations Calculated:**
   - **Total Revenue:** `$2,297,201` (`=SUM(Table1[Sales])`)
   - **Total Orders:** `9,994` (`=COUNTA(Table1[Order ID])`)
   - **Average Order Value (AOV):** `$229.86` (`=Total Revenue / Total Orders`)
   - **Technology Sales (Conditional):** `$836,154` (`=SUMIFS(Table1[Sales], Table1[Category], "Technology")`)

---

## 📊 Business Findings & Insights

- **Sales by Category:** **Technology** generated the highest total revenue (`$836,154`), closely followed by Furniture (`$741,999`) and Office Supplies (`$719,047`).
- **Sales by Region:** The **West Region** performed best with `$725,457` in sales, while the South region represents the lowest sales volume (`$391,721`).
- **Sales by Segment:** The **Consumer Segment** drives over 50% of total company revenue (`$1,161,401`).

---

## ❓ Business & Technical Interview Questions

### Q1: When would you use `SUMIFS` vs. a PivotTable for the same question?
> **Answer:** I use `SUMIFS` when I need a specific aggregate value integrated into a fixed dashboard card, custom financial template, or hardcoded report cell without altering the layout. I use a `PivotTable` for interactive, multi-dimensional exploratory data analysis, dynamic slicing, and rapid cross-tabulation.

### Q2: How do you keep a PivotTable's source data 'live' as new rows are added?
> **Answer:** By converting the raw data range into an official Excel Table (`Ctrl + T`) and referencing the structural Table name (e.g., `Table1`) as the PivotTable source. As new records are appended, the table auto-expands, and simply clicking **Refresh** updates all linked PivotTables.

### Q3: What's a KPI you'd track for a retail dataset, and why?
> **Answer:** **Average Order Value (AOV = Total Revenue / Total Orders)**. It measures the average dollar amount spent every time a customer places an order, helping evaluate customer purchasing behavior, pricing strategy, and the effectiveness of cross-selling tactics.



## 📅 Day 6: Excel Formulas & Functions Fundamentals

### 📌 Overview
Practiced core Excel functions (VLOOKUP, XLOOKUP, SUMIFS, COUNTIFS, Nested IF, and Text manipulation) on a retail transactional dataset.

### 🛠️ Formulas Implemented & Logic
* **Sales Tier (`Nested IF`):** `=IF(I2>=300, "High", IF(I2>=100, "Medium", "Low"))`
* **Category Code (`Text Join`):** `=UPPER(LEFT(F2, 3)) & "-" & D2`
* **Lookup Operations:** Implemented `VLOOKUP` and `XLOOKUP` on `lookup-analysis` sheet.
* **Aggregations:** Evaluated `SUMIFS` and `COUNTIFS` on `Summary-Metrics` sheet.

### ❓ Interview QA Summary
* **SUMIF vs SUMIFS:** `SUMIF` handles single conditions; `SUMIFS` supports multiple conditions with `sum_range` specified first.
* **XLOOKUP vs VLOOKUP:** `XLOOKUP` supports left lookups, avoids fixed column index dependencies, and features built-in error handling.
* **INDEX/MATCH vs VLOOKUP:** Provides bidirectional lookups and improved memory performance on large datasets.
