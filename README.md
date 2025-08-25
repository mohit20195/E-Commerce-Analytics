# 📊 E-Commerce Analytics Dashboard (Power BI + SQL)

## 🔎 Project Overview  
This project demonstrates how I used **SQL** for data extraction and transformation, and **Power BI** for building an interactive business intelligence dashboard.  

The goal is to analyze **Orders, Customers, Revenue, Units, and Average Order Value (AOV)** to generate actionable insights, such as:  

- Revenue & order trends over time  
- Repeat customer behavior & retention  
- Cohort analysis of customer engagement  
- KPIs for business performance monitoring  

---

## 🛠 Tools & Technologies
- **SQL (MySQL / ClassicModels Database)** → Data extraction & preprocessing  
- **Power BI Desktop** → Data modeling, DAX measures, and dashboard creation  
- **ODBC Connector** → To connect SQL database with Power BI  

---

## 📈 Dashboard Features
✔️ **KPI Cards**: Revenue, Orders, Units, AOV  
✔️ **Trend Analysis**: Monthly revenue & orders with drilldowns  
✔️ **Cohort Heatmap**: Customer retention by cohort month  
✔️ **Customer Segmentation**: New vs repeat customers  
✔️ **Interactive Filters**: Slicers for country, product category, and time period  
✔️ **Time Intelligence** using custom Date table (DAX)  

---

## ⚙️ Steps Performed
1. **Extracted** raw data from SQL using joins & aggregations.  
2. **Connected** Power BI to MySQL via ODBC.  
3. **Created Date Table** for proper time intelligence in DAX.  
4. Built **DAX Measures** for Revenue, Orders, AOV, Repeat Rate.  
5. Designed **multiple report pages**:  
   - **Page 1:** KPIs & New vs Returning Revenue  
   - **Page 2:** Top 10 Customers & Products  
   - **Page 3:** RFM Pie Chart & Table and Revenue by Country on Map
   - **Page 4:** Cohort Heatmap  
6. Published the interactive dashboard design.  

---

## 📊 Sample Dashboard Preview

**Page 1: KPIs & New vs Returning Revenue**

<img width="752" height="449" alt="image" src="https://github.com/user-attachments/assets/1c9f1978-f32a-4d1a-bd1d-b5dfd68af00a" />

**Page 2: Page 2: Top 10 Customers & Products**

<img width="764" height="421" alt="image" src="https://github.com/user-attachments/assets/613770be-3514-4fbb-94ad-38e3ebafa49c" />

**Page 3: RFM Pie Chart & Table and Revenue by Country on Map**

<img width="754" height="433" alt="image" src="https://github.com/user-attachments/assets/1dbe195a-aed1-4dc5-a647-878d80869c1d" />

**Page 4: Cohort Heatmap**

<img width="597" height="393" alt="image" src="https://github.com/user-attachments/assets/485d999f-4a96-4695-b767-fa88901dd35d" />


---

## 📜 Example DAX Measures
```DAX
Date = CALENDARAUTO()

---

## 📜 Example SQL Query
```sql
SELECT 
    c.country, 
    o.orderDate, 
    COUNT(o.orderNumber) AS total_orders, 
    SUM(od.quantityOrdered * od.priceEach) AS revenue
FROM orders o
JOIN customers c ON o.customerNumber = c.customerNumber
JOIN orderdetails od ON o.orderNumber = od.orderNumber
GROUP BY c.country, o.orderDate
ORDER BY o.orderDate;

---

## 🎯 Key Learnings

Connecting SQL to Power BI with ODBC

Creating DAX measures and date tables for time intelligence

Building cohort analysis in Power BI

Designing interactive dashboards for decision-making

---

## 📬 Contact

👤 Mohit Sharma
📧 mohit20195@gmail.com

