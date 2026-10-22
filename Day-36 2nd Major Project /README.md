# COVID-19 Global Impact & Analytical Dashboard

## 📌 Project Overview
This project presents an interactive **COVID-19 Global Impact & Vaccination Dashboard** built using **Power BI** and **Python**. It provides an in-depth epidemiological analysis of global COVID-19 trends, mortality severity, and vaccination coverage across 200+ countries from 2020 to 2024.

---

## 📊 Key Business Insights & Metrics
- **Total Confirmed Cases:** 103 Million global cases recorded.
- **Total Deaths:** 1 Million global deaths recorded.
- **Overall Case Fatality Rate (CFR %):** 1.15% fatality rate across diagnosed cases.
- **Total Vaccinations:** Over 3 Billion doses administered globally.
- **7-Day Rolling Average Trends:** Smoothed out weekend reporting lags to highlight true epidemiological surges (e.g., Alpha, Delta, and Omicron waves).
- **Normalized Country Impact:** Analyzed Top 10 impacted countries per million population to ensure fair regional comparison.

---

## 🛠️ Tech Stack & Tools
- **Data Processing:** Python (Pandas, NumPy)
- **Data Visualization & BI:** Power BI Desktop
- **Analytics & Calculations:** DAX (Data Analysis Expressions)
- **Data Modeling:** Star Schema / Fact Table Optimization

---

## 📐 DAX Measures Implemented
- **Total Cases:** `Total Cases = MAX(cleaned_covid_data[total_cases])`
- **Total Deaths:** `Total Deaths = MAX(cleaned_covid_data[total_deaths])`
- **Total Vaccinations:** `Total Vaccinations = MAX(cleaned_covid_data[total_vaccinations])`
- **Overall CFR %:** `Overall CFR % = DIVIDE([Total Deaths], [Total Cases], 0)`

---

## 📸 Dashboard Preview
![Dashboard Preview](Dashboard_Overview.png)

---

## 📂 Repository Contents
- `COVID19_Global_Impact_Dashboard.pbix` : Power BI Desktop File
- `COVID19_Global_Impact_Dashboard.pdf` : PDF Version of the Report
- `cleaned_covid_data.csv` : Processed Dataset
- `README.md` : Documentation & Insights Report
