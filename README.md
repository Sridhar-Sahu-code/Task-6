# 🍕 Pizza Sales SQL Analysis

A hands-on SQL project analyzing pizza sales using a dataset containing order and pricing details. This repo focuses on extracting business insights like monthly revenue and order volume.

---

## 📊 Dataset Overview

This analysis is based on `pizza_sales.csv`, which contains the following key columns:

- `order_id`: Unique identifier for each order
- `order_date`: The date the order was placed (e.g., "01 January 2015")
- `unit_price`: Price per pizza unit
- `total_price`: Total price for the line item (unit_price × quantity)
- `quantity`: Number of pizzas in the line item

---

## ✅ SQL Analysis Objectives

We perform the following SQL operations:

### a. Extract Month
We extract the **month** from `order_date` using:

```sql
EXTRACT(MONTH FROM TO_DATE(order_date, 'DD Month YYYY')) AS month
