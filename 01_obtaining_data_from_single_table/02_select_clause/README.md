
# 🌟 The Select Clause

## 📋 Table of Contents:
- [📜 SQL Code](#-sql-code)
- [📖 Explanation](#-explanation)
  - [🔄 USE sql_store;](#1-use-sql_store-)
  - [📋 SELECT customer_id, first_name, last_name, city, points](#2-select-customer_id-first_name_last_name_city_points)
  - [🆕 SELECT with Alias (AS)](#3-select-with-alias-as)
- [🗂️ Properties of SQL Keywords](#%EF%B8%82%EF%B8%8F-properties-of-sql-keywords)
  - [🗂️ USE](#%EF%B8%82%EF%B8%8F-1-use)
  - [🔍 SELECT](#-2-select)
  - [🏛️ FROM](#%F0%9F%8F%9B%EF%B8%8F-3-from)
  - [🏷️ Alias (AS)](#%F0%9F%8F%B7%EF%B8%8F-alias-as)
- [🚀 Summary](#-summary)

## 📜 SQL Code:
```sql
USE sql_store;
SELECT customer_id, first_name, last_name, city, points, (points+100) AS new_points FROM customers;
```

## 📖 Explanation:
The provided SQL code performs the following tasks:

### 1. `USE sql_store;` 🔄
- **Purpose:**
  - This statement switches the context to the `sql_store` database.
  - All subsequent operations will be performed within the `sql_store` database unless specified otherwise.
- **Key Points:**
  - It helps organize queries for a specific database.
  - Prevents errors by ensuring that the correct database is being accessed.

### 2. `SELECT customer_id, first_name, last_name, city, points` 📋
- **Purpose:**
  - Retrieves specific columns (`customer_id`, `first_name`, `last_name`, `city`, and `points`) from the `customers` table in the `sql_store` database.
- **Key Points:**
  - Using specific column names improves query efficiency.
  - Only the required data is fetched, making it more performance-friendly for large datasets.

### 3. `SELECT with Alias (AS)` 🆕
- **Purpose:**
  - Adds a computed column (`points+100`) and labels it as `new_points` using the alias keyword (`AS`).
- **Key Points:**
  - **Alias (`AS`)** is used to rename a column or table for better readability.
  - Computations can be performed directly within the `SELECT` clause.
  - The result is displayed with the alias name (`new_points`).

---

## 🗂️ Properties of SQL Keywords:

### 🗂️ 1. `USE`
- Switches the database context to the specified database.
- Ensures that all subsequent SQL commands refer to the correct database.
- Prevents the need to specify database names in every query.

### 🔍 2. `SELECT`
- Used to retrieve data from a database.
- Can be customized to retrieve specific columns, rows, or computed values.
- Common clauses paired with `SELECT` include:
  - `WHERE` for filtering rows.
  - `GROUP BY` for grouping rows.
  - `ORDER BY` for sorting results.

### 🏛️ 3. `FROM`
- Specifies the table(s) from which to retrieve data.
- Can be paired with:
  - `JOIN` to combine data from multiple tables.
  - Subqueries to provide additional data sources.

### 🏷️ Alias (`AS`)
- Used to assign a temporary name to a column or table.
- **Purpose:**
  - Improves readability of the result set.
  - Simplifies reference to computed columns or complex expressions.
- **Example:**
  - `(points+100) AS new_points` creates a new column `new_points` based on the computation.

---

## 🚀 Summary:
- The code switches to the `sql_store` database and retrieves selected data from the `customers` table.
- **Key keywords** like `USE`, `SELECT`, `FROM`, and `AS` play vital roles in making queries efficient and readable.
- Aliases (`AS`) enhance clarity by providing meaningful labels to computed or complex columns.

> ⚡ **Tip:** Use aliases to make complex queries easier to understand and maintain.

