# 📊 Sales & Business Analytics Dashboard

## 📌 Project Overview

The **Sales & Business Analytics Dashboard** is an interactive Power BI project designed to analyze sales performance, profitability, products, customer segments, and geographic markets.

The dashboard transforms raw sales data into meaningful business insights using **Power Query, DAX, interactive visuals, and slicers**.

---

## 🎯 Project Objectives

- Analyze overall sales and profit performance
- Track monthly sales trends
- Identify top-performing products
- Compare profitability across customer segments
- Analyze sales performance across countries
- Calculate overall profit margin
- Build an interactive business dashboard using Power BI
- Practice Power Query and DAX for business analytics

---

## 📂 Dataset

This project uses Microsoft's **Financial Sample** dataset.

The dataset contains **700 records and 16 columns** related to sales and financial performance.

### Main Columns

- Segment
- Country
- Product
- Discount Band
- Units Sold
- Manufacturing Price
- Sale Price
- Gross Sales
- Discounts
- Sales
- COGS
- Profit
- Date
- Month Number
- Month Name
- Year

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel**
- **Data Visualization**
- **Business Intelligence**

---

## 🔄 Data Preparation

Power Query was used for data preparation and quality checking.

### Data Preparation Steps

- Imported the Financial Sample Excel dataset
- Checked column data types
- Checked for missing values
- Checked for data errors
- Verified numeric and date columns
- Created a `Month Year` field for chronological analysis
- Loaded the cleaned data into the Power BI data model

The dataset was checked using Power Query's column quality features. The inspected columns contained **100% valid values with no visible errors or empty values**.

---

## 🧮 DAX Measures

The following DAX measures were created for the dashboard.

### Total Sales

```DAX

Total Sales = SUM(SalesData[Sales])

Total Profit = SUM(SalesData[Profit])

Total Units Sold = SUM(SalesData[Units Sold])

Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
