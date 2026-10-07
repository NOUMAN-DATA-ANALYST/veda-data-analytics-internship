# Day 30: Simple Inventory Tracker & Low-Stock Report

## Project Overview
This project focuses on building a rule-based inventory tracking system in Microsoft Excel to monitor product stock levels, reorder thresholds, and operational stock statuses dynamically. The goal is to provide clear visibility into inventory health and automatically generate low-stock reports for timely purchasing decisions.

## Objectives
- Practice rule-based inventory tracking and status determination.
- Implement conditional logic using Excel formulas (`IF`).
- Apply conditional formatting for dynamic visual alerts.
- Filter and isolate low-stock items into an actionable report.

## Deliverables
1. **Master Inventory Tracker Sheet**: Complete list of inventory items with stock status logic.
2. **Low-Stock Report Sheet**: Filtered report highlighting items that require reordering.

## Key Features & Logic
- **Stock Status Automation**: Evaluates whether `Current Stock <= Reorder Level`.
  - **Formula Used**: `=IF(C2<=D2, "Reorder", "In Stock")`
- **Visual Risk Highlighting**: Conditional formatting automatically highlights `"Reorder"` items in light red to draw immediate attention.
- **Reporting**: Isolated view for purchasing teams to manage inventory depletion efficiently.

## Practical Insights / Interview Questions
- **What is Reorder Level?**
  The reorder level is a minimum stock threshold that triggers a purchase order to prevent stockouts before new stock arrives.
- **Why Track Stock Status?**
  Tracking stock status ensures optimal inventory levels, prevents holding excess stock (reducing carrying costs), and guarantees uninterrupted supply chain operations.

## Tools Used
- Microsoft Excel (Formulas, Conditional Formatting, Data Filtering)
