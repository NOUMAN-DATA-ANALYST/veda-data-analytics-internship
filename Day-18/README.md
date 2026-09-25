Day 18: Region Performance Dashboard

📌 Project Overview

This project is part of the Veda Technology Business Intelligence Internship. The objective of Day 18 was to analyze regional performance across the dataset, calculate total sales, total profit, and rank regions dynamically using DAX measures, and visualize the findings using both a summary table and a clustered bar chart.

🛠️ Key Features & Technical Implementation

Summary Table & Data Visuals:

Table Visual: Highlighting regional performance using aggregated measures and dynamic ranking.

Clustered Bar Chart: Visualizing Total Sales and Total Profit across regions with customized colors and data labels for instant readability.

DAX Measures Created:

Total Sales:

Total Sales = SUM('Sample - Superstore'[Sales])


Total Profit:

Total Profit = SUM('Sample - Superstore'[Profit])


Region Rank (Dynamic Ranking):

Region Rank = RANKX(ALL('Sample - Superstore'[Region]), [Total Sales], , DESC, Dense)


Multi-Page Report Architecture:

Page 1 (Region Performance): Main executive dashboard containing tables, charts, and key business visual indicators.

Page 2 (Interview Questions & Documentation): Dedicated page embedded directly in the .pbix file to outline DAX logic and key insights.

💡 Key Business Insights

Top Performing Region: The West region secured Rank 1, leading both in Total Sales ($725,457.82) and Total Profit ($108,418.45).

Low Margin Alert: The Central region maintains strong overall sales ($501,239.89) but yields significantly lower profit margins ($39,706.36) compared to other regions, indicating high operational costs or discount structures.

❓ Technical Q&A (Viva / Interview Notes)

Q1: Why did you use the ALL() function inside the RANKX measure?

Answer: The ALL('Sample - Superstore'[Region]) function overrides and clears the row-level filter context on the Region column within the visual. This allows RANKX to evaluate all regions simultaneously and assign a true, relative rank (1 to 4) across the entire dataset.

Q2: What is the primary difference between a Calculated Column and a DAX Measure?

Answer: A Calculated Column evaluates values row-by-row during data refresh and stores the result in RAM (increasing overall file size). A DAX Measure calculates aggregations dynamically at runtime based on user interactions, filters, and slicers, making it much more performance-efficient.

📂 Repository Contents

Day 18 - Region Performance.pbix — Full Power BI Desktop report containing visuals, measures, and documentation.

README.md — Project documentation and interview insights.
