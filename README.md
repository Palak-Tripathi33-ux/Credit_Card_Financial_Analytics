# Credit_Card_Financial_Analytics
Developed an end-to-end interactive BI solution analyzing $935K in revenue and $10M in customer income data. Formulated complex DAX measures and relational data models to segment consumer behavior across 5+ demographic vectors and transactional channels, enabling targeted portfolio optimization.

💳 Credit Card Financial Analytics Dashboard — Power BI
> An end-to-end interactive BI solution monitoring $935K in revenue and $10M in customer income data across transaction behaviour, demographics, and weekly performance trends.
---
📁 Project Overview
Built a two-page Power BI dashboard delivering real-time operational and customer-level insights into a credit card portfolio. The data model connects `cc_detail` (transaction-level) and `cust_detail` (customer profile) tables via a common `client_num` key, with custom DAX measures powering dynamic week-over-week (WoW) revenue comparisons.

🎯 Business Objective
Turn high-volume credit card transaction and customer data into a self-service analytics tool so financial stakeholders can track revenue shifts, identify at-risk segments, and make faster decisions in product management, risk monitoring, and customer retention — without writing a single query.

🧩 Dashboard Features
Page 1 — CC Transactions Report opens with four KPI cards covering Total Revenue, Transaction Amount, Interest Earned, and Transaction Count. A combo line-and-column chart tracks week-over-week revenue using custom DAX measures. Horizontal bar charts break down spending across Bills, Entertainment, Fuel, Grocery, Food, and Travel, while a second bar chart compares Blue, Silver, Gold, and Platinum card performance. A treemap visualises transaction method distribution — Chip, Swipe, and Online — and a quarterly bar chart highlights Q1–Q4 trends. Quarter and Gender slicers cross-filter all visuals simultaneously.
Page 2 — CC Customer Report leads with KPI cards for Revenue, Total Income, Customer Satisfaction Score (CSS), and Interest Earned. Clustered column and bar charts segment customers by age group, income level, marital status, gender, job category, and education level. State-level treemaps provide geographic revenue distribution. A full customer data table enables granular drill-down, with Quarter and Gender slicers maintaining cross-page consistency.

🛠️ Tools Used
Power BI Desktop · DAX · Power Query (M) · SQL / PostgreSQL

💡 Key Insights
Blue card holders drive the largest revenue share — a high-volume mass-market segment carrying the core business
Bills and Entertainment are the top expenditure types, outperforming discretionary categories consistently
Swipe dominates in volume, but Chip transactions show stronger revenue per transaction
Male customers aged 40–50 generate higher revenue; satisfaction scores vary sharply across income groups — a clear retention flag
Businessmen and White-collar professionals are the top two revenue-contributing job segments, ideal targets for premium card upselling
Q4 shows strong recovery trends across WoW fluctuations — useful for seasonal planning

📚 Learning Outcomes
Wrote time-intelligence DAX measures using `CALCULATE`, `FILTER`, `ALL`, and `DIVIDE` for WoW revenue tracking
Built and validated a star-schema-like relational model between fact and dimension tables
Cleaned raw CSVs via Power Query — handled null values, data type mismatches, and created calculated columns like `AgeGroup` and `IncomeGroup`
Structured two report pages around business questions, not data availability

⚠️ Challenges Faced
WoW DAX measures returned incorrect values until `ALL()` inside `FILTER()` was used to correctly clear filter context — took significant trial and error
Several numeric columns imported as text due to nulls, causing aggregation errors resolved through Power Query transformations
A many-to-many relationship warning between the two tables required diagnosing cardinality and confirming the correct many-to-one join via `client_num`
Fitting 16+ visuals per page without losing readability required multiple layout iterations

🙋 My Contributions
Independently handled the full pipeline — from studying raw datasets and understanding each field's business meaning, to building the data model, writing all DAX measures, designing both report pages, and deriving business-relevant insights from the final output. Nothing in this report was pre-built or templated.

🧠 Skills Demonstrated
`Power BI` · `DAX` · `Power Query` · `Data Modelling` · `KPI Design` · `Financial Analytics` · `Customer Segmentation` · `Revenue Analysis` · `Time-Intelligence Functions` · `Business Intelligence` · `Report Design` · `SQL / PostgreSQL`

✅ Conclusion
This project demonstrates the ability to handle financial data end-to-end — from raw transaction tables to a two-page executive dashboard — with the technical depth and design judgment that a real analytics role demands.

Power BI Desktop · cc_detail & cust_detail Dataset · Two-Page Report · WoW DAX Measures
