# 🚖 Ride-Hailing Supply & Demand Dashboard

## 📌 Project Overview
This project simulates a **Supply & Demand analysis** for a ride-hailing company. It analyzes over **600,000 rides** to identify surge pricing patterns, high-demand locations, and weather impacts on ride volume.

The goal was to build a scalable BI solution that helps Operations Managers optimize driver allocation during peak hours.

## 📊 Dashboard Preview
![Dashboard Overview]([dashboard_overview_page1.png](https://github.com/arefeh-a/drive-supply-demand-analysis/tree/main/dashboard_overview))


## 🛠 Tech Stack & Skills
* **Power BI Desktop**: Data modeling, visualization, and reporting.
* **DAX (Data Analysis Expressions)**: Complex measures for time intelligence and conditional logic.
* **Star Schema**: Designed a normalized data model for performance optimization.
* **ETL**: Cleaned and transformed Unix timestamps using Python/Pandas before loading.

## 🧠 Key Business Insights
1.  **Surge Pricing Logic**: Correlated `Surge Multipliers` with specific weather conditions (Rain vs. Clear) and "Day of Week" peaks.
2.  **Geospatial Analysis**: Mapped Source vs. Destination flows to identify "Commuter Routes."
3.  **Demand Heatmap**: Built a matrix to pinpoint the "Golden Hours" (Friday/Saturday 18:00-23:00) where revenue is highest.

## 📐 Data Model (Star Schema)
I constructed a Star Schema to ensure high performance on large datasets:
* **Fact Table**: `Rides` (600k+ rows)
* **Dimension Tables**: `Calendar`, `Weather`, `Location`
* **Relationships**: 1-to-Many relationships utilizing a custom `Date-Hour` key for cross-analyzing weather patterns.

## 🚀 How to Run
1.  Download the `Supply_Demand_Analysis.pbix` file.
2.  Open in Power BI Desktop.
3.  Explore the interactive filters (Vehicle Type, Source, Weather).
