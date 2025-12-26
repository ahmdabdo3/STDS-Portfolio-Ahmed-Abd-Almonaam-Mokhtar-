# 🍕 Pizza Sales Analytics | SQL & Excel Project

![SQL](https://img.shields.io/badge/SQL-Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-Data_Analysis-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📖 Project Overview

This project involves a comprehensive analysis of a pizza store's sales data to uncover key business insights. By leveraging **SQL** for data extraction and querying, and **Excel** for visualization, the analysis identifies best-selling products, peak sales periods, and customer purchasing behaviors.

The goal is to provide data-driven recommendations to optimize inventory, marketing strategies, and operational efficiency.

---

## 🔢 Key Performance Indicators (KPIs)

Based on the dataset analysis, the following core metrics were established to measure business performance:

| Metric | Value | Description |
| :--- | :--- | :--- |
| **💰 Total Revenue** | **$817,860** | The sum of the total price of all pizza orders. |
| **📦 Total Orders** | **21,350** | The total number of orders placed. |
| **🍕 Total Pizzas Sold** | **49,574** | The total quantity of pizzas sold. |
| **🛒 Avg Order Value** | **$38.31** | The average amount spent per order. |
| **🔢 Avg Pizzas/Order** | **2.32** | The average number of pizzas per single order. |

---

## 🛠️ Tools & Technologies

* **SQL (Data Querying):** Used to perform complex queries, aggregations (`SUM`, `COUNT`, `AVG`), and grouping to extract KPIs and trends from the raw database.
* **Excel (Data Visualization):** Used to create Pivot Tables and Charts (Bar, Line, Pie) to visualize the SQL outputs.
* **Data Cleaning:** Handled data types and formatted date/currency fields for accurate analysis.

---

## 📊 Key Insights & Trends

### 1. 📅 Daily & Monthly Trends
* **Busiest Days:** **Friday** and **Saturday** see the highest volume of orders, indicating a strong weekend demand.
* **Peak Months:** **July** and **May** recorded the highest order activity, while consumption dips slightly towards the end of the year.

### 2. 🥧 Sales by Category & Size
* **Top Category:** The **Classic** category contributes the most to both total orders and total revenue.
* **Preferred Size:** **Large (L)** pizzas are the most popular choice among customers, accounting for the highest percentage of sales, followed by Medium (M).

### 3. 🏆 Best & Worst Sellers
Analysis of top 5 and bottom 5 pizzas based on Revenue, Quantity, and Total Orders:

* **👑 Best Seller:** The **Thai Chicken Pizza** generates the highest revenue. The **Classic Deluxe Pizza** is the most ordered by quantity.
* **📉 Worst Seller:** The **Brie Carre Pizza** consistently ranks lowest in revenue, total quantity, and total orders.

---

## 💻 SQL Methodology

The project utilized advanced SQL queries to derive insights. Below is a conceptual overview of the queries used:

```sql
-- Example: Calculating Total Revenue
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

-- Example: Daily Trend for Total Orders
SELECT DATENAME(DW, order_date) AS order_day, COUNT(DISTINCT order_id) AS total_orders 
FROM pizza_sales
GROUP BY DATENAME(DW, order_date);

-- Example: % of Sales by Pizza Category
SELECT pizza_category, CAST(SUM(total_price) AS DECIMAL(10,2)) as total_revenue,
CAST(SUM(total_price) * 100 / (SELECT SUM(total_price) from pizza_sales) AS DECIMAL(10,2)) AS PCT
FROM pizza_sales
GROUP BY pizza_category;
(Note: Full SQL script is available in the repository file SQL + EXCEL.sql)

📉 Visualizations
[Insert Screenshot of your Excel Dashboard here]

The Excel dashboard includes:

KPI Cards: Highlighting the main financial metrics.

Trend Charts: Line charts for daily and monthly order trends.

Distribution Charts: Pie charts showing sales % by category and size.

Ranking Charts: Bar charts for top/bottom 5 selling pizzas.

🚀 Business Recommendations
Promotional Offers: Launch special promotions for the Brie Carre Pizza to boost its sales or consider removing it from the menu if low performance persists.

Inventory Management: Stock up on ingredients for Classic pizzas and Large size dough, especially before Fridays and Saturdays.

Seasonal Marketing: Maximize marketing spend in July and May to capitalize on peak demand periods.

👤 Author
Ahmed Abdel Moneim

AI & Data Science Engineer
