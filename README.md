💳 Credit Card Financial Analytics Dashboard — Power BI

A two-page interactive Power BI dashboard analyzing credit card transactions and customer behavior across ₹55M+ in revenue data.

📌 Project Overview

This project is a Power BI business intelligence dashboard built to analyze credit card financial data across two perspectives — transactions and customers. It covers over 1 million transactions, ₹55M in total revenue, and ₹45M in transaction amounts, helping stakeholders understand spending patterns, customer demographics, and revenue drivers at a glance.

The dashboard is divided into two report pages:

CC Transactions Report — focuses on spend categories, card performance, and quarterly trends.

CC Customer Report — focuses on customer demographics, income groups, geography, and CSS (Customer Satisfaction Score).

🎯 Business Objective

Identify which card categories and customer segments drive the most revenue.

Track quarterly revenue trends and transaction volumes across Q1–Q4.

Understand how demographics (age, job, education, marital status) influence spending.

Enable data-driven decisions for credit card product strategy and customer targeting.

📊 Dashboard Features

CC Transactions Report (Page 1)

KPI cards: Revenue ₹55M | Trans_Amt ₹45M | Total Interest ₹8M | Count 1M.

Revenue breakdown by card category — Blue (₹46M), Silver (₹6M), Gold (₹2M), Platinum (₹1M).

Revenue by expenditure type: Bills ₹14M, Entertainment ₹10M, Fuel ₹9M, Grocery ₹9M, Food ₹8M, Travel ₹6M.

QTR Revenue + Transaction Count combo chart (Q1–Q4 trend with ~164K avg transactions per quarter).

Revenue by use chip method: Swipe ₹35M, Chip ₹17M, Online ₹3M.

Revenue by education level, customer job, and card category bar charts.

Gender filter (M/F) + Card type slicer for dynamic segmentation.

CC Customer Report (Page 2)

KPI cards: Revenue ₹55M | Total Interest ₹8M | Income ₹576M | CSS 3.19.

Revenue by week (Jan–Oct 2023) with weekly fluctuation between ₹0.38M–₹0.77M.

Revenue by age group: 40–50 age band contributes the highest (₹11M + ₹14M across genders).

Job-wise breakdown: Businessman ₹17M, White-collar ₹10M, Self-employed ₹8M.

Top 5 States: TX, NY, CA, FL, NJ — with TX and NY each generating ₹6–7M.

Revenue by marital status: Married ₹26M, Single ₹22M.

Revenue by income group: HIGH ₹29M, MEDIUM ₹16M, LOW ₹10M.

Revenue by dependent count and education level.

Quarter (Q1–Q4) + Week start date slicer for time-based filtering.

🛠️ Tools Used

Microsoft Power BI Desktop — dashboard design, DAX measures, data modeling.

Power Query (M Language) — data cleaning and transformation.

DAX (Data Analysis Expressions) — custom measures for revenue, interest, CSS, and time intelligence.

PostgreSQL / CSV — source data tables (public.cc_detail, public.cust_detail).

GitHub — version control and project documentation.

🔍 Key Insights

Blue card holders account for ₹46M out of ₹55M total revenue — over 83% of all revenue.

Bills is the top expenditure category at ₹14M, followed by Entertainment at ₹10M.

Businessmen generate the highest revenue by job at ₹17M with ₹2.5M in interest earned.

The 40–50 age group is the most valuable customer segment with combined ₹25M+ revenue.

Swipe transactions dominate at ₹35M vs Chip ₹17M and Online ₹3M — indicating low digital adoption.

High-income group customers alone contribute ₹29M — 53% of total revenue.

Married customers generate slightly more revenue (₹26M) vs Single (₹22M).

Revenue peaked mid-year with weekly highs around ₹0.77M in April 2023.

Graduate-level customers are the top earners by education at ₹22M revenue.

CSS score of 3.19/5 signals moderate customer satisfaction — room for product improvement.

📚 Learning Outcomes

Built a multi-page Power BI report from raw relational data with two fact/dimension tables.

Wrote DAX measures for aggregated KPIs, time intelligence (quarterly comparison), and CSS calculation.

Designed interactive slicers — quarter filter, week start date, gender, and card type — enabling cross-page filtering.

Applied data modeling best practices by linking cc_detail and cust_detail tables on customer ID.

Learned to choose the right visual type per use case — combo charts for trend + volume, clustered bars for demographic comparison.

Understood how to present ₹55M+ financial data in an executive-ready, one-glance format.

⚡ Challenges Faced

Messy demographic data — multiple nulls and "Unknown" values in education, marital status, and dependent count fields required careful handling in Power Query without distorting totals.

Date table setup — building a proper calendar table for week-based and quarterly slicing required custom DAX and Power Query steps.

Chart clutter — fitting 8+ visuals per page while keeping the layout readable required iterative design decisions on spacing, font sizes, and color coding.

Dual-axis chart — aligning revenue bars and transaction count line on different scales in the QTR chart was technically tricky.

Filter consistency — ensuring slicers on Page 1 didn't bleed into Page 2 unintentionally required explicit filter scope management.

💼 My Efforts and Contributions

Sourced, cleaned, and modeled two raw data tables with 10,000+ customer records and 1M+ transactions.

Designed the entire dashboard layout from scratch — no templates used.

Wrote 15+ DAX measures including Revenue, Total Interest, CSS, QoQ comparisons, and income-group segmentation.

Created a consistent color theme — blue/gold palette aligned with credit card brand aesthetics.

Tested all slicers and cross-filter interactions to ensure accurate drill-down behavior.

🧠 Skills Demonstrated

Power BI Dashboard Design (multi-page, multi-visual).

DAX — calculated columns, measures, time intelligence.

Power Query — data cleaning, joins, type casting.

Data Modeling — star schema, table relationships.

Business Analysis — translating raw financial data into actionable insights.

Data Storytelling — structuring a narrative across two focused report pages.

Attention to Detail — consistent formatting, labeled axes, readable color contrast.

✅ Conclusion

This project demonstrates my ability to independently build a production-grade Power BI dashboard on real-world financial data — from raw CSV/SQL tables to a polished, recruiter-ready analytics report. As a BBA student, this project reflects my understanding of both business fundamentals and data analytics, and my commitment to building skills that are directly applicable in roles like Business Analyst, Data Analyst, or Financial Analyst.

Made by - Palak Tripathi | BBA Student | Aspiring Data & Business Analyst

📬 Feel free to connect with me on LinkedIn - https://www.linkedin.com/in/palak-tripathi-37a56234a/  or reach out if you'd like to discuss this project further.
