# 📘 SQL Resume Project – Online Bookstore Analysis

SQL project completed as part of hands-on learning and portfolio building for Data Analyst roles.

---

## 📘 Project - Online Bookstore Analysis

### 📁 Files Included
- `Data analysis using SQL.sql`: SQL script for database creation, data import, and analysis
- `Books.csv`: Book details dataset
- `Customers.csv`: Customer information dataset
- `Orders.csv`: Order transactions dataset
- `SQL Project Questions.pdf`: Business problem statements

---

### 📌 SQL Concepts Covered
- `CREATE DATABASE`, `CREATE TABLE`, `DROP TABLE`
- Data import using `COPY`
- `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY`
- Aggregate functions: `SUM`, `AVG`, `COUNT`
- `JOINS` (INNER JOIN, LEFT JOIN)
- `HAVING`, `DISTINCT`, `LIMIT`
- Handling NULLs using `COALESCE`

---

### 📊 Key Analysis Performed

#### 🔹 Basic Queries
- Retrieve books by genre (e.g., Fiction)
- Filter books published after a specific year
- Identify customers by country
- Analyze orders within a date range
- Calculate total stock and revenue
- Find most expensive and least stocked books

#### 🔹 Advanced Queries
- Total books sold per genre
- Average price by category (Fantasy)
- Customers with multiple orders
- Most frequently ordered books
- Top spending customers
- Remaining stock after fulfilling orders

---

### 🚀 Sample Query

```sql
-- Find the customer who spent the most on orders
SELECT 
    c.Customer_ID, 
    c.Name, 
    SUM(o.Total_Amount) AS Total_Spent
FROM Orders o
JOIN Customers c 
    ON o.Customer_ID = c.Customer_ID
GROUP BY c.Customer_ID, c.Name
ORDER BY Total_Spent DESC 
LIMIT 1;
```

---

### 📌 Connect
Let’s connect on [LinkedIn](https://www.linkedin.com/in/swaraj-borhade-921a411a4/)  
📧 borhadeswaraj01@gmail.com
