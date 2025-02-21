# 🚚 Logistics Performance Dashboard - Delhivery Dataset

## 🧀️ Project Overview
This project focuses on developing an **interactive dashboard** to analyze **logistics performance** using the **Delhivery dataset**. The goal is to extract insights on **transport times, route optimization, and delivery performance**, supporting data-driven decision-making.

**Relevance:** Aligns with **Business Analyst (d/m/w) role at AUTO1 Group**, focusing on **logistics performance analysis**.

### 🔗 Resources & Links
- **Google Colab Notebook**: [Colab Link](https://colab.research.google.com/drive/1_ZJ_mHKCUal1ZZCkXEyGBVg6YMZO1PRJ?usp=sharing)
- **Google Sheets Analysis**: [Google Sheets Link](https://docs.google.com/spreadsheets/d/1dhU3fMzNQHpREPe7-ux9AtRWTdQPdg6MQyo7quUI1pc/edit?usp=sharing)
- **Looker Studio Dashboard**: [Looker Studio Link](https://lookerstudio.google.com/reporting/a8f830bf-771f-44d8-8ba4-b48bee7d958f)
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
    - **`trip_creation_time`**: Timestamp when the trip was created  
    - **`route_type`**: Transport type (e.g., FTL)  
    - **`destination_name`**: Name of the destination logistics center  
    - **`actual_time`**: Actual trip duration *(mean: 416.93, max: 4532)*  
    - **`osrm_time`**: Estimated time from OSRM *(mean: 213.87, max: 1686)*  
    - **`delay_factor`**: Ratio of actual time to estimated time *(mean: 2.12, max: 77.39)*  
    - **`trip_duration`**: Total trip time in hours.  
    - **`efficiency_score`**: Distance covered per hour.  
    - **`time_variance`**: Difference between actual & estimated delivery time.  
    - **`route_category`**: Categorized as **Long-haul vs. Short-haul**.  

---

## 📚 Key Insights & Visuals

### 📊 **1. Actual vs. Estimated Travel Time by Route Type (Pivot Table)**
![Actual vs Estimated Travel Time](https://imgur.com/uBTH2mm.png)

**Summary:**
- **FTL routes** have significantly higher travel times than **Carting routes**.
- On average, actual travel times are **longer than OSRM-estimated times** across all route types.
- **FTL deliveries take nearly twice the estimated time**, indicating potential inefficiencies or traffic constraints.

---

### 📊 **2. Top 10 Destination Hubs by Shipment Volume (Pivot Table)**
![Top 10 Destination Hubs](https://imgur.com/NAmCea7.png)

**Summary:**
- The top **10 hubs** handle the highest shipment volumes.
- **Gurgaon_Bilaspur_HB (Haryana)** is the busiest hub with **15,000+ shipments**, followed by **Bangalore_Nelmngla_H (Karnataka)** with **11,000+ shipments**.
- These high-traffic hubs are critical for **logistics efficiency and resource optimization**.

---

### 📊 **3. Average Delay Factor by Route Type (Pivot Table)**
![Average Delay Factor](https://imgur.com/637PmLb.png)

**Summary:**
- **Carting routes have a higher average delay factor (2.4) compared to FTL (2.0)**.
- This suggests **Carting routes may face more operational delays**.
- FTL, despite having longer actual times, is relatively more predictable in delays.

---

### 📊 **4. Delivery Hotspots: Heatmap of Travel Times (Looker Studio)**
![Delivery Hotspots](https://i.imgur.com/XFg3doS.png)

**Summary:**
- A **heatmap visualization** in Looker Studio identifies key delivery hotspots across India.
- **High-density areas** indicate major logistics hubs with **longer travel times**.
- A **route filter** allows differentiation between **FTL and Carting deliveries**.

---

### 📊 **5. Route Efficiency & Delay Analysis (Looker Studio)**
![Route Efficiency & Delay](https://i.imgur.com/HxJxXNP.png)

**Summary:**
- **FTL routes consistently exceed OSRM travel estimates**, indicating inefficiencies.
- A **scatter plot** of actual distances vs. delay factors reveals clustering around **1.6–2.2 delay factor**, suggesting **consistent delays** across certain distances.

---

## 🔍 **Overall Insights & Business Impact**

### **Key Findings:**
- **Delivery times exceed OSRM estimates**, indicating delays across both FTL and Carting routes.
- **High-traffic hubs** like Gurgaon and Bangalore handle the largest shipment volumes, making them **key points for optimization**.
- **Carting routes experience higher delay factors**, suggesting a need for **operational improvements**.
- **The heatmap identifies major delivery hotspots**, revealing areas where logistics performance could be improved.

### **Potential Business Solutions:**
- **Route Optimization:** Adjust routes with high delay factors to improve efficiency.
- **Performance Monitoring:** Implement real-time tracking for key hubs.
- **Operational Improvements:** Reduce bottlenecks in **Carting deliveries**.

---

## 🚀 Project Completion & Conclusion
- **All planned analyses have been successfully conducted**, and insights have been visualized in Looker Studio.
- The **dashboard provides a comprehensive view** of logistics performance, highlighting key areas for **efficiency improvements**.
- **Next Steps:** Further refinement and automation of data updates for real-time monitoring.

✅ **Project Completed!** 🚀
