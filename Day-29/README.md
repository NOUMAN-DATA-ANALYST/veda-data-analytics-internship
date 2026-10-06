# Day 29: Basic Conditional Formatting in Excel

## Overview
This repository contains the completed Task 29 for the VEDA Technology Data Analytics Internship. The primary objective of this project is to improve report readability by implementing basic automated conditional formatting rules on a retail sales dataset.

## Objective
- Highlight top and bottom performing sales values dynamically.
- Eliminate manual color coding to prevent errors and optimize visualization.
- Ensure formatting automatically adjusts when underlying sales numbers change.

## Dataset Description
The dataset used is **Retail Sales Data**, containing transaction-level details including:
- `Transaction ID`, `Date`, `Customer ID`, `Gender`, `Age`
- `Product Category`, `Quantity`, `Price per Unit`, `Total Amount`

## Applied Rules & Logic
| Applied Conditional Formatting Rule | Target Column | Visual Formatting | Logic / Purpose |
| :--- | :--- | :--- | :--- |
| **Top 3 Items** | Total Amount | Green Fill with Dark Green Text | Automatically highlights the highest performing transactions. |
| **Bottom 3 Items** | Total Amount | Light Red Fill with Dark Red Text | Instantly flags low-value sales or potential outliers. |

## Verification & Edge Case Testing
- **Dynamic Response Test:** Modified a low-value cell (`$30`) to a high value (`$9,999`). The conditional formatting rule instantly shifted the cell highlight from Light Red to Green, validating rule automation.

## Interview Concepts Covered
1. **Why automate formatting?**
   Automating formatting saves time, reduces human error, and provides instant visual cues as data changes dynamically.
2. **What is conditional formatting?**
   It is a feature in spreadsheet software that automatically applies formatting (colors, data bars, icons) to cells based on specified criteria or formulas.
