# 🚚 Logistics Performance Dashboard - Delhivery Dataset

## 🧀️ Project Overview
This project focuses on developing an **interactive dashboard** to analyze **logistics performance** using the **Delhivery dataset**. The goal is to extract insights on **transport times, route optimization, and delivery performance**, supporting data-driven decision-making.

**Relevance:** Aligns with **Business Analyst (d/m/w) role at AUTO1 Group**, focusing on **logistics performance analysis**.

### 🔗 Resources & Links
- **Google Colab Notebook**: [Colab Link](https://colab.research.google.com/drive/1_ZJ_mHKCUal1ZZCkXEyGBVg6YMZO1PRJ?usp=sharing)
- **Google Sheets Analysis**: [Google Sheets Link](https://docs.google.com/spreadsheets/d/1dhU3fMzNQHpREPe7-ux9AtRWTdQPdg6MQyo7quUI1pc/edit?usp=sharing)
- **Dataset Source**: [Delhivery Logistics Dataset - Kaggle](https://www.kaggle.com/datasets/devarajv88/delhivery-logistics-dataset/data)

---

## 🎯 Project Goal

- Develop a dashboard to provide **real-time insights** into logistics performance.  
- Identify **bottlenecks and inefficiencies** in delivery operations.  
- Generate **data-driven management reports** to optimize route planning.  

---

## 📊 Dashboard & Analysis Plan
- **Data Cleaning & Preparation:** SQL (Google Colab), handling missing values, outliers, and transformations.
- **Analysis & Insights:** SQL queries, Python (pandas, matplotlib), Google Sheets pivot tables.
- **Dashboard Development:** Looker Studio with filters for transport type, routes, and time periods.

---

## ⚙️ Tools & Technologies

- **Data Analysis:** SQL (SQLite in Google Colab)  
- **Programming:** Python (pandas, matplotlib, numpy)  
- **Data Visualization:** Looker Studio  
- **Development Environment:** Google Colab  
- **Additional Tools:** Excel, Google Sheets (for pivot tables)  

---

## 📊 Planned Analyses & Metrics

- **Transport Time Analysis:** Average delivery time by route/region.  
- **Route Optimization:** Identify inefficient routes.  
- **Delay Analysis:** Frequency and causes of delivery delays.  
- **Cost Efficiency:** Identify optimization potential through route adjustments.  

---

## 💂️ Dataset Description

**Dataset:** Delhivery Logistics Dataset *(from Kaggle)*  
- **Content:** Logistics data including transport types, routes, delivery times, and performance metrics.  
- **Size:** 144,867 records  
- **Structure:**  
    - **`data`**: Identifies whether the data is for training or testing  
    - **`trip_creation_time`**: Timestamp when the trip was created  
    - **`route_schedule_uuid`**: Unique ID for route scheduling  
    - **`route_type`**: Transport type (e.g., FTL)  
    - **`trip_uuid`**: Unique ID for each trip  
    - **`source_center`**: Code for the source logistics center  
    - **`source_name`**: Name of the source logistics center  
    - **`destination_center`**: Code for the destination logistics center  
    - **`destination_name`**: Name of the destination logistics center  
    - **`od_start_time`**: Start time of the trip  
    - **`od_end_time`**: End time of the trip  
    - **`actual_time`**: Actual trip duration *(mean: 416.93, max: 4532)*  
    - **`osrm_time`**: Estimated time from OSRM *(mean: 213.87, max: 1686)*  
    - **`delay_factor`**: Ratio of actual time to estimated time *(mean: 2.12, max: 77.39)*  
    - **`trip_duration`**: Total trip time in hours.  
    - **`efficiency_score`**: Distance covered per hour.  
    - **`time_variance`**: Difference between actual & estimated delivery time.  
    - **`route_category`**: Categorized as **Long-haul vs. Short-haul**.  
    - **`segment_actual_time`**: Actual time for each segment of the trip.  
    - **`segment_osrm_time`**: Estimated OSRM time for each segment.  
    - **`segment_osrm_distance`**: Estimated OSRM distance per segment.  
    - **`segment_factor`**: Ratio of actual to estimated time for segments.  

---

## 📚 Key Insights & Visuals

### 📊 **1. Actual vs. Estimated Travel Time by Route Type**
![Actual vs Estimated Travel Time](https://yourimagehosting.com/image1.png)

**Summary:**
- **FTL routes** have significantly higher travel times than **Carting routes**.
- On average, actual travel times are **longer than OSRM-estimated times** across all route types.
- **FTL deliveries take nearly twice the estimated time**, indicating potential inefficiencies or traffic constraints.

---

### 📊 **2. Top 10 Destination Hubs by Shipment Volume**
![Top 10 Destination Hubs](https://yourimagehosting.com/image2.png)

**Summary:**
- The top **10 hubs** handle the highest shipment volumes.
- **Gurgaon_Bilaspur_HB (Haryana)** is the busiest hub with **15,000+ shipments**, followed by **Bangalore_Nelmngla_H (Karnataka)** with **11,000+ shipments**.
- These high-traffic hubs are critical for **logistics efficiency and resource optimization**.

---

### 📊 **3. Average Delay Factor by Route Type**
![Average Delay Factor](https://yourimagehosting.com/image3.png)

**Summary:**
- **Carting routes have a higher average delay factor (2.4) compared to FTL (2.0)**.
- This suggests **Carting routes may face more operational delays**.
- FTL, despite having longer actual times, is relatively more predictable in delays.

---

## 💡 Next Steps
- [x] Import & clean dataset  
- [x] Generate SQL-based insights  
- [x] Develop pivot tables in Google Sheets  
- [ ] Create Looker Studio dashboard  
- [ ] Document final insights  

---

**📚 Note:** This project was created as part of an application for the **Business Analyst (d/m/w) position at AUTO1 Group**.
