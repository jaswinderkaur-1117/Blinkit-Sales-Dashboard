# Blinkit Sales Analysis Dashboard 📊

## Project Overview
This project features a comprehensive **Power BI Dashboard** designed to analyze the sales performance and operational efficiency of **Blinkit** (India’s Last Minute App). The goal was to transform raw retail data into actionable insights for stakeholders, focusing on revenue growth, customer satisfaction, and inventory distribution across various outlet types.

---

## 🚀 Key Features & Insights
The dashboard provides a 360-degree view of the business through the following sections:

* **KPI Tracking:** Real-time visibility into **Total Sales ($1.20M)**, **Average Sales ($141)**, **Inventory Volume (8,523 items)**, and **Customer Ratings (4.0)**.
* **Sales Trends:** Analysis of outlet establishment years, showing a significant growth peak in **2018**.
* **Product Analysis:** Detailed breakdown of sales by **Fat Content** (Low Fat vs. Regular) and **Item Type** (identifying Fruits and Snacks as top earners).
* **Outlet Segmentation:** Comparison of performance across **Tier 1, 2, and 3 cities**, as well as Outlet Size (Small, Medium, High).
* **Interactive Filtering:** A custom sidebar allows users to slice data by Year, Location, and Outlet Size for granular reporting.

---

## 🛠️ Technical Stack
* **Tool:** Power BI Desktop
* **Data Source:** BlinkIT Grocery Data (3,900+ records)
* **DAX (Data Analysis Expressions):** Used for calculating custom measures (Total Sales, Average Ratings, No. of Items).
* **Data Modeling:** Cleaned and structured data to ensure accurate relationships and optimized performance.
* **Design:** Executive-style UI with a professional **Yellow and Dark-Grey** color palette.

---

## 📈 DAX Measures Used
To power the visuals, the following measures were created:

```dax
// Total Sales Calculation
Total Sales = SUM('BlinkIT Grocery Data'[Sales])

// Average Sales per Entry
Average Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

// Total Item Count
No of Items = COUNTROWS('BlinkIT Grocery Data')

// Average Customer Rating
Average Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
