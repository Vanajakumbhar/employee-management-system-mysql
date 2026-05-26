# SQL Relational Database Project

## Overview
A relational database project demonstrating core SQL concepts including 
table design, data manipulation, and advanced querying techniques 
using MySQL.

## Database Structure
- Designed 5+ normalized tables with Primary Keys and Foreign Keys
- Enforced referential integrity using constraints
- Applied proper data types and column definitions

## SQL Concepts Covered

### Joins
- INNER JOIN — fetch matching records across tables
- LEFT JOIN — include all records from left table
- RIGHT JOIN — include all records from right table

### Data Manipulation (DML)
- INSERT — add new records
- UPDATE — modify existing records
- DELETE — remove records
- ALTER — modify table structure

 Querying & Filtering
- WHERE, AND, OR conditions
- GROUP BY — group records for aggregation
- HAVING — filter grouped results
- ORDER BY — sort results ascending/descending

 Aggregate Functions
- SUM(), COUNT(), AVG(), MAX(), MIN()

 Constraints
- PRIMARY KEY — unique identifier for each record
- FOREIGN KEY — enforce relationships between tables
- NOT NULL, UNIQUE

 Sample Queries

```sql
-- Total sales by category using GROUP BY and HAVING
SELECT category, SUM(amount) AS total_sales
FROM sales
GROUP BY category
HAVING SUM(amount) > 1000
ORDER BY total_sales DESC;

-- Customer orders using JOIN
SELECT c.customer_name, o.order_id, o.order_date, o.amount
FROM customers c
INNER JOIN orders o ON c.customer_id = o.customer_id;

-- Update a record
UPDATE products
SET price = 299
WHERE product_id = 101;
```

 Tools Used
- MySQL
- SQL (DDL + DML)
- VS Code / MySQL Workbench

 Skills Demonstrated
SQL | MySQL | Joins | GROUP BY | HAVING | Aggregate Functions |
Primary Key | Foreign Key | Data Manipulation | Query Optimization
