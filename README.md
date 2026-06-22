🚀 Sales Insights Data Analysis (AtliQ Hardware)
📌 Project Overview
This project focuses on analyzing sales data of AtliQ Hardware, a company dealing in computer hardware and peripherals across India.

The goal was to build an interactive Power BI dashboard to help stakeholders track key business metrics and make data-driven decisions instead of relying on manual reporting.

❗ Problem Statement
The Sales Director faced challenges such as:

No centralized dashboard to track performance
Reliance on verbal updates from regional managers
Declining sales with no clear insights into the cause
👉 This project provides a single source of truth for sales performance.

🎯 Objectives
Analyze sales trends across different markets
Identify top-performing customers and products
Track revenue and sales quantity over time
Enable quick and informed decision-making
🛠️ Tools & Technologies
SQL (MySQL) → Data extraction & analysis
Power BI → Dashboard & visualization
Power Query → Data cleaning & transformation
DAX → Calculated measures & KPIs
📂 Dataset Information
The dataset consists of multiple tables:

sales_transactions → Sales data (amount, date, product, market)
sales_customers → Customer details
sales_products → Product information
sales_markets → Market/region data
sales_date → Date hierarchy
🔄 Data Cleaning & Transformation
Removed invalid values (0 or negative sales)
Converted USD transactions into INR
Filtered irrelevant/duplicate records
Built a star schema data model
📊 Data Modeling
A proper relational model was created connecting:

Transactions → Customers
Transactions → Products
Transactions → Markets
Transactions → Date
👉 Ensures efficient and scalable analysis.
