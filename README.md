# 📊 Sales Data Analysis using SQL, Excel & Power BI  
A complete end-to-end analytics project using **MySQL, SQL queries, data visualization (Excel / Power BI)**, and a structured sales dataset.  
This project focuses on analyzing sales performance, cancellations, returns, and revenue trends across multiple regions, categories, and sales agents.

---

## 🚀 Project Overview

This project performs:

- ✔ Database creation and data import (CSV → MySQL)  
- ✔ SQL analysis on sales trends, cancellations, revenue loss, etc.  
- ✔ Data cleaning and structured querying  
- ✔ Excel/Power BI dashboard visualizations  
- ✔ Insights into customer behavior, category performance, and sales agent ranking  

You can use this project for **portfolio**, **academic assignments**, or **data analytics practice**.

---

## 📁 Project Structure

Sales-Analysis-Project/
│
├── dataset/
│ └── sales_data.csv
│
├── sql/
│ ├── create_table.sql
│ ├── insert_data.sql
│ └── analysis_queries.sql
│
├── dashboard/
│ ├── Excel_Dashboard.xlsx (optional)
│ └── PowerBI_Dashboard.pbix (optional)
│
└── README.md


---

# 📦 Dataset Information

### **Dataset: `sales_data.csv`**  
Contains 30 rows of real-world-like sales data.

| Column Name | Description |
|------------|-------------|
| OrderID | Unique order number |
| OrderDate | Date of order |
| CustomerID | Unique customer code |
| Region | East, West, North, South |
| ProductName | Item purchased |
| Category | Product category |
| Quantity | Units sold |
| UnitPrice | Selling price |
| TotalAmount | Quantity × UnitPrice |
| Status | Completed / Cancelled / Returned |
| SalesPerson | Responsible sales agent |

---

# 🛠️ MySQL Setup

## **1️⃣ Create Database**

```sql
CREATE DATABASE salesdb;
USE salesdb;

# 📊 PART 2 – Excel / Power BI Dashboard

This section focuses on building visual dashboards using **Excel** or **Power BI** based on SQL outputs or the original sales dataset.

---

## 📌 1️⃣ Heatmap: Region vs Category Sales

**Goal:** Identify which regions perform best in each product category.

### Steps (Excel / Power BI)
- Insert a **Pivot Table**
- **Rows:** Region  
- **Columns:** Category  
- **Values:** SUM(Total Sales Amount)  
- Apply **Conditional Formatting → Color Scale**  
- High values = dark/strong color  
- Low values = light color  

This visual quickly highlights strong and weak performing region–category combinations.

---

## 📌 2️⃣ Stacked Bar Chart: Order Status by Region

**Purpose:** Compare the distribution of **Completed, Cancelled, and Returned** orders across regions.

### Steps:
- Create a Pivot Table:
  - **Rows:** Region  
  - **Columns:** Status  
  - **Values:** COUNT(OrderID)
- Insert a **Stacked Bar Chart**

This chart helps identify:
- Regions with high return rates  
- Regions with frequent cancellations  
- Operational or logistic issues  

---

## 📌 3️⃣ Line Chart: Monthly Sales Trend

**Goal:** Identify time-based patterns in completed sales.

### Steps:
- Use SQL Query fo
