

---

# 🏬 Walmart Superstore Sales Analysis (USA) — Power BI Dashboard

## 📌 Project Objective

To analyze Walmart’s sales performance across the United States and provide actionable insights for managers by evaluating sales, profit, customer segments, regional performance, and future sales trends using interactive Power BI dashboards.



---

## 📊 Dashboards Overview

This project contains **three interactive dashboard pages** with navigation buttons for easy movement across dashboards.

---

## 📈 1. Manager Dashboard

### 🎯 Purpose

Provides high-level business performance metrics for management decision-making.

### ✅ KPIs

* Total Profit
* Total Sales
* Total Quantity Sold
* Average Delivery Days

### 📊 Visuals Used

* Sales by Category (Horizontal Bar Chart)
* Sales by Sub-Category (Horizontal Bar Chart)
* Sales by Customer Segment (Donut Chart)
* Sales by Payment Mode (Donut Chart — COD preferred)
* Monthly & Quarterly Sales Trend (2019 vs 2020)
* Monthly & Quarterly Profit Trend (2019 vs 2020)

### 🔍 Key Insights

* **Phones sub-category generated the highest sales.**
* **Consumer segment contributes the most to total sales.**
* Most customers prefer **Cash on Delivery (COD)**.
* Both **sales and profit increased from 2019 to 2020**, indicating business growth.
* Sales and profit trends are not identical, showing profit is affected by factors beyond sales volume.

---

## 🗺️ 2. Map Visuals — Regional Sales Analysis

### 🎯 Purpose

To analyze geographic sales distribution across U.S. states and regions.

### 📊 Visuals Used

* Interactive USA Map with sales size by state
* Region slicer: Central, East, South, West

### 🔍 Key Insights

* **West region performs best**, mainly driven by **California**.
* **California is the top-selling state** in the dataset.
* Several states like **District of Columbia and Maine have very low sales (below $1,000)** and need business improvement strategies.

---

## 📉 3. Sales Forecasting Dashboard

### 🎯 Purpose

To evaluate historical performance and predict future sales trends.

### 📊 Visuals Used

* Sales & Profit Trend Over Time (Line Chart with Date Hierarchy)
* Sales Forecast using Power BI Forecast feature with zoom slider
* Top States by Sales (Horizontal Bar Chart)

### 🔍 Key Insights

* Overall **sales trend is upward**.
* Forecast shows **good sales initially but slight decline over future periods**.
* **Profit trend does not strictly follow sales trend**, highlighting the need for margin control strategies.

---

## 🧮 DAX Measure Used

```DAX
AvgDelivery = 
DATEDIFF(
    Walmart_superstore_Sales_Dataset[Order Date],
    Walmart_superstore_Sales_Dataset[Ship Date],
    DAY
)
```

---

## 🛠️ Tools & Technologies Used

* Power BI
* Power Query (Data Cleaning & Transformation)
* DAX (Calculated Measures)
* Excel (Initial Data Review)

---

## 📂 Dataset Information

* Source: Kaggle (Walmart Superstore Dataset — Cleaned Version)
* Includes: Sales, Profit, Category, Sub-Category, Region, State, Segment, Payment Mode, Order Date, Ship Date, Quantity.

---

## 💡 Business Recommendations

* Increase focus on **high-performing states like California** to maximize returns.
* Improve logistics and marketing in **low-performing states such as Maine and District of Columbia**.
* Review discount strategies to prevent **profit decline despite sales growth**.
* Continue targeting the **Consumer segment** as it generates the highest revenue.
* Optimize shipping processes to reduce **average delivery time** and improve customer satisfaction.

---

## 📂 Repository Structure

```
📁 Dataset
 └── walmart-Superstore-sales-data-2019-2020.csv

📁 PowerBI_File
 └── walmart Superstore sales analysis.pbix

📁 Screenshots
 ├── Manager Dashboard.png
 ├── Map Visuals.png
 └── Sales Forecasting.png

📄 README.md
```

---


## 🎯 Skills Demonstrated

* KPI Development
* Time Series Analysis
* Sales Forecasting
* Regional Performance Analysis
* Dashboard Design for Business Reporting
* Business Insight Generation


