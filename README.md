# 🏬 Store Sales Dashboard – Power BI Project (Historical Trend Analysis)

## 📌 Project Overview

This Power BI project aims to contribute to the success of a fictional retail store by leveraging **data analysis techniques**, with a special focus on understanding **historical performance trends**. The dashboard provides insights into sales, profit, delivery times, and regional performance — helping decision-makers monitor operations and strategize effectively.

> **Disclaimer:** The dataset used is **not from a real business store**. It was sourced from the internet purely for **educational and learning purposes**.

---

## 🎯 Project Objectives

- Analyze sales and profit trends over time (**no forecasting was performed**).
- Use Power BI to create a professional, interactive business dashboard.
- Understand delivery efficiency and customer preferences using data.
- Empower decision-making using regional, categorical, and temporal insights.

---

## 📁 Dataset Description

The dataset used is named **`SuperStore_Sales_Dataset.csv`**. It includes order-level data that covers:

- **Order and Shipping Details**: `Order Date`, `Ship Date`, `Ship Mode`
- **Sales Information**: `Sales`, `Profit`, `Quantity`
- **Product Classification**: `Category`, `Sub-Category`
- **Customer Segmentation**: `Segment` (e.g., Consumer, Corporate)
- **Geographical Data**: `State`, `Region`
- **Payment Modes**: Includes options such as COD, Online, and Cards

This rich dataset allows for **trend analysis** across different months and categories, along with regional comparisons.

---

## 🧹 Data Preparation & Cleaning

Steps performed before building the dashboard:

- ✅ Changed **data types** (e.g., dates for `Order Date`, numeric for `Sales`, `Profit`)
- ✅ **Removed empty columns** that had no analytical value
- ✅ Created a new **calculated column**:
  - `Average Delivery Days` using DAX:  
    ```DAX
    DATEDIFF([Order Date], [Ship Date], DAY)
    ```
- ✅ Checked for and avoided unnecessary duplicates or formatting errors
- ✅ Established proper **relationships** for accurate filtering and aggregations

---

## ⚙️ Power BI Workflow

### 🔹 1. Data Import
- Loaded the dataset into **Power BI Desktop**.

### 🔹 2. Data Modeling
- Applied transformations and DAX formulas.
- Ensured consistency in relationships and column formats.

### 🔹 3. Visualizations
The dashboard features multiple charts and visuals:

- 📊 **Sales by Category and Sub-Category**
- 📈 **Monthly Sales and Profit Trends (2019 vs. 2020)**
- 🚚 **Average Delivery Days** KPI
- 💳 **Sales by Payment Mode**
- 👥 **Sales by Segment (e.g., Consumer, Corporate)**
- 🌍 **Map Visualization**:
  - A **bubble map** showing **sum of sales by state** (bubble size represents sales volume)

### 🔹 4. Interactivity
- 🧭 **Region Slicer** added for filtering data by region: Central, East, South, and West

---

## 🧠 Key Business Insights

The dashboard helps the business store understand:

- 🏆 **Top Categories**: Office Supplies led in sales, followed by Technology and Furniture
- 🔍 **Best-Performing Sub-Categories**: Phones, Chairs, and Binders
- 🧾 **Delivery Efficiency**: Average delivery time across orders is **4 days**
- 📅 **Monthly Trends**: November and December saw the highest spikes in sales
- 🧭 **Regional Trends**: Easily identify sales strengths and gaps across regions using the **map**
- 💰 **Customer Preferences**:
  - **COD** is the most popular payment mode (~43%)
  - **Consumers** make up the largest customer segment (~48%)

These insights help in **targeted marketing, optimizing delivery logistics, and enhancing operational strategy**.

---

## 🔄 Project Flow

### ✅ Upstream (Input)
- Structured CSV dataset
- Light cleaning and column enrichment

### 📊 Downstream (Output)
- Interactive dashboard featuring:
  - Time-based performance tracking
  - Category and regional breakdowns
  - KPI visualizations

---

## 🛠️ Tools Used

- Microsoft Power BI Desktop  
- DAX (Data Analysis Expressions)  
- Microsoft Excel (for preliminary inspection)

---

## 🖼️ Dashboard Preview

> 📎 Check the `Store Dashboard new.pdf` in this repository to view a snapshot of the final dashboard layout and visuals.

---


---
