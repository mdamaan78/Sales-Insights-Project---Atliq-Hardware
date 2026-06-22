# 🚀 Sales Insights Data Analysis (AtliQ Hardware)

## 📌 Project Overview

This project focuses on analyzing sales data of **AtliQ Hardware**, a company dealing in computer hardware and peripherals across India.

The goal was to build an interactive **Power BI dashboard** to help stakeholders track key business metrics and make data-driven decisions instead of relying on manual reporting.

---

## ❗ Problem Statement

The Sales Director faced challenges such as:

- No centralized dashboard to track performance
- Reliance on verbal updates from regional managers
- Declining sales with no clear insights into the cause

👉 This project provides a single source of truth for sales performance.

---

## 🎯 Objectives

- Analyze sales trends across different markets
- Identify top-performing customers and products
- Track revenue and sales quantity over time
- Enable quick and informed decision-making

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------------|------------------------------|
| **SQL (MySQL)** | Data extraction & analysis |
| **Power BI** | Dashboard & visualization |
| **Power Query** | Data cleaning & transformation |
| **DAX** | Calculated measures & KPIs |

---

## 📂 Dataset Information

The dataset consists of multiple tables:

- **sales_transactions** → Sales data (amount, date, product, market)
- **sales_customers** → Customer details
- **sales_products** → Product information
- **sales_markets** → Market/region data
- **sales_date** → Date hierarchy

---

## 🔄 Data Cleaning & Transformation

- Removed invalid values (0 or negative sales)
- Converted USD transactions into INR
- Filtered irrelevant and duplicate records
- Standardized data formats
- Built a star schema data model

---

## 📊 Data Modeling

A proper relational model was created connecting:

- Transactions → Customers
- Transactions → Products
- Transactions → Markets
- Transactions → Date

👉 Ensures efficient and scalable analysis.

---

## 📌 Data Model

![Data Model](data-model.png)

---

## 📈 Dashboard Features

### 📊 KPIs

- 💰 **Total Revenue:** ₹985M
- 📦 **Total Sales Quantity:** 2M

### 📉 Visualizations

- Revenue by Market
- Sales Quantity by Market
- Revenue Trend (Time Series)
- Top 5 Customers by Revenue
- Top 5 Products by Revenue

### 🎛️ Filters

- Year Slicer
- Month Slicer

---

## 📌 Dashboard Preview

![Dashboard](dashboard.png)

---

## 🔍 Key Insights

- Delhi NCR generates the highest revenue.
- Low-performing markets were identified for improvement.
- A small number of customers and products contribute the majority of revenue (Pareto Principle).
- Seasonal fluctuations are visible in revenue trends.

---

## 📊 DAX Measures Used

```DAX
Revenue = SUM(sales_amount)

Sales Quantity = SUM(sales_qty)

Revenue LY =
CALCULATE(
    [Revenue],
    SAMEPERIODLASTYEAR('Date'[Date])
)

Profit Margin % =
DIVIDE([Profit], [Revenue], 0)
```

---

## 💡 Business Impact

- Eliminates manual reporting
- Provides real-time business insights
- Helps identify growth opportunities
- Supports faster, data-driven decision-making

---

## 🚀 Skills Demonstrated

- SQL Querying
- Data Cleaning & Transformation
- Data Modeling
- ETL Process
- Power Query
- DAX Calculations
- KPI Development
- Dashboard Design
- Business Intelligence
- Data Visualization

---

## 📁 Project Files

```
Sales-Insights-Project
│
├── Atliq_Hardware_Sales_Data_Analysis.pbix
├── dashboard.png
├── data-model.png
└── README.md
```

---

## ⭐ Conclusion

This project showcases an end-to-end Business Intelligence workflow—from SQL data extraction and cleaning to Power BI dashboard development and DAX calculations. The final dashboard enables stakeholders to monitor KPIs, identify trends, and make faster, data-driven business decisions.

---

## 🙌 Support

If you found this project useful, consider giving it a ⭐ on GitHub!
