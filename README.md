# Credit Card Financial Analytics Dashboard (Power BI)

## Project Overview

This project features a comprehensive, two-page interactive Power BI business intelligence dashboard designed to analyze credit card financial data from dual perspectives: transactions and customers. 

Processing over 1 million transactions and evaluating ₹55M in total revenue alongside ₹45M in transaction volumes, the dashboard converts raw relational datasets into an executive-ready interface for monitoring spending trends, customer demographics, and revenue drivers.

The architecture is divided into two target-focused report pages:

* **CC Transactions Report:** Focuses on expenditure categories, card tier performance, and quarterly transaction trends.

* **CC Customer Report:** Focuses on customer demographic profiling, income segmentations, geographic penetration, and customer satisfaction metrics.

## Business Objective

The project aims to diagnose portfolio performance to drive optimization for credit card product positioning and marketing strategy by:

* Identifying high-value card categories and customer segments driving the largest share of revenue.

* Tracking quarterly revenue trajectories and transaction volume baseline variations (Q1–Q4).

* Understanding the direct impact of consumer demographics (age, occupation, education, marital status) on spending behavior.

* Providing data-driven insights to optimize customer targeting and risk-segmentation strategies.

## Dashboard Features

### Page 1: CC Transactions Report

* **Executive KPI Snapshot:** High-visibility cards monitoring core financial health: Revenue (**₹55M**), Transaction Amount (**₹45M**), Total Interest Earned (**₹8M**), and Total Volume (**1M** transactions).

* **Card Performance Matrix:** Breakdown of revenue distribution across product tiers: Blue (**₹46M**), Silver (**₹6M**), Gold (**₹2M**), and Platinum (**₹1M**).

* **Expenditure Allocation:** Category-wise revenue tracking across primary spend buckets: Bills (**₹14M**), Entertainment (**₹10M**), Fuel (**₹9M**), Grocery (**₹9M**), Food (**₹8M**), and Travel (**₹6M**).

* **Quarterly Volume & Trend Analysis:** A dual-axis line-and-bar combo chart mapping quarterly revenue performance alongside transaction density (averaging ~164K transactions/quarter).

* **Payment Method Segmentation:** High-level overview of revenue generation by usage channel: Swipe (**₹35M**), Chip (**₹17M**), and Online (**₹3M**).

* **Cross-Filter Infrastructure:** Integrated Gender (M/F) and Card Type slicers for immediate on-the-fly data discovery.

### Page 2: CC Customer Report

* **Customer Health KPIs:** High-level summaries tracking Total Revenue (**₹55M**), Total Interest (**₹8M**), Aggregate Customer Income (**₹576M**), and Customer Satisfaction Score (**3.19/5 CSS**).

* **Weekly Revenue Trajectory:** Time-series analysis modeling weekly revenue trends (Jan–Oct 2023), highlighting cyclical variations between ₹0.38M and ₹0.77M.

* **Demographic Age Banding:** Comparative analysis revealing the 40–50 age bracket as the highest revenue driver, yielding over **₹25M** across genders.

* **Occupational Revenue Share:** Breakdown by profession: Businessman (**₹17M**), White-collar (**₹10M**), and Self-employed (**₹8M**).

* **Geographic Top 5 States:** Performance rankings across top revenue-generating territories: TX, NY, CA, FL, and NJ, with TX and NY leading at ₹6M–₹7M each.

* **Socio-Economic Segmentations:** Layered visualizations analyzing revenue by Marital Status (Married: **₹26M** vs. Single: **₹22M**), Income Tier (High: **₹29M**, Medium: **₹16M**, Low: **₹10M**), Dependent Count, and Education Level.

## Tools & Technical Stack Used

* **Power BI Desktop:** Core platform utilized for report page design, data modeling, and visualization architecture.

* **Power Query (M Language):** Employed for advanced ETL processes, data cleaning, attribute standardization, and structural normalization.

* **DAX (Data Analysis Expressions):** Formulated custom measures for calculated columns, multi-variable KPI aggregations, satisfaction indexing, and time-intelligence comparisons.

* **PostgreSQL / CSV:** Source database storage managing the underlying transaction (`public.cc_detail`) and demographic (`public.cust_detail`) relational tables.

## Key Insights

* **Product Concentration:** The **Blue Card** tier acts as the primary revenue engine, contributing **₹46M** out of the ₹55M total portfolio value—accounting for over **83%** of aggregate revenue.

* **Dominant Spend Buckets:** **Bills** represent the leading transaction category at **₹14M**, closely followed by **Entertainment** at **₹10M**, pinpointing clear targets for rewards-program optimization.

* **High-Value Professional Segment:** The **Businessman** cohort yields the highest occupational revenue at **₹17M** and commands **₹2.5M** of the total interest earned.

* **Demographic Target Core:** The **40–50 age group** forms the most valuable customer segment, accounting for a combined **₹25M+** in revenue share.

* **Low Digital Channel Adoption:** **Swipe transactions dominate at ₹35M**, far exceeding Chip (₹17M) and Online (₹3M), signaling a major opportunity to digitize user behaviors.

* **Income Tier Disparity:** High-income consumers represent the financial anchor of the portfolio, contributing **₹29M**—over **53%** of total revenue.

* **Seasonal Peaks:** Portfolio revenue experienced strong mid-year acceleration, reaching weekly peaks of approximately **₹0.77M** in April 2023.

## Learning Outcomes

* **Relational Data Modeling:** Gained hands-on experience establishing structured star-schema relationships between large scale transaction and dimension tables based on Customer IDs.

* **Advanced DAX Engineering:** Developed proficiency in writing custom calculations for context-aware KPIs, time-intelligence trend comparisons, and dynamic demographic bucketing.

* **Interactive UI/UX Best Practices:** Mastered configuration of synchronized multi-page slicers, cross-filtering, and strategic space management to ensure seamless navigation.

* **Strategic Visual Selection:** Learned to select optimal visualization styles based on data complexity—utilizing dual-axis combo charts for volume-to-value trends and clustered bars for multi-variable demographic profiling.

## Challenges Faced & Resolution

* **Handling Incomplete Demographic Records:** The raw data contained widespread null values and "Unknown" text indicators across critical tracking metrics like education levels and dependent counts.

  * *Resolution:* Standardized missing fields within Power Query using conditional formatting logic to prevent downstream data skewing while protecting row-count integrity.
  
* **Calendar & Time Intelligence Setup:** Building weekly and quarterly filters required a dedicated fiscal time dimension to manage asynchronous reporting dates.

  * *Resolution:* Engineered a robust, custom calendar table utilizing DAX to establish predictable time intelligence filtering paths.
  
* **Visual Density Management:** Consolidating more than 8 individual data visuals on a single dashboard screen created high visual density and potential cognitive overload.

  * *Resolution:* Applied rigorous design alignment rules, adjusted typography hierarchies, eliminated redundant labels, and utilized an intentional, clean layout to maximize whitespace.
  
* **Synchronizing Scales on Dual-Axes:** Combining high-volume transaction counts with monetary revenue metrics on a unified quarterly trend line risked data misinterpretation.

  * *Resolution:* Calibrated the visual scale properties manually, applying distinct data-label themes to isolate volume metrics from currency values.

## My Efforts and Contributions

* Directed the end-to-end business intelligence workflow: extracting raw SQL/CSV tables, defining table relationships, auditing data constraints, and designing layouts.

* Authored **15+ foundational DAX measures** covering Core Revenue, Aggregate Interest, CSS score indexing, and custom customer category segmentation boundaries.

* Designed a custom, high-contrast visual theme featuring a professional blue and gold color palette tailored to credit card industry branding.

* Conducted system validation testing to verify that all page interactions, cross-highlighting, and filter dependencies operate accurately without processing bottlenecks.

## Skills Demonstrated

`Business Intelligence (BI)` • `Data Modeling (Star Schema)` • `DAX Measure Engineering` • `Power Query & ETL` • `Data Cleaning & Standardization` • `Financial Analytics` • `Demographic Segmentation` • `Dashboard UI/UX Design`

## Conclusion

This portfolio project demonstrates my capacity to take large-scale, relational financial datasets and translate them into polished, interactive dashboard solutions tailored for executive leadership review. As a BBA student, building this project from scratch has bridge the gap between financial administration theory and modern data analytics tools, developing core competencies directly applicable to roles such as Business Analyst, Data Analyst, or Financial Analyst.

***

**Project Developed By:** Palak Tripathi | BBA Student | Aspiring Data & Business Analyst  

**Let's Connect:** Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/palak-tripathi-37a56234a/) or reach out if you would like to discuss this project further!
