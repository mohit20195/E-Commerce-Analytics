📊 E-Commerce Analytics Dashboard (Excel + SQL)
🔎 Project Overview

This project demonstrates how I used SQL for data extraction and transformation, and Excel for building an interactive analytics dashboard.
The goal is to analyze Orders, Customers, Revenue, Units, and Average Order Value (AOV) to uncover business insights such as:

Monthly revenue trends

Order and unit volumes

Repeat customer rate

Average Order Value (AOV)


🛠 Tools & Technologies

SQL (MySQL / ClassicModels Database) → Data extraction & preprocessing

Excel → Pivot tables, pivot charts and slicers for interactive charts

ODBC Connector → To connect SQL database with Excel


📈 Dashboard Features

✔️ Interactive KPIs: Revenue, Orders, Units, AOV
✔️ Time-series analysis with monthly trends
✔️ Cohort analysis for customer retention
✔️ User-controlled slicers & drop-downs (e.g., by country, product, category)
✔️ Clean and professional design


⚙️ Steps Performed

Extracted data from SQL using queries (joins, aggregations).

Connected MySQL database to Excel via ODBC DSN.

Cleaned & shaped data into tables for analysis.

Built Pivot Tables & Pivot Charts.

Applied Slicers & Dropdown controls for user interaction.

Created a final dashboard summarizing KPIs and trends.


📊 Sample Dashboard Preview

<img width="1306" height="463" alt="image" src="https://github.com/user-attachments/assets/f7732a4c-3a45-4912-b3e0-b649c582902a" />



📜 SQL Example Query
SELECT 
    customernumber,
    country,
    state,
    city,
    COUNT(customernumber) AS NumberOfCustomers
FROM customers
GROUP BY country, state, city;


🎯 Key Learnings

How to integrate SQL with Excel using ODBC

Building interactive dashboards with pivot charts and slicers

Presenting business insights effectively



📬 Contact

👤 Mohit Sharma
📧 mohit20195@gmail.com
