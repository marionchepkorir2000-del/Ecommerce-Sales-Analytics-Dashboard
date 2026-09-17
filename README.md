# E-Commerce Sales & Analytics Dashboard

## Project Overview
This repository contains end-to-end data analysis and interactive dashboards created in Google Sheets to evaluate e-commerce sales performance, customer purchasing trends, marketing ROI, and order fulfillment efficiency.

---

## Project 1: Baseline Sales & Marketing Performance

### Overview & KPIs
An initial deep dive into transactional sales data to establish core business performance metrics and customer purchasing patterns.
* **Total Revenue:** $1,264,761.96
* **Total Orders:** 1,200
* **Total Unique Customers:** 1,189

## 📊 Key Exploratory Data Analysis (EDA) Findings

* **Fulfillment & Operational Health:** 41% of total orders were either cancelled or returned, highlighting a critical area to optimize inventory availability, shipping reliability, and post-purchase customer experience.
* **Customer Retention & Repeat Purchase:** Only 11 out of 1,189 customers placed repeat orders, signaling a major opportunity to implement targeted retention strategies, post-sale engagement, and loyalty programs.
* **Multi-Year Revenue Trend:** Overall revenue experienced a downward trend, dropping from ~$552.6K in 2023 to ~$231.9K in 2025, warranting further analysis into product pricing, churn, and market demand shift.
* **Acquisition Channel Performance:** Instagram proved to be the top-performing referral channel, driving the highest revenue share at approximately $275.3K.
* **Seasonality & Peak Demand:** June emerged as the strongest month across the analyzed timeframe, generating both the highest order volume and peak monthly revenue.

## Project 2: Advanced Operations & Promotional Analysis

### Overview & Focus Areas
An expanded analysis evaluating operational delivery health, coupon promotional effectiveness, and channel attribution modeling.
* **Fulfillment & Order Tracking:** Detailed breakdown across **Delivered**, **Pending**, and **Cancelled** order states to isolate delivery bottlenecks and improve operational efficiency.
* **Promotional Discount Impact:** Evaluated coupon usage and discount depth to measure conversion lift versus profit margin impact.
* **Workbook Modules:** Organized into structured tabs including `RAWDATA`, `CLEANEDDATA`, `SALESANALYSIS`, `ORDERSTATUSANALYSIS`, `PRODUCTANALYSIS`, `COUPONANALYSIS`, `MARKETING ANALYSIS`, `CUSTOMER ANALYSIS`, and `DASHBOARD`.

---

## Data Cleaning & Validation Rules

To ensure high data quality and accuracy across both projects, all datasets underwent structured cleaning in Google Sheets:

* **Duplicate Removal:** Identified and removed duplicate entries using unique order IDs to prevent skewed metrics.
* **Missing Value Treatment:** Imputed missing values in categorical fields (`PaymentMethod`, `OrderStatus`) and added default placeholders for missing coupon codes.
* **Format Standardization:** Unified all transaction dates to `YYYY-MM-DD`, converted price fields to standard currency (`$ USD`), and normalized text casing across product names and referral sources.
* **Data Validation:** Applied custom dropdown validation rules on status and payment fields to prevent invalid entries.
* **Calculated Fields:** Derived Gross Revenue (`Quantity` × `UnitPrice`) and calculated order-level aggregation flags across all rows.

---

## Tools Used
* **Google Sheets:** Data cleaning, pivot tables, lookup formulas, and interactive dashboard design.
* **Data Visualization:** Bar charts, horizontal breakdown charts, and summary metric cards.
