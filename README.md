# Task 7: Basic Sales Summary using MYSQL and Python

## 🎯 Objective
Connect to a SQLite database using Python and analyze sales data to calculate total quantity sold and revenue for each product. Visualize the results using a bar chart.

## 🧰 Tools Used
- Python
- MySql
- pandas
- matplotlib

## 🔍 SQL Query Used
```sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
```

## 📊 Output
- A table showing `product`, `total_qty`, and `revenue`
- A bar chart visualizing revenue by product

## 📁 Files Included
- `task 7 DA.ipynb` – Jupyter Notebook with Python code and output
- `sales_data.db` – SQLite database file containing sales data
- `sales_chart.png` – Revenue bar chart visualization

## ✅ Summary
This task demonstrates the ability to:
- Use SQL inside Python using the `MYSql` module
- Perform basic data analysis using `pandas`
- Visualize aggregated sales data using `matplotlib`
