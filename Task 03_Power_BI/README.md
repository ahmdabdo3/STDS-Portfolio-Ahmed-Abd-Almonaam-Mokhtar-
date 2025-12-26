# 👗 Fashion Retail Analytics | SQL & Power BI Solution

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=Power%20Bi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Data Engineering](https://img.shields.io/badge/Data_Engineering-ETL-blue?style=for-the-badge)

## 📖 Project Overview

This project is a comprehensive end-to-end Business Intelligence solution designed to analyze the sales performance of a fashion retail business. Leveraging **SQL** for robust data processing and **Power BI** for advanced visualization, the solution provides deep insights into profitability, product trends, and customer behavior. 

The objective is to move beyond static reporting to a dynamic, interactive experience that answers critical business questions regarding sales performance, profit margins, and customer segmentation.

---

## 🚀 Key Performance Indicators (Headline Metrics)

The analysis is built upon a high-volume transactional dataset, summarizing the following financial and operational metrics:

| Metric Category | KPI Name | Value |
| :--- | :--- | :--- |
| **Financials** | 💰 Total Sales | **$123M** |
| | 💵 Total Revenue | **$117M** |
| | 📈 Total Profit | **$54M** |
| | 📉 COGS | **$69M** |
| | 📊 Profit Margin | **43.81%** |
| **Operations** | 📦 Total Orders | **120K** |
| | 🛒 Avg Order Value | **$1.03K** |
| **Customer Base** | 👥 Total Customers | **33K** |

---

## 🛠️ Tools & Technologies

* **SQL (Data Transformation):** Used for cleaning raw transactional data, handling inconsistent values/nulls, and aggregating metrics (Revenue, Profit, Orders) to create analysis-ready views.
* **Power BI (Visualization):** Developed a multi-page interactive dashboard with dynamic navigation.
* **DAX (Data Modeling):** Implemented complex measures for Time-Intelligence (YoY, MoM), Pareto Analysis, and Moving Averages.
* **Data Modeling:** Designed a Star Schema optimized for high-performance querying.

---

## 🔄 Data Architecture & SQL Workflow

The project follows a structured ETL (Extract, Transform, Load) process:

1.  **Data Cleaning:** Validation of transactional records and handling missing values.
2.  **Aggregation:** Calculation of core business metrics at the grain level.
3.  **View Generation:** SQL views were created to feed the BI tool:
    * `vw_Sales_Trends`: Yearly, Quarterly, and Monthly aggregates.
    * `vw_Product_Performance`: Category and Subcategory breakdowns.
    * `vw_Customer_Metrics`: Customer lifetime value and segmentation.
    * `vw_Geo_Analysis`: Country-level sales performance.

---

## 📊 Dashboard Analysis Modules

The solution is divided into **6 analytical modules**, each focusing on a specific business dimension:

### 1. 🔹 Snapshot Overview
* **Executive Summary:** High-level cards for quick health checks.
* **Statistical Distribution:** Analysis of order values (Min, Max, Median, Mode).
* **Forecasting:** Predictive time-series modeling for future sales.

### 2. 🔹 Sales Performance
* **Temporal Analysis:** Drill-down capabilities from Year → Quarter → Month.
* **Growth Tracking:** Year-over-Year (YoY) and Month-over-Month (MoM) visualizations.
* **Channel Split:** Comparative analysis of Online vs. In-store performance.

### 3. 🔹 Profitability & Margins
* **Cost Analysis:** Revenue vs. COGS breakdown.
* **Margin Trends:** Tracking profit margin fluctuations across different seasons.
* **Customer Profitability:** Identifying high-value vs. low-margin customers.

### 4. 🔹 Product Intelligence
* **Category Performance:** Revenue and profit matrix by Category and Subcategory.
* **Trend Analysis:** Identifying rising and declining product lines.

### 5. 🔹 Customer Segmentation
* **Demographics:** Sales breakdown by Gender and Geography.
* **Pareto Analysis (80/20 Rule):** Identifying the top 20% of customers contributing to 80% of revenue.
* **Top Spenders:** Leaderboards for top-tier clients.

### 6. 🔹 Advanced Insights
* **Geo-Spatial Analysis:** Heatmaps showing profit distribution by country.
* **Seasonality:** Understanding the impact of seasons on order volume.

---

## 🎛️ Interactive Capabilities

The report allows users to slice and dice data dynamically using:
* **Time Filters:** Year, Quarter, Month.
* **Categorical Filters:** Product Category, Subcategory.
* **Geographic Filters:** Country, Region.
* **Cross-Filtering:** Clicking on any metric updates the entire dashboard context.

---

## 👤 Author

**Ahmed Abdel Moneim**
* *AI & Data Science Engineer*
* [LinkedIn Profile](Your_LinkedIn_URL) | [GitHub Profile](Your_
