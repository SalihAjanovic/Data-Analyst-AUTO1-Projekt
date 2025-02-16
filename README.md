🚚 Logistics Performance Dashboard - Delhivery Dataset

🛠️ Project Overview

This project focuses on developing an interactive dashboard to analyze logistics performance using the Delhivery dataset.
The goal is to derive insights regarding transport times, route optimization, and delivery performance to support data-driven decision-making.

Relevance:
The project aligns with the requirements of the Business Analyst position (d/m/w) at AUTO1 Group, especially in logistics performance analysis.

🗂️ Dataset Description

Dataset: Delhivery Logistics Dataset (from Kaggle)

Content: Logistics data including transport types, routes, delivery times, and performance metrics.

Source: Kaggle

Size: 144,867 records

Structure:

data: Identifies whether the data is for training or testing

trip_creation_time: Timestamp when the trip was created

route_schedule_uuid: Unique ID for route scheduling

route_type: Transport type (e.g., FTL)

trip_uuid: Unique ID for each trip

source_center: Code for the source logistics center

source_name: Name of the source logistics center

destination_center: Code for the destination logistics center

destination_name: Name of the destination logistics center

od_start_time: Start time of the trip

od_end_time: End time of the trip

start_scan_to_end_scan: Duration from the start to the end scan (numeric, with values ranging from 20 to 7898)

is_cutoff: Indicator for cutoff occurrence (True/False)

cutoff_factor: Factor associated with cutoff (mean: 232.93, max: 1927)

cutoff_timestamp: Timestamp of the cutoff event

actual_distance_to_destination: Measured distance to the destination (mean: 234.07, max: 1927.45)

actual_time: Actual trip duration (mean: 416.93, max: 4532)

osrm_time: Estimated time from OSRM (mean: 213.87, max: 1686)

osrm_distance: Estimated distance from OSRM (mean: 284.77, max: 2326.19)

factor: Ratio of actual to estimated time (mean: 2.12, max: 77.39)

segment_actual_time: Actual time for a trip segment (mean: 36.19, max: 3051)

segment_osrm_time: Estimated time for a trip segment (mean: 18.50, max: 1611)

segment_osrm_distance: Estimated distance for a trip segment (mean: 22.83, max: 2191.40)

segment_factor: Ratio of actual to estimated time for a trip segment (mean: 2.21, max: 574.25)

🎯 Project Goal

Develop a dashboard to provide real-time insights into logistics performance.

Identify bottlenecks and areas for improvement.

Create management reports to support strategic decisions.

🔍 Methodology

Data Preparation:

Clean and structure the dataset using SQL in Google Colab.

Handle missing values, duplicates, and outliers.

Apply transformations for analysis in pivot tables.

Analysis & Insights:

SQL queries for metric calculations.

Python (pandas, matplotlib) for data exploration.

Pivot tables in Excel for deeper insights.

Dashboard Development:

Create an interactive dashboard in Looker Studio.

Include filters for transport type, route, and time period.

⚙️ Tools & Technologies

Data Analysis: SQL (SQLite in Google Colab)

Programming: Python (pandas, matplotlib, numpy)

Data Visualization: Looker Studio

Development Environment: Google Colab

Additional Tools: Excel (for pivot tables)

📊 Planned Analyses & Metrics

Transport Time Analysis: Average delivery time by route/region.

Route Optimization: Identify inefficient routes.

Delay Analysis: Frequency and causes of delivery delays.

Cost Efficiency: Identify optimization potential through route adjustments.

🚀 Progress & Results



📈 Sample Insights (placeholder)

(Add screenshots or graphs here after initial analysis.)

🔗 Resources & Links

Kaggle Dataset

Project Dashboard (to be added after completion)

GitHub Repository

💡 Next Steps:

Clean and preprocess the dataset in Google Colab.

Create SQL queries for key performance metrics.

Develop pivot tables in Excel.

Build an interactive dashboard in Looker Studio.

🖊️ Note:This project was developed as part of an application for the Business Analyst (d/m/w) position at AUTO1 Group.

