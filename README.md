# 🍕 Pizza Sales SQL Analysis

This project involves analyzing sales data for a pizza company using SQL. The dataset contains details about customer orders, including order time, pizza types, sizes, quantities, and prices. The goal is to extract actionable business insights through structured queries, KPIs, and trend analysis.

---

## 📁 Dataset

The dataset used is a single table named `pizza_sales` containing the following columns:

- `order_id`
- `order_date`
- `order_time`
- `pizza_name`
- `pizza_category`
- `pizza_size`
- `quantity`
- `total_price`

> 📌 Note: The dataset is assumed to be pre-cleaned and ready for analysis.

---

## 📊 Key Performance Indicators (KPIs)

1. **Total Revenue**
   ```sql
   SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;
   ```

2. **Average Order Value**
   ```sql
   SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_ord_value FROM pizza_sales;
   ```

3. **Total Pizzas Sold**
   ```sql
   SELECT SUM(quantity) AS Total_pizza_sold FROM pizza_sales;
   ```

4. **Total Orders**
   ```sql
   SELECT COUNT(DISTINCT order_id) AS Total_orders FROM pizza_sal_
