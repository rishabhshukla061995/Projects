# EDA-FedEx-Logistics-Performance-Analysis

# FedEx Logistics Performance Analysis

## Project Overview

This project performs an Exploratory Data Analysis (EDA) on a FedEx Logistics dataset to uncover patterns, identify bottlenecks, and provide insights for improving delivery timelines, reducing costs, and enhancing overall operational efficiency. The analysis covers various aspects of logistics operations, including purchase orders, shipment methods, vendor agreements (INCO terms), delivery schedules, and product details.

## Problem Statement

The analysis aims to address several key questions:

1.  Delivery performance comparison by managing teams (e.g., PMO - US).
2.  Impact of shipment mode (air, sea, etc.) on meeting scheduled delivery dates.
3.  Delivery delays by country.
4.  Frequency of on-time deliveries by shipment mode.
5.  Vendor Lead Time and Delivery Performance.
6.  Impact of INCO term type on vendor delivery performance.
7.  Relationship between shipment weight and insurance costs.

## Business Objective

With the rise of eCommerce and global shipments, the business objective is to optimize logistics operations by identifying bottlenecks, monitoring vendor and carrier performance, optimizing delivery routes, and minimizing delays. The goal is to make data-driven decisions to ensure reliable, timely, and cost-effective FedEx services.

## Dataset

The dataset used for this analysis is the `SCMS_Delivery_History_Dataset.csv`, which contains details of various logistics operations, including:

*   Purchase order information
*   Shipment details (mode, weight, cost, insurance)
*   Dates (PO sent, scheduled delivery, delivered)
*   Product information (description, dosage, dosage form)
*   Vendor and manufacturing site details
*   Geographical information (Country)

## Exploratory Data Analysis (EDA)

The EDA process involved:

*   Loading and inspecting the dataset.
*   Handling missing values (imputation for numerical and categorical columns).
*   Converting relevant columns to appropriate data types ('Weight (Kilograms)', 'Freight Cost (USD)' to numeric).
*   Identifying and addressing potential outliers.
*   Analyzing the distribution of key variables (e.g., Line Item Quantity, Weight, Freight Cost).
*   Exploring relationships between variables through various visualizations.

## Key Findings & Insights

Based on the EDA and visualizations, some key findings include:

*   Most shipments are relatively light and in smaller quantities, but there are significant outliers in terms of weight, quantity, and freight cost.
*   'Air' and 'Truck' are the most frequent shipment modes, while 'Ocean' shipments experience the longest average delays.
*   There is significant variability in delivery delays by country, with some countries experiencing much higher average delays than others.
*   Air and Air Charter are generally more expensive per kilogram than Truck and Ocean.
*   There is a strong positive correlation between 'Line Item Value' and 'Line Item Insurance (USD)'.
*   The distribution of shipments by country and vendor highlights key markets and supplier relationships.
*   Overall monthly shipment volume shows an increasing trend with fluctuations.

## Recommendations

Based on the analysis, the following recommendations are suggested:

1.  **Optimize Shipment Mode Selection:** Implement a data-driven framework to select the most efficient mode based on urgency, cargo characteristics, and destination.
2.  **Implement Freight Cost Control Measures:** Benchmark costs, negotiate contracts, and monitor trends to reduce variability and inefficiencies.
3.  **Strengthen Inventory and Order Planning:** Improve forecasting and consolidate orders to avoid high-cost emergency shipments.
4.  **Monitor High-Risk Shipment Patterns:** Investigate outliers in high-cost or delayed shipments to identify and address underlying issues.
5.  **Enhance Vendor and Country Performance Monitoring:** Focus efforts on countries and vendors identified with higher average delays.

## Conclusion

The EDA provides valuable insights into FedEx's logistics operations, highlighting areas for optimization in terms of cost, timeliness, and efficiency. By leveraging these findings, FedEx can make informed decisions to improve performance, enhance customer satisfaction, and achieve business objectives.
