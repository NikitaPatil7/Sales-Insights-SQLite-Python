# Sales-Insights-SQLite-Python
This basic project demonstrates how to use SQL within Python to analyze and visualize sales data from a local SQLite database. Includes basic SQL queries, pandas integration, and matplotlib charts.

# SQLite Sales Summary

This is a beginner-friendly Python project that demonstrates how to use **SQL inside Python** to analyze sales data stored in a local **SQLite database**. It also includes basic data visualization using **Matplotlib**.

---

## Project Overview

**Objective:**  
- Connect to an SQLite database
- Run SQL queries to summarize sales
- Load the results into a pandas DataFrame
- Display the results using `print()`
- Plot a simple bar chart showing revenue per product

---

## Tools & Libraries Used

- Python 3.x
- SQLite (via `sqlite3`)
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Files Included

| File | Description |
|------|-------------|
| `sales_data.db` | SQLite database file with sample sales records |
| `Sales_Analysis_SQLite_Python.ipynb` | Jupyter Notebook containing the code for analysis and visualization |


---

## Sample SQL Query Used

```sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
