
# 🌟 Mastering SQL Queries: Unlocking Database Insights

## 📋 Table of Contents:
- [📜 SQL Code](#-sql-code)
- [📖 Explanation](#-explanation)
  - [🔄 USE sql_hr;](#1-use-sql_hr-)
  - [📋 SELECT * FROM employees;](#2-select--from-employees)
  - [📋 SELECT employee_id, first_name, last_name](#3-select-employee_id-first_name_last_name)
- [🗂️ Properties of SQL Keywords](#🗂️-properties-of-sql-keywords)
  - [🗂️ USE](#🗂️-use)
  - [🔍 SELECT](#🔍-select)
  - [🏛️ FROM](#🏛️-from)
- [🚀 Summary](#🚀-summary)

## 📜 SQL Code:
```sql
USE sql_hr;
SELECT * FROM employees;
SELECT employee_id, first_name, last_name FROM employees;
```

## 📖 Explanation:
The provided SQL code performs the following tasks:

### 1. `USE sql_hr;` 🔄
- **Purpose:**
  - This statement switches the context to the `sql_hr` database.
  - All subsequent operations will be performed within the `sql_hr` database unless specified otherwise.
- **Key Points:**
  - It helps organize queries for a specific database.
  - Prevents errors by ensuring that the correct database is being accessed.

### 2. `SELECT * FROM employees;` 📋
- **Purpose:**
  - Retrieves all columns (`*`) and rows from the `employees` table in the `sql_hr` database.
- **Key Points:**
  - `SELECT` is used to specify the data you want to retrieve.
  - `*` is a wildcard symbol, meaning "select all columns".
  - `FROM` specifies the source table (`employees`) where the data is stored.

### 3. `SELECT employee_id, first_name, last_name FROM employees;` 📋
- **Purpose:**
  - Retrieves only the `employee_id`, `first_name`, and `last_name` columns from the `employees` table in the `sql_hr` database.
- **Key Points:**
  - Instead of retrieving all columns, specific columns are selected for clarity and efficiency.
  - This approach improves performance, especially when working with large tables.
  - It allows better control over the data being fetched.

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

---

## 🚀 Summary:
- The code switches to the `sql_hr` database and retrieves all data from the `employees` table.
- **Key keywords** like `USE`, `SELECT`, and `FROM` play vital roles in database operations.
- A more specific query selects only the `employee_id`, `first_name`, and `last_name` columns for better performance and precision.

> ⚡ **Tip:** Use specific column names instead of `*` for better performance and clarity in large databases.
