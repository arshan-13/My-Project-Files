 Asmon Electronics – Monthly Sales Growth Analysis Project

An end-to-end data analysis project covering data cleaning, transformation, database storage, and interactive visualization for Asmon Electronics' sales data. The project demonstrates a complete data pipeline using **Python, MySQL, and Power BI**.

## Project Overview

The goal of this project was to analyze raw sales transaction data for Asmon Electronics, clean and process it programmatically, store it in a relational database, and build an interactive Power BI dashboard to track monthly sales growth, profitability, and regional/product performance.

## Tech Stack

| Tool | Purpose |
|------|---------|
| **Python (Pandas)** | Data cleaning, transformation, feature engineering |
| **SQLAlchemy + MySQL** | Storing cleaned data in a relational database |
| **Power BI** | Building interactive dashboards and visualizations |
| **Excel/CSV** | Raw data source and intermediate exports |

## Workflow

### 1. Data Cleaning & Preparation (Python)
- Loaded raw sales data (`sales_raw_500.csv`) containing 500+ transaction records with fields like Order ID, Order Date, Customer, Region, Product, Sales, and Cost.
- Removed duplicate records using `drop_duplicates()`.
- Converted `Order_Date` to proper datetime format and dropped rows with invalid/missing dates.
- Engineered new features for deeper analysis:
  - **Profit** = Sales − Cost
  - **Year** and **Month** extracted from Order Date for time-based trend analysis.
- Exported the cleaned dataset for downstream use.

### 2. Database Integration (MySQL)
- Connected to a MySQL database using **SQLAlchemy**.
- Loaded the cleaned dataset into a `sales_data` table, enabling structured storage and the ability to query the data using SQL for further analysis or reporting.

### 3. Dashboard & Visualization (Power BI)
- Connected Power BI to the processed sales data.
- Built an interactive dashboard to visualize:
  - Monthly and yearly sales growth trends
  - Profit margins across products and regions
  - Top-performing products and customer regions
  - KPI cards summarizing total sales, profit, and order volume

## Key Insights
- Identified month-over-month sales growth patterns to highlight peak sales periods.
- Compared profitability across product categories (Mobile, Laptop, Monitor, Printer, etc.).
- Surfaced regional performance differences to support targeted business strategy.

## Project Files
- `sales_raw_500.csv` — Raw input dataset
- `Python_File_of_Project.ipynb` — Data cleaning and MySQL integration script
- `Asmon_Electronics_Monthly_Sales_Growth_Analysis_Project.pbix` — Power BI dashboard

## Skills Demonstrated
- Data cleaning and preprocessing with Pandas
- Feature engineering for time-series and profitability analysis
- Database connectivity and data loading with SQLAlchemy/MySQL
- Dashboard design and DAX-based visualization in Power BI
- End-to-end data pipeline thinking (raw data → clean data → database → insights)

---
**Author:** Mohammed Arshan H E
📧 mohdarshan1326@gmail.com | 🔗 [LinkedIn](https://www.linkedin.com/in/mohammedarshan1326/)
