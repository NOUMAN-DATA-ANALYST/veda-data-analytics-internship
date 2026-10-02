Employee Data Management System — Basic Data Validation

This project demonstrates the implementation of Data Validation, Custom Dropdown Lists, Error Alerts, and Input Messages in Microsoft Excel to maintain data integrity and prevent user entry errors.

📌 Project Overview

When managing employee records or database entry sheets, improper formatting, misspellings, and out-of-range entries can significantly degrade data quality. This project establishes automated validation rules within Microsoft Excel to ensure all submitted records strictly adhere to company policies and data standards.

🚀 Features & Configuration Rules

The workbook is structured into two primary sheets:

Employee_Data: The main data entry worksheet protected with active validation rules.

LISTS: A dedicated reference sheet storing lookup values for dropdown lists.

📋 Validation Summary Table

Column Name

Data Type

Validation Type

Applied Criteria / Source Rule

Custom Alert / Message

Employee ID

Text

Manual Entry

Unique Identifier Format (EMPxxx)

—

Employee Name

Text

Manual Entry

Standard Text Input

—

Department

List

Dropdown List

Source: =LISTS!$A$2:$A$6

Restricts entries to valid department options

Role / Designation

Text

Manual Entry

Standard Job Title Input

—

Joining Date

Date

Date Criteria

Between 2015-01-01 and 2026-12-31

Input Message: Guidance on acceptable date format and range

Age

Whole Number

Numeric Limits

Between 18 and 65

Error Alert (Blocking): Rejects entries outside 18–65

Employment Status

List

Dropdown List

Source: =LISTS!$B$2:$B$5

Restricts options to pre-approved employment types

🛠️ Step-by-Step Implementation Guide

1. Data Structure Setup

Created main headers on Employee_Data: Employee ID, Employee Name, Department, Role/Designation, Joining Date, Age, and Employment Status.

Defined master lookup lists on the LISTS sheet:

Column A (Departments): HR, IT, Finance, Marketing, Operations

Column B (Employment Status): Full Time, Part Time, Contract, Intern

2. Dropdown List Configuration

Applied Data Validation to Department (C2:C20) using =LISTS!$A$2:$A$6.

Applied Data Validation to Employment Status (G2:G20) using =LISTS!$B$2:$B$5.

3. Date & Age Constraints

Configured Whole Number validation on Age (F2:F20) restricted to values between 18 and 65.

Configured Date validation on Joining Date (E2:E20) restricted to dates between 2015-01-01 and 2026-12-31.

4. User Guidance & Error Handling

Implemented a Blocking Error Alert on the Age column to stop invalid data entry.

Added an Input Message on the Joining Date column to guide end users before they input a date.

❓ Technical & Conceptual Insights

Q1: Why use Data Validation in spreadsheets?

Ensures Data Quality & Integrity: Prevents out-of-bounds numbers, incorrect dates, or invalid entries right at the point of input.

Reduces Data Cleaning Overhead: Eliminates human error during manual entry, saving significant preprocessing time during analysis and reporting.

Enforces Business Logic: Automatically enforces organizational policies (e.g., legal working age, valid employment contract dates).

Q2: What issues do dropdown lists prevent?

Spelling Errors & Typos: Stops users from entering typos (e.g., typing "Finanace" or "FIN" instead of "Finance").

Case Sensitivity & Formatting Discrepancies: Prevents variations caused by extra spaces or casing differences (e.g., "Full-Time" vs "full time"), which break summary formulas and data aggregation.

Unauthorized Categorization: Restricts selection strictly to pre-approved categories established in the reference list.

📂 Repository File Structure ├── Veda_Day25_Basic_Data_Validation.xlsx   # Main Excel Workbook
└── README.md                                # Project Documentation
