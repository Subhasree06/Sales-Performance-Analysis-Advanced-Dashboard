# 📊 Sales Performance Analysis Dashboard (Excel Project)

---

## 🚀 Project Overview

This project demonstrates an end-to-end sales analytics solution built using Microsoft Excel. It includes data cleaning, data modeling, advanced calculations, and forecasting to derive meaningful business insights.

The project transforms raw sales data into an interactive dashboard that supports data-driven decision-making.

---

## 🛠️ Tools & Technologies Used

* Microsoft Excel
* Power Query (Data Cleaning)
* Power Pivot (Data Modeling)
* DAX (Data Analysis Expressions)
* Forecasting (ETS Model)
* Conditional Formatting

---

## 📂 Dataset Description

The project uses three datasets:

### 1. Sales Data

* OrderID
* OrderDate
* CustomerID
* ProductID
* Quantity
* UnitPrice
* TotalSale
* Region

### 2. Products Data

* ProductID
* ProductName
* Category
* Cost

### 3. Customers Data

* CustomerID
* CustomerName
* Region
* Segment

---

## 🔗 Data Modeling

A **Star Schema** was implemented:

* Sales → Products (ProductID)
* Sales → Customers (CustomerID)

This structure improves performance and enables advanced analytics.

---

## 📈 Key DAX Measures

* Total Revenue = SUM(Sales[TotalSale])
* Total Quantity = SUM(Sales[Quantity])
* Total Orders = DISTINCTCOUNT(Sales[OrderID])
* Total Cost = SUMX(Sales, Sales[Quantity] * RELATED(Products[Cost]))
* Profit = [Total Revenue] - [Total Cost]
* Profit % = DIVIDE([Profit], [Total Revenue])

---

## 📊 Dashboard Features

### 🔹 KPI Cards

* Total Revenue
* Profit
* Profit %

### 🔹 Visualizations

* Sales Trend Over Time
* Region-wise Sales
* Top Performing Products

### 🔹 Interactive Filters

* Region
* Category
* Segment

---

## 📉 Forecasting Analysis (NEW 🔥)

Forecasting was performed using Excel’s **Exponential Smoothing (ETS) model**.

### Key Observations:

* Sales show a consistent **upward trend**
* Forecast predicts continued growth in future periods
* Confidence intervals indicate expected value range
* No strong seasonality pattern observed

### Accuracy Metrics:

* Low error values (MAE, RMSE, SMAPE)
* Indicates reliable forecasting model

👉 This helps in predicting future sales and supports business planning.

---

## 🎨 Conditional Formatting (NEW 🔥)

Conditional formatting was used to enhance data visualization:

* Highlighted high and low sales values
* Identified top-performing regions and products
* Improved readability and quick decision-making

👉 This enables users to quickly identify trends and anomalies.

---

## 🔍 Key Insights

* Identified high-performing regions
* Analyzed top-selling products
* Evaluated profitability trends
* Forecasted future sales growth
* Enabled dynamic filtering for better decision-making

---

## 📸 Dashboard Preview

<img width="1339" height="448" alt="Sales Advanced Dashboard" src="https://github.com/user-attachments/assets/ad51c7be-4880-4185-bf2d-61f36af28402" />


---

## 📌 Project Highlights

✔ End-to-end data analytics workflow
✔ Real-world business problem solving
✔ Advanced Excel (Power Query + DAX + Data Model)
✔ Forecasting using ETS model
✔ Interactive and dynamic dashboard

---

## 📄 Project Report

Detailed project report is included in the repository.

---

## 👤 Author

Subhasree B

---

## ⭐ If you like this project, give it a star!

---
