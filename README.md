# 🍕 Pizza Sales Dashboard — Power BI

An end-to-end Power BI dashboard analyzing a full year of pizza sales data (Jan–Dec 2025), built to answer real business questions around revenue, order patterns, and product performance. SQL was used to independently validate every KPI and chart before building it in Power BI.

## 📊 About the Project

A pizza restaurant wanted to understand its sales performance across the year — which days and months drive the most orders, which pizzas are top and bottom performers, and how customer preferences break down by category and size. This project turns raw order-level data into a 2-page interactive report that answers those questions at a glance.

**Key results surfaced by the dashboard:**
- **817.86K** total revenue, **49,574** pizzas sold, **21,350** total orders
- **38.31** average order value, **2.32** average pizzas per order
- Orders peak on **weekends, especially Friday/Saturday evenings**
- **July and January** are the highest-volume months
- **Classic** category and **Large** size pizzas contribute the most to sales
- **The Thai Chicken Pizza** is the top performer by revenue; **The Brie Carre Pizza** is the lowest across revenue, quantity, and orders

## 🧭 Dashboard Pages

**1. Home**
- KPI cards: Total Revenue, Total Pizzas Sold, Total Orders, Avg Order Value, Avg Pizzas per Order
- Daily trend for total orders (bar chart)
- Monthly trend for total orders (line chart)
- % of sales by pizza category (donut chart)
- % of sales by pizza size (donut chart)
- Total pizzas sold by pizza category (funnel chart)
- Slicers for Pizza Category and Order Date

**2. Best/Worst Sellers**
- Top 5 and Bottom 5 pizzas by Revenue, Total Quantity, and Total Orders (bar charts)
- Summary callouts for best- and worst-performing pizzas by revenue, quantity, and orders

## 🎯 Business Requirements

The dashboard was built against a defined set of chart requirements:

| # | Requirement | Chart Type |
|---|---|---|
| 1 | Daily trend for total orders | Bar chart |
| 2 | Monthly trend for total orders | Line chart |
| 3 | % of sales by pizza category | Pie/donut chart |
| 4 | % of sales by pizza size | Pie/donut chart |
| 5 | Total pizzas sold by pizza category | Funnel chart |
| 6 | Top 5 best sellers by revenue, quantity, orders | Bar chart |
| 7 | Bottom 5 worst sellers by revenue, quantity, orders | Bar chart |

## 🛠️ Tools & Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, report design
- **SQL** — pre-validation of every KPI and chart value against raw data before building visuals
- **Excel/CSV** — raw source data

## ✅ SQL Validation

Every number on the dashboard was first calculated and cross-checked in SQL, covering:
- Core KPIs: total revenue, total orders, average order value, total pizzas sold, average pizzas per order
- Daily and monthly order trends
- Sales % by category and by size
- Total pizzas sold by category
- Top 5 / Bottom 5 pizzas by revenue, quantity, and orders

Full queries and result sets are in [`PIZZA_SALES_SQL_QUERIES.pdf`](./PIZZA_SALES_SQL_QUERIES.pdf).

## 📁 Repo Contents

| File | Description |
|---|---|
| `pizza_dash.pbix` | Power BI report file — open in Power BI Desktop |
| `pizza_sales.csv` / `pizza_sales_excel_file.xlsx` | Raw source data |
| `PIZZA_SALES_SQL_QUERIES.pdf` | SQL queries + results used to validate every KPI/chart |
| `chart_requirements.png`, `problem_statements.png` | Original business requirements this dashboard was built to satisfy |
| `README.md` | This file |

## 🚀 View the Dashboard

Download `pizza_dash.pbix` and open it in [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads) (free) to explore interactively — or see the screenshots below.

## 🖼️ Preview

**Home Page**
<img width="1586" height="865" alt="Screenshot 2026-08-09 042222" src="https://github.com/user-attachments/assets/78d0702b-6092-4b66-911e-85ab117b10ee" />


**Best/Worst Sellers Page**
<img width="1307" height="1105" alt="Screenshot 2026-08-09 041136" src="https://github.com/user-attachments/assets/e1b1edc6-17ba-4656-8e6e-6e0f14521510" />


