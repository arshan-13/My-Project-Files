## Madhav E-Commerce Sales Analysis Project

An end-to-end e-commerce data analysis project covering data cleaning, transformation, and interactive dashboard creation to analyze sales, profit, and customer ordering behavior for an online retail business.

## Project Overview

The goal of this project was to analyze e-commerce order and transaction data, clean and structure it in Excel, and build an interactive Power BI dashboard to uncover sales trends, profitability by category, regional performance, and customer payment preferences — supporting data-driven business decisions.

## Tech Stack

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Data cleaning, transformation, and merging of raw datasets |
| **Power BI** | Data modeling, DAX measures, and dashboard visualization |

## Dataset

The project uses two related datasets joined on **Order ID**:

- **Orders.csv** (500+ records): Order ID, Order Date, Customer Name, State, City
- **Details.csv** (1,500+ records): Order ID, Amount, Profit, Quantity, Category, Sub-Category, Payment Mode

Combined, the dataset covers orders across **19 states**, **3 main product categories** (Electronics, Furniture, Clothing) spanning **17 sub-categories**, and **5 payment modes** (Credit Card, Debit Card, EMI, UPI, COD).

## Workflow

### 1. Data Cleaning & Transformation (Excel)
- Loaded the raw Orders and Details datasets into Excel.
- Cleaned inconsistencies in date formats, customer names, and category labels.
- Verified and standardized the **Order ID** field as the common key between both datasets to enable a reliable join in Power BI.
- Prepared the cleaned files for import into Power BI.

### 2. Data Modeling & Dashboard Design (Power BI)
- Imported the cleaned Orders and Details tables into Power BI and built a relationship between them using **Order ID**.
- Created **DAX measures** to calculate key metrics such as total sales, total profit, profit margin, and average order value.
- Designed **KPI cards** summarizing overall sales and profit performance.
- Built interactive visualizations including:
  - Sales and profit trends over time
  - Category and sub-category performance breakdown
  - State/city-level geographic analysis
  - Payment mode distribution
- Added **slicers** (Category, State, Payment Mode) and **drill-through reports** for deeper, on-demand analysis.

## Key Insights
- Identified top-performing product categories and sub-categories by sales and profit margin.
- Highlighted states and cities driving the highest order volumes.
- Surfaced customer payment mode preferences to inform checkout/payment strategy.
- Enabled drill-through analysis from high-level KPIs down to individual order details.

## Project Files
- `Orders.csv` — Raw order-level data (customer, date, location)
- `Details.csv` — Raw transaction-level data (amount, profit, category, payment mode)
- `Madhav_Ecom_Sales_Analysis_Report.pbix` — Power BI report with data model, DAX measures, and dashboards

## Skills Demonstrated
- Data cleaning and preparation in Excel
- Relational data modeling (joining multiple tables) in Power BI
- DAX measure creation for business KPIs
- Interactive dashboard design with slicers and drill-through
- Translating raw transactional data into actionable e-commerce business insights

---
**Author:** Mohammed Arshan H E
📧 mohdarshan1326@gmail.com | 🔗 [LinkedIn](https://www.linkedin.com/in/mohammedarshan1326/)# My-Project-Files
