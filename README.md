# Credit_Card_Financial_Analytics
Developed an end-to-end interactive BI solution analyzing $935K in revenue and $10M in customer income data. Formulated complex DAX measures and relational data models to segment consumer behavior across 5+ demographic vectors and transactional channels, enabling targeted portfolio optimization.

💳 Credit Card Financial Analytics Dashboard
Power BI | Financial Analytics | Customer Intelligence | Transaction Monitoring

📌 Project Overview
This project is an end-to-end Credit Card Financial Analytics Dashboard built using Microsoft Power BI. It is designed to provide real-time operational and customer-level insights into a credit card portfolio, enabling financial stakeholders to monitor revenue performance, transaction trends, and customer behaviour on a single, interactive platform.

The dashboard is divided into two dedicated report pages:
CC Transactions Report — focused on weekly revenue tracking, spending categories, card usage patterns, and transaction volumes.
CC Customer Report — focused on customer demographics, income segmentation, satisfaction scores, and behavioural trends.

The data model integrates two core tables — cc_detail (transaction-level data) and cust_detail (customer profile data) — connected via a common client_num key, with DAX measures powering dynamic week-over-week (WoW) revenue comparisons.

🎯 Business Objective
Credit card operations generate enormous volumes of daily transaction and customer data. Without proper visibility, financial institutions struggle to:

Identify which card categories, expenditure types, or customer segments are driving or dragging revenue.
Detect early signs of delinquency or underutilisation.
Understand demographic patterns in card usage and satisfaction.
Monitor WoW revenue shifts to react quickly to drops or spikes.

This dashboard was built to address these challenges — translating raw transactional and customer data into actionable business intelligence that can support decisions in product management, risk monitoring, marketing strategy, and customer retention.

📊 Dashboard Features
Page 1 — CC Transactions Report

KPI Cards: Total Revenue, Total Transaction Amount, Total Interest Earned, Total Transaction Count — all at a glance.
Week-over-Week Revenue Trend: A combo chart (line + stacked column) tracking current vs. previous week revenue using custom DAX measures (Current_Week_revenue, Previous_Week_revenue, wow_revenue).
Revenue by Expenditure Type: Horizontal bar charts breaking down spending across categories such as Bills, Entertainment, Fuel, Grocery, Food, and Travel.
Revenue by Card Category: Visual comparison of Blue, Silver, Gold, and Platinum card performance.
Revenue by Chip Usage: Treemap showing distribution across Chip, Swipe, and Online transaction methods.
Revenue by Quarterly Performance: Bar chart highlighting Q1–Q4 revenue trends.
Transaction Data Table: Detailed tabular view for granular drill-down.
Slicers: Interactive filters by Quarter and Gender to slice all visuals simultaneously.

Page 2 — CC Customer Report

KPI Cards: Total Revenue, Total Income, Customer Satisfaction Score (CSS), Interest Earned.
Customer Age Group Distribution: Clustered column chart segmenting customers by age brackets.
Revenue by Income Group: Bar chart showing how revenue differs across Low, Medium, and High income groups.
Revenue by Marital Status and Gender: Stacked bar charts revealing demographic breakdowns.
Revenue by Job Category: Bar chart mapping professions (Businessman, White-collar, Blue-collar, Self-employed, Govt, Retirees) to revenue contribution.
Revenue by State: Treemaps providing geographic distribution insights.
Revenue by Education Level: Visual breakdown across education categories.
Customer Data Table: Full customer-level detail for deep-dive analysis.
Slicers: Quarter and Gender filters for cross-page consistency.

💡 Key Insights

Blue card holders account for the largest share of total revenue compared to Silver, Gold, and Platinum categories, suggesting a high-volume, mass-market segment drives the core business.
Bills and Entertainment are consistently the top expenditure types by transaction amount, indicating that everyday spending categories are more profitable than discretionary ones.
Swipe-based transactions dominate chip and online usage in volume, though chip transactions show relatively stronger revenue per transaction.
Male customers in the 40–50 age group tend to generate higher revenue, while satisfaction scores vary significantly across income groups — a flag for targeted retention strategies.
Businessmen and White-collar professionals are the two highest revenue-contributing job categories, pointing to clear priority segments for premium card upselling.
Week-over-week revenue fluctuations are visible across quarters, with Q4 showing strong recovery trends — useful for seasonal planning and budgeting.
Delinquency patterns in the transaction table, when filtered by card category, can expose risk concentration in specific segments.


📚 Learning Outcomes
Working on this project gave me practical, hands-on exposure to skills that are directly applicable in a data analyst role:

Data Modelling: Building and managing table relationships in Power BI using primary and foreign keys across fact and dimension tables.
DAX Proficiency: Writing time-intelligence and filter-context measures including CALCULATE, FILTER, ALL, and DIVIDE functions for business KPIs.
Power Query Transformation: Cleaning and preparing raw data, handling data type conversions, and creating calculated columns like AgeGroup and Income Group.
Dashboard Design Thinking: Structuring visuals around business questions rather than just data availability — learning to ask "what does the business need to see?"
Storytelling with Data: Organising two report pages with logical flow so that any business user can derive insights without technical guidance.

⚙️ Challenges Faced
1. DAX Context Errors in WoW Revenue:
The week-over-week calculation initially returned incorrect values because the filter context was not being cleared properly. Resolving this required using ALL() inside FILTER() to override row context — a concept that took significant trial and error to get right.
2. Data Type Inconsistencies:
Several numeric columns were imported as text due to null values and formatting in the source CSV, which caused aggregation errors. These were resolved through Power Query transformation steps.
3. Relationship Ambiguity:
The initial data model had a many-to-many relationship warning between cc_detail and cust_detail. Diagnosing and fixing this by confirming the correct cardinality (many-to-one via client_num) was a meaningful learning experience in relational data modelling.
4. Visual Overcrowding:
Fitting 16+ visuals per page without losing clarity was a real design challenge. Multiple layout iterations were needed to achieve a clean, readable dashboard.

🤝 My Efforts & Contributions
This project was independently designed, built, and documented by me from the ground up. My specific contributions include:

Data Acquisition & Understanding: Studied the raw cc_detail and cust_detail datasets, understood each field's business meaning before building anything.
Data Model Design: Established the star-schema-like relationship between transaction and customer tables.
DAX Measure Development: Wrote all custom DAX measures including Current Week Revenue, Previous Week Revenue, and WoW % Change — none of these were pre-built.
Dashboard Layout & UX: Designed both report pages with consistent colour themes, slicer placements, and card formatting for professional visual quality.
Insight Generation: Analysed the final dashboard outputs to derive business-relevant observations, not just describe what the charts show.
Documentation: Wrote this README to communicate the project professionally for technical and non-technical audiences.

Skills Demonstrated
Power BI DAX Power Query Data Modelling KPI Design Financial Analytics
Customer Segmentation Revenue Analysis Data Visualisation Business Intelligence
Time-Intelligence Functions Report Design Relational Data Modelling SQL / PostgreSQL
