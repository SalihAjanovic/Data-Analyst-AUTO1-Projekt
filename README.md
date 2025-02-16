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

start_scan_to_end_scan: Duration from the start to the end scan

is_cutoff: Indicator for cutoff occurrence

cutoff_factor: Factor associated with cutoff

cutoff_timestamp: Timestamp of the cutoff event

actual_distance_to_destination: Measured distance to the destination

actual_time: Actual trip duration

osrm_time: Estimated time from OSRM (Open Source Routing Machine)

osrm_distance: Estimated distance from OSRM

factor: Ratio of actual to estimated time

segment_actual_time: Actual time for a trip segment

segment_osrm_time: Estimated time for a trip segment

segment_osrm_distance: Estimated distance for a trip segment

segment_factor: Ratio of actual to estimated time for a trip segment

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

