# E-Commerce Customer Segmentation (RFM Analysis) 🎯

## 📌 Project Overview
This project focuses on segmenting e-commerce customers using the industry-standard **RFM (Recency, Frequency, Monetary)** framework combined with **K-Means Clustering** machine learning technique. The objective is to translate transactional customer data into actionable business and marketing recommendations to optimize loyalty programs and win-back campaigns.

---

## 🛠️ Tools & Technologies Used
* **Python (Google Colab):** Data Cleaning, Feature Engineering, RFM Metrics Calculation, StandardScaler, and K-Means Clustering.
* **Pandas & NumPy:** Exploratory Data Analysis & Manipulation.
* **Scikit-Learn:** Machine Learning Model for Customer Clustering.
* **Power BI:** Interactive Dashboard, Data Visualizations, KPI Cards, and Segment Analysis.

---

## 📊 Methodology & Steps Executed

### 1. Data Cleaning & Preprocessing
* Loaded the raw UCI Online Retail dataset.
* Removed missing records containing null `CustomerID` values.
* Excluded cancelled orders (invoices starting with 'C') and invalid negative/zero prices and quantities.
* Calculated total transaction amount (`TotalSum = Quantity * UnitPrice`).

### 2. RFM Metrics Calculation
For each unique customer, calculated three core parameters:
* **Recency (R):** Days elapsed since the customer's last transaction relative to the reference date.
* **Frequency (F):** Total number of distinct orders placed by the customer.
* **Monetary (M):** Total monetary value spent across all orders.

### 3. Machine Learning (K-Means Clustering)
* Standardized RFM features using `StandardScaler` to bring metrics to an equal scale.
* Applied **K-Means Clustering** ($K=4$) to partition customers into distinct behavioural groups.
* Mapped numerical clusters into business-friendly marketing segments:
  * 🥇 **Champions:** High spenders, frequent shoppers, and recently active.
  * 💎 **Loyal Customers:** Frequent buyers with consistent revenue contributions.
  * ⚠️ **At-Risk Customers:** Previously valuable customers who haven't purchased recently.
  * ❌ **Lost Customers:** Inactive buyers with low engagement and spending.

### 4. Interactive Power BI Dashboard
Built a comprehensive one-page dashboard displaying:
* **KPI Summary Cards:** Total Customers, Total Revenue, and Average Recency.
* **Donut Chart:** Customer Count Distribution by Segment.
* **Clustered Column Chart:** Total Revenue Contribution by Segment.
* **Scatter Plot:** Recency vs Monetary distribution across segments.
* **Dynamic Slicer:** Segment filter for deep-dive analysis.

---

## 💡 Business Recommendations

1. **Champions:** Target with exclusive VIP loyalty offers, early access to new product launches, and referral incentives.
2. **At-Risk Customers:** Launch targeted "Win-Back" email campaigns featuring personalized discounts and special deals to reactivate them before churn.
3. **Lost Customers:** Minimize direct marketing spending and utilize automated low-cost re-engagement ad campaigns.

---

## 📂 Project Repository Structure
