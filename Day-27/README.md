# Task 27: Date Cleaning Basics & Standardize Inconsistent Date Formats

## 📌 Project Overview
This project focuses on handling and standardizing inconsistent date formats in data analytics using Microsoft Excel. Raw datasets often contain dates formatted as plain text, mixed date structures, or invalid entries. This task ensures proper date parsing, structural formatting, and quality validation before performing further analysis.

## 🎯 Objectives
* Convert text-formatted dates into standardized date datatypes.
* Ensure reliable date handling across the dataset.
* Construct an **Issue Log** to flag missing, error-prone, or future transaction dates.
* Answer core data architecture questions regarding date datatypes and issues.

## 🛠️ Tools & Technologies Used
* **Microsoft Excel** (Excel Online / Excel Desktop)
* **Data Cleansing Formulas:** `DATE`, `DATEVALUE`, `TEXT`, `IF`, `ISBLANK`, `ISERROR`, `TODAY`

## 📊 Methodology & Steps Taken
1. **Data Inspection:** Verified date column alignment (Left-aligned text vs. Right-aligned true date datatypes).
2. **Explicit Parsing:** Standardized raw entries into a uniform `YYYY-MM-DD` / `MM/DD/YYYY` date format in a dedicated `Clean_Date` column.
3. **Data Quality Audit & Issue Logging:** Built a automated `Issue_Log` using dynamic logical checks:
   * **Missing Date:** Identifies blank cells.
   * **Invalid Format:** Flags syntax or parsing errors.
   * **Future Date:** Validates transactions against `TODAY()`.
   * **Valid:** Confirms verified records.

## 💡 Key Takeaways & Interview Insights
* **Why are dates problematic?** Dates vary across locales (`MM/DD/YYYY` vs `DD/MM/YYYY`), frequently export as string/text objects, and often contain invalid values that break chronological aggregation.
* **What is a Date Datatype?** A structured data representation stored as an underlying numeric serial value (e.g., Day 1 = Jan 1, 1900 in Excel), allowing time-series arithmetic, filtering, and duration metrics.

---
*Created as part of the Veda Technology Internship Program.*
