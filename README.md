# E-Commerce-Store-Sales-Power-Bi-Dashboard
This project demonstrates the creation of an interactive Power BI dashboard to analyze and visualize the sales performance of an e-commerce store. The dashboard provides insights into key business metrics, helping decision-makers track sales trends, customer behavior, and product performance.
# E-Commerce Sales Dashboard - Power BI Project

## Project Overview

This project is a **Power BI dashboard** built to analyze and visualize sales data of an e-commerce store. It provides actionable insights into sales performance, product trends, and customer behavior, enabling businesses to make data-driven decisions.

## Data Description

### Orders File

Contains all order-level transactions. Typical columns:

* `Order ID` – Unique identifier for each order
* `Customer ID` – Unique identifier for each customer
* `Order Date` – Date when the order was placed
* `Product` – Name of the product
* `Category` – Product category
* `Quantity` – Number of items purchased
* `Sales Amount` – Revenue from the order
* `Region` – Customer’s region

### Details File

Contains additional information about products or customers (if available). Typical columns may include:

* `Product ID` / `Customer ID` – Unique identifiers for joining with Orders
* `Product Name` – Product details
* `Price` – Unit price of products
* `Customer Info` – Demographic or location details

> The two files are joined in Power BI to enable comprehensive analysis.

## Key Features

* **Sales Analysis:** Track total sales, revenue, and number of orders over time (daily, monthly, yearly).
* **Product Insights:** Identify best-selling products and categories.
* **Customer Analysis:** Analyze repeat customers, new vs returning, and purchase frequency.
* **Time Intelligence:** Compare sales month-over-month and year-over-year.
* **Interactive Dashboard:** Use slicers to filter by category, region, or time period.
* **KPIs:** Monitor metrics like Average Order Value (AOV), total orders, and sales growth.

## Power BI Components

* **Data Modeling:** Define relationships between Orders and Details files.
* **DAX Measures:**

  * `Total Sales` = COUNTROWS(Orders) or SUM([Sales Amount])
  * `Average Orders per Month`
  * `Sales Growth`
* **Visualizations:** Line charts, bar charts, KPIs, tables, and slicers for interactive exploration.
* **Calculated Columns:** Year, Month, or Year-Month for time-based analysis.

## Setup Instructions

1. Open **Power BI Desktop**.
2. Load the `Orders` and `Details` files.
3. Create relationships between files if needed (`Customer ID` or `Product ID`).
4. Create calculated columns for `Year`, `Month`, or `Year-Month` from `Order Date`.
5. Add DAX measures for Total Sales, Average Orders per Month, and other KPIs.
6. Build visuals like line charts, bar charts, and KPIs.
7. Use slicers for dynamic filtering.
8. Save the `.pbix` file and optionally publish to Power BI Service.

## Skills & Tools

* **Tools:** Power BI Desktop
* **Skills:** DAX, Data Modeling, Data Visualization, KPIs, Interactive Dashboards, E-Commerce Analytics

## Outcome

The dashboard enables managers to:

* Monitor monthly and yearly sales trends
* Identify high-performing products and categories
* Understand customer purchase behavior
* Make data-driven decisions for marketing, inventory, and sales strategy
