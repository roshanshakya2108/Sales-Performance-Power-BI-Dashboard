# 📊 Power BI Sales Performance Dashboard

This project presents a **Sales Performance Dashboard** built using **Microsoft Power BI**, designed to visualize and analyze sales data from two related tables — `Orders` and `Details`.  
The dashboard provides actionable insights into sales, profit, customer behavior, and regional performance.

---

## 🧾 Dataset Overview

The dataset consists of two main tables:

### **Details Table**
| Column Name | Description |
|--------------|--------------|
| Amount | Total sale amount |
| Category | Product category |
| Order ID | Unique identifier for each order |
| PaymentMode | Mode of payment used |
| Profit | Profit earned from the sale |
| Quantity | Quantity of items sold |
| Sub-Category | Specific product sub-category |

### **Orders Table**
| Column Name | Description |
|--------------|--------------|
| City | City where the order was placed |
| CustomerName | Name of the customer |
| Order Date | Date when the order was placed |
| Order ID | Unique identifier for each order |
| State | State of the customer |

---

## 🔗 Data Model

A **one-to-many relationship** is established between:

This relationship ensures accurate aggregation of sales and profit data across customer and regional dimensions.

---

## 📈 Dashboard Features

### 💡 KPIs
- **Total Sales (Amount)**
- **Total Profit**
- **Total Quantity Sold**
- **Total Orders**
- **Profit Margin %**
- **Average Order Value**

### 📊 Visuals
- **Sales by Category** — Bar Chart  
- **Profit by Sub-Category** — Column Chart  
- **Sales by Payment Mode** — Donut Chart  
- **Sales Trend Over Time** — Line Chart  
- **Sales by State** — Filled Map  
- **Top 10 Customers by Sales** — Bar Chart  

### 🎛️ Interactive Elements
- Slicers for **State**, **Category**, and **Order Date**  

---

## 🧮 DAX Measures

```DAX
Total Sales = SUM(Details[Amount])
Total Profit = SUM(Details[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
Total Orders = DISTINCTCOUNT(Orders[Order ID])
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

## 🎨 Design Highlights
- Clean, minimal layout with **KPI cards** at the top  
- **Interactive filters** and **tooltips** for dynamic insights  
- **Consistent color palette** and responsive visuals  

---

## 🛠️ Tools & Technologies
- **Power BI**  
- **DAX (Data Analysis Expressions)**  
- **Data Modeling**  
- **Data Visualization**  

---

## 📸 Dashboard Preview
<img width="1164" height="650" alt="image" src="https://github.com/user-attachments/assets/6eea1022-9930-491d-a0d1-17f571c548da" />

