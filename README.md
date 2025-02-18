# 🚚 Logistics Performance Dashboard - Delhivery Dataset

## 🛠️ Project Overview
This project focuses on developing an **interactive dashboard** to analyze **logistics performance** using the **Delhivery dataset**. The goal is to extract insights on **transport times, route optimization, and delivery performance**, supporting data-driven decision-making.

**Relevance:** Aligns with **Business Analyst (d/m/w) role at AUTO1 Group**, focusing on **logistics performance analysis**.

### 🔗 Resources & Links
- **Google Colab Notebook**: [Colab Link](https://colab.research.google.com/drive/1_ZJ_mHKCUal1ZZCkXEyGBVg6YMZO1PRJ?usp=sharing)
- **Dataset Source**: [Delhivery Logistics Dataset - Kaggle](https://www.kaggle.com/datasets/devarajv88/delhivery-logistics-dataset/data)

---

## 🎯 Project Goal

- Develop a dashboard to provide real-time insights into logistics performance.  
- Identify bottlenecks and areas for improvement.  
- Create management reports to support strategic decisions.

---

## 🗂️ Dataset Description

**Dataset:** Delhivery Logistics Dataset *(from Kaggle)*  
- **Content:** Logistics data including transport types, routes, delivery times, and performance metrics.  
- **Source:** [Delhivery Logistics Dataset - Kaggle](https://www.kaggle.com/datasets/devarajv88/delhivery-logistics-dataset/data)  
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
    - **`start_scan_to_end_scan`**: Duration from the start to the end scan *(numeric, with values ranging from 20 to 7898)*  
    - **`is_cutoff`**: Indicator for cutoff occurrence *(True/False)*  
    - **`cutoff_factor`**: Factor associated with cutoff *(mean: 232.93, max: 1927)*  
    - **`cutoff_timestamp`**: Timestamp of the cutoff event  
    - **`actual_distance_to_destination`**: Measured distance to the destination *(mean: 234.07, max: 1927.45)*  
    - **`actual_time`**: Actual trip duration *(mean: 416.93, max: 4532)*  
    - **`osrm_time`**: Estimated time from OSRM *(mean: 213.87, max: 1686)*  
    - **`osrm_distance`**: Estimated distance from OSRM *(mean: 284.77, max: 2326.19)*  
    - **`factor`**: Ratio of actual to estimated time *(mean: 2.12, max: 77.39)*  
    - **`segment_actual_time`**: Actual time for a trip segment *(mean: 36.19, max: 3051)*  
    - **`segment_osrm_time`**: Estimated time for a trip segment *(mean: 18.50, max: 1611)*  
    - **`segment_osrm_distance`**: Estimated distance for a trip segment *(mean: 22.83, max: 2191.40)*  
    - **`segment_factor`**: Ratio of actual to estimated time for a trip segment *(mean: 2.21, max: 574.25)*  
    - **`trip_duration`**: Total trip time in hours.  
    - **`efficiency_score`**: Distance covered per hour.  
    - **`time_variance`**: Difference between actual & estimated delivery time.  
    - **`delay_factor`**: Ratio of actual time to estimated time.  
    - **`route_category`**: Categorized as **Long-haul vs. Short-haul**.  

## 📚 Key Insights
- **Average trip duration:** ~16 hours.
- **Efficiency score:** ~0.54 (distance covered per hour).
- **Delay factor:** Deliveries take **twice as long as estimated**.
- **Routes with highest delays:** Carting routes have **more delays** than FTL.
- **Busiest hubs:** Certain logistics centers handle **significantly more shipments**, requiring optimized resource allocation.

---

## 📊 Dashboard & Analysis Plan
- **Data Cleaning & Preparation:** SQL (Google Colab), handling missing values, outliers, and transformations.
- **Analysis & Insights:** SQL queries, Python (pandas, matplotlib), Excel pivot tables.
- **Dashboard Development:** Looker Studio with filters for transport type, routes, and time periods.

---

## ⚙️ Tools & Technologies

- **Data Analysis:** SQL (SQLite in Google Colab)  
- **Programming:** Python (pandas, matplotlib, numpy)  
- **Data Visualization:** Looker Studio  
- **Development Environment:** Google Colab  
- **Additional Tools:** Excel (for pivot tables)  

---

## 📊 Planned Analyses & Metrics

- **Transport Time Analysis:** Average delivery time by route/region.  
- **Route Optimization:** Identify inefficient routes.  
- **Delay Analysis:** Frequency and causes of delivery delays.  
- **Cost Efficiency:** Identify optimization potential through route adjustments.  

---

## 💡 Next Steps
- [x] Import & clean dataset  
- [x] Generate SQL-based insights  
- [ ] Develop pivot tables in Excel  
- [ ] Create Looker Studio dashboard  
- [ ] Document final insights  

---

**📚 Note:** This project was created as part of an application for the **Business Analyst (d/m/w) position at AUTO1 Group**.
"""
