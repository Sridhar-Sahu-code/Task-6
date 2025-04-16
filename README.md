# 🍕 Pizza Sales SQL Analysis

This project explores monthly trends in pizza sales using SQL queries applied to the `pizza_sales.csv` dataset. It includes analysis of revenue, order volume, and filtering by time ranges.

---

## 📦 Dataset Structure

Key columns from `pizza_sales.csv`:

- `order_id`: Unique identifier for each order
- `order_date`: Date the order was placed (format: "01 January 2015")
- `unit_price`: Price per unit
- `total_price`: Line total (unit_price × quantity)
- `quantity`: Number of pizzas ordered

---

## 🧠 SQL Tasks

This project covers the following operations:

---

### a. Extract Month from `order_date`

```sql
SELECT 
  EXTRACT(MONTH FROM TO_DATE(order_date, 'DD Month YYYY')) AS month
FROM pizza_sales;
