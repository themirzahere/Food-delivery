# 🧠 Smart SQL Filtering: Multi-Condition Query Optimization

## 📌 Project Overview
This project demonstrates practical SQL query skills by solving a multi-layered real-world problem. The dataset represents a raw `orders` table, and the task was to extract meaningful insights using advanced filtering and sorting techniques.

---

## 🛠️ Tech Stack
- **Language:** SQL
- **Platform:** CodeChef Learn (SQL Module)
- **Tools:** MySQL / PostgreSQL (syntax compatible)

---

## 🎯 Problem Statement
You are provided with an `orders` table. Your goal is to:
- Identify customers who live in **pincode 122001 or 122002**
- Filter orders that were placed **before 12:30 PM**
- Find customers residing on the **3rd floor or higher**

---

## 🔍 Key Concepts Used
- Conditional filtering with `AND` / `OR`
- Time-based filtering using numerical format
- `LIKE` operator for pattern matching
- NULL handling with `IS NULL`
- Sorting using `ORDER BY`
- Aggregations and DISTINCT values

---

## 💡 Sample Query
```sql
SELECT customer_name  
FROM orders  
WHERE (address_pincode = 122001 OR address_pincode = 122002)  
  AND order_time < 12.3  
  AND apartment_floor >= 3;
