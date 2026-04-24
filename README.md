# 📊 Sales Performance Analysis Dashboard (Excel Project)

---

## 🚀 Project Overview

This project demonstrates an end-to-end sales analytics solution built using Microsoft Excel. It covers data cleaning, data modeling, and business analysis using advanced Excel tools like Power Query, Power Pivot, and DAX.

The goal of this project is to transform raw sales data into meaningful insights and build an interactive dashboard for decision-making.

---

## 🛠️ Tools & Technologies Used

* Microsoft Excel
* Power Query (Data Cleaning)
* Power Pivot (Data Modeling)
* DAX (Data Analysis Expressions)

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

This enables efficient querying and advanced calculations.

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

* KPI Cards:

  * Total Revenue
  * Profit
  * Profit %

* Visualizations:

  * Sales Trend Over Time
  * Region-wise Sales
  * Top Performing Products

* Interactive Filters (Slicers):

  * Region
  * Category
  * Segment

---

## 🔍 Key Insights

* Identified high-performing regions
* Analyzed top-selling products
* Evaluated profitability trends
* Enabled dynamic filtering for better decision-making

---

## 📸 Dashboard Preview

<img width="1339" height="448" alt="Sales Advanced Dashboard" src="https://github.com/user-attachments/assets/62253940-7fe6-42f1-92cc-49698a72ee0b" />


---

## 📌 Project Highlights

✔ End-to-end data analytics workflow
✔ Real-world business problem solving
✔ Hands-on with Power Query, Data Modeling & DAX
✔ Interactive dashboard design

---

## 📄 Project Report

Detailed report is available in the repository.

---

## 👤 Author

Subhasree B

---

## ⭐ If you like this project, give it a star!

---
