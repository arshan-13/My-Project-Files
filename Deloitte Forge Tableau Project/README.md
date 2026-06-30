## Daikibo Telemetry Machine Data Analysis

An end-to-end IoT telemetry analysis project that transforms raw JSON sensor data from Daikibo Manufacturing's global factories into an interactive Tableau dashboard for monitoring machine health and equipment performance.

## Project Overview

Daikibo Manufacturing operates factories across multiple countries, with thousands of connected machines (CNC machines, welders, presses, drills, furnaces, etc.) continuously streaming telemetry data. The goal of this project was to clean and structure this raw JSON telemetry data, load it into a usable format, and build a Tableau dashboard to identify unhealthy machines across factories, device types, and locations — enabling predictive maintenance insights.

## Tech Stack

| Tool | Purpose |
|------|---------|
| **JSON** | Raw telemetry data source from IoT-connected machines |
| **Microsoft Excel** | Data cleaning, transformation, and restructuring |
| **Tableau** | Dashboard design, calculated fields, and visualization |

## Dataset

The raw dataset (`daikibo-telemetry-data.json`) contains **160,000+ telemetry records** from connected machines across 3 countries and 4 factories:

- **Countries:** Japan, China, Germany
- **Factories:** daikibo-factory-meiyo, daikibo-factory-seiko, daikibo-shenzhen, daikibo-berlin
- **Device Types:** CNC, AirWrench, Furnace, LaserWelder, LaserCutter, MetalPress, SpotWelder, ConveyorBelt, HeavyDutyDrill
- **Fields per record:** Device ID, Device Type, Timestamp, Location (Country, City, Area, Factory, Section), Status (healthy/unhealthy), Temperature

## Workflow

### 1. Data Cleaning & Transformation (Excel)
- Loaded the nested JSON telemetry data and flattened it into a structured tabular format.
- Extracted and organized key fields: Device ID, Device Type, Timestamp, Location hierarchy (Country → City → Area → Factory → Section), Status, and Temperature.
- Cleaned the dataset to ensure consistency in categorical fields (device types, status values, location names) before loading into Tableau.

### 2. Dashboard Design (Tableau)
- Connected the cleaned dataset to Tableau.
- Built **calculated fields** to quantify machine health:
  - An `Unhealthy` measure that flags records where `status = "unhealthy"` (assigns a value of 10, else 0), enabling easy aggregation of unhealthy machine counts.
- Designed multiple worksheets analyzing:
  - Machine status (healthy vs. unhealthy) by **Factory** and **Device Type**
  - Geographic breakdown by **Country, City, Area, and Section**
  - **Temperature trends** across devices and timestamps
- Combined worksheets into an interactive dashboard with filtering by Factory, Device Type, and Status for drill-down analysis.

## Key Insights
- Identified which factories and device types had the highest concentration of unhealthy machine readings.
- Enabled location-level drill-down (Country → Factory → Section) to pinpoint problem areas within the manufacturing network.
- Surfaced temperature patterns that may correlate with machine health status, supporting predictive maintenance planning.

## Project Files
- `daikibo-telemetry-data.json` — Raw IoT telemetry dataset (160,000+ records)
- `Book1.twb` — Tableau workbook containing data source connections, calculated fields, and dashboard sheets

## Skills Demonstrated
- Working with nested/raw JSON data and flattening it for analysis
- Data cleaning and transformation using Excel
- Building calculated fields and custom measures in Tableau
- Designing multi-dimensional dashboards (device, location, time, status)
- Translating raw IoT sensor data into actionable business/maintenance insights

---
**Author:** Mohammed Arshan H E
📧 mohdarshan1326@gmail.com | 🔗 [LinkedIn](https://www.linkedin.com/in/mohammedarshan1326/)
