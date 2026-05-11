# ✈️ Flights Delay & Cancellation Analysis Dashboard (Power BI)
Data-driven insights into flight delays and cancellations, powered by SQL + Power BI

## 📌 Overview
This project provides a comprehensive analysis of flight delays and cancellations using SQL Server for data modeling and Power BI for visualization.
It transforms raw flight data into structured dimensions and fact tables, enabling root cause analysis and performance monitoring across airlines and airports.


---

## 🛠️ Data Model
- **Fact_Flights**: Central fact table containing flight records, delays, and cancellations.  
- **Dimensions**:  
  - `Dim_Date` – Calendar attributes (Year, Month, Day, Week, Weekend flag)  
  - `Dim_Airlines` – Airline reference data  
  - `Dim_Airports` – Airport reference data  
  - `Dim_Cancellation_Codes` – Cancellation reason mapping  
  - `Dim_Month` – Month-level aggregation support  

---

## 📊 Dashboard Features
- **Summary KPIs**: Total Flights, Total Delay Minutes, Average Delay Minutes, % Delayed  
- **Top 5 Delayed Airlines & Airports**: Ranked visuals by delay minutes  
- **Delay Reasons Breakdown**: Late Aircraft, Airline, Air System, Weather, Security  
- **Busiest Airports**: Flight volume comparison across major hubs  
- **Trends Over Time**: Monthly line charts for delays and flight counts  
- **Route-Level Analysis**: Origin–Destination pairs with flight counts and average delay minutes  
- **Cancellation Insights**: Controllable vs. Uncontrollable categories, with Arrival/Departure status  
- **Root Cause Visualization**: Stacked bar charts showing delay reasons by airport  

---

## 🎯 Purpose
- Identify **operational bottlenecks** and external factors driving delays/cancellations  
- Support **airline performance monitoring** and **airport efficiency analysis**  
- Provide **actionable insights** for reducing delays, improving scheduling, and enhancing passenger experience  

---

## 🚀 Getting Started
### Prerequisites
- **SQL Server** (2019 or later recommended)  
- **Power BI Desktop** (latest version)  

### Steps
1. Load SQL scripts into your SQL Server instance to build dimensions, fact tables, and views.  
2. Import datasets (`flights.xlsx`, `airlines.xlsx`, `airports.xlsx`, `cancellation_codes.xlsx`) into the database.  
3. Open the Power BI file (`Flight Delay & Cancellation Performance.pbix`) and connect it to your SQL database.  
4. Refresh the model to populate visuals with live data.  

---

## 📌 Notes
- Dataset currently covers **2015 flight records**.  
- Scripts are modular and can be extended to additional years.  
- Dashboard is optimized for **root cause analysis** but can be adapted for real-time monitoring.  

---

## ✨ Tagline
*“Data-driven insights into flight delays and cancellations, powered by SQL + Power BI.”*
