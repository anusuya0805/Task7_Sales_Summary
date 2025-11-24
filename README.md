# Task 7 – Basic Sales Summary using SQLite and Python

## Objective
Use SQL inside Python to extract basic sales summary information such as total quantity sold and total revenue, and visualize the result using a bar chart.

## Tools Used
- Python
- SQLite (sqlite3 module)
- Pandas
- Matplotlib
- Jupyter Notebook

## Steps Performed
1. Created the SQLite database named sales_data.db and inserted sample sales records.
2. Connected Python to SQLite using the following command:
   conn = sqlite3.connect("sales_data.db")
3. Executed the SQL query to calculate total quantity and total revenue per product:
   SELECT product,
          SUM(quantity) AS total_quantity,
          SUM(quantity * price) AS total_revenue
   FROM sales
   GROUP BY product;
4. Loaded the SQL output into a pandas DataFrame using read_sql_query().
5. Displayed the sales summary result using print(df).
6. Plotted a bar chart for revenue per product using matplotlib.
7. Saved the bar chart as sales_chart.png.

## Sample Output
Sales summary displayed in the notebook after executing the SQL query.

## Files Included
- task7.ipynb – Jupyter Notebook with complete code
- sales_data.db – SQLite database
- sales_chart.png – Generated bar chart
## Completion
Task 7 completed using Python and SQLite integration.
