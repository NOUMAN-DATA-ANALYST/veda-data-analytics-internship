# Day 26: Text Cleaning Basics in Excel

## 📌 Project Overview
This project is part of the **Veda Technology Data Analytics Internship (Day 26 Task)**. The objective of this task is to perform standard text-cleaning operations on a raw customer dataset using fundamental Excel formulas.

Cleaning and standardizing text data ensures consistency, prevents lookup errors, and prepares datasets for accurate analytical reporting and database storage.

---

## 🛠️ Tools & Functions Used
* **Tool:** Microsoft Excel
* **Excel Functions:**
  * `TRIM()`: Removes leading, trailing, and excessive internal whitespaces.
  * `PROPER()`: Standardizes capitalization by converting text to Proper Case (Capitalizing the first letter of each word).
  * `LOWER()`: Converts text strings into lowercase (specifically used for Email addresses).
  * `UPPER()`: Standardizes categories into uppercase (used for Status fields).

---

## 📂 Workbook Structure
The Excel workbook is structured into two separate worksheets to maintain an audit trail and data integrity:

1. **`Raw Data` Sheet:** Contains the original uncleaned dataset along with the applied live formulas for evaluation purposes.
2. **`Cleaned Data` Sheet:** Contains the final standardized dataset converted to static values (Paste Special > Values), ready for further analysis.

---

## 🔄 Before vs. After Transformation Examples

| Field | Raw / Uncleaned Input | Cleaned Output | Excel Formula Applied |
| :--- | :--- | :--- | :--- |
| **Full Name** | `   muhammad nouman   ` | `Muhammad Nouman` | `=PROPER(TRIM(B2))` |
| **Email Address** | ` SARA@GMAIL.COM ` | `sara@gmail.com` | `=LOWER(TRIM(D2))` |
| **City** | `  lahore` | `Lahore` | `=PROPER(TRIM(C2))` |
| **Status** | ` active` | `ACTIVE` | `=UPPER(TRIM(E2))` |

---

## 💡 Key Learnings & Interview Insights

### Q1: Why is whitespace a data-quality issue?
**Answer:** Whitespaces (leading, trailing, or duplicate spaces) cause data quality issues because tools like Excel, SQL, and Power BI treat `"Ali "` and `"Ali"` as distinct values. This leads to broken lookup functions (e.g., `VLOOKUP`/`XLOOKUP`), incorrect aggregations, and duplicated categories in Pivot Tables.

### Q2: What does `TRIM()` do?
**Answer:** The `TRIM()` function in Excel removes all leading and trailing spaces from a text string while reducing multiple consecutive spaces between words to a single space.

---

## 🚀 How to View
1. Download the `.xlsx` file from this repository.
2. Check the `Raw Data` sheet to review live dynamic formulas.
3. Check the `Cleaned Data` sheet for the final cleaned dataset.
