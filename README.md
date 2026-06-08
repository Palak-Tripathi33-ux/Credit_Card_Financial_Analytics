# 💳 Credit Card Financial Analytics Dashboard
Power BI | Financial Analytics | Business Intelligence | DAX QUERY

📌 Project Overview
This is an end-to-end Power BI dashboard project built to analyze credit card transaction and customer data. The dashboard is split into two report pages — Credit Card Transaction Report and Credit Card Customer Report — and provides a consolidated view of revenue performance, spending behavior, and customer demographics.
The project uses real-world-style structured data with two core tables: cc_detail (transaction data) and cust_detail (customer data), connected via a shared client_num key. All data was loaded from a PostgreSQL database into Power BI for transformation and visualization.

🎯 Business Objective
Credit card companies generate revenue through interest, annual fees, and transaction volumes — but understanding who is spending, how much, and when requires more than raw numbers. The goal of this project was to:

Track weekly and quarterly revenue trends across card categories
Identify which customer segments (by age, income, job, education) are most profitable
Monitor key risk indicators like delinquent accounts and revolving balances
Enable data-driven decisions for marketing, credit limit adjustments, and customer retention

📊 Dashboard Features — Page 1 (Transaction Report)

Revenue by Card Category — compares Blue, Silver, Gold, and Platinum cards
Revenue by Expenditure Type — breaks down bills, entertainment, fuel, grocery, food, travel
Revenue by Use Chip — separates Chip, Swipe, and Online transactions
Weekly Revenue Trend — a line chart tracking week-over-week movement
KPI Cards — Total Revenue, Total Interest Earned, Total Transaction Amount, Transaction Count
Quarter Filter — slicers for Q1 to Q4

Key DAX Measures Used:

Current_Week_Revenue — SUM of revenue filtered to the latest week number
Previous_Week_Revenue — SUM of revenue from the previous week
WoW_Revenue — Week-over-Week growth rate using DIVIDE()

📊 Dashboard Features — Page 2 (Customer Report)

Revenue by Age Group — 20s, 30s, 40s, 50s, 60+ segments
Revenue by Income Group — Low, Medium, High income brackets
Revenue by Education Level — graduates, post-graduates, high school, others
Revenue by Marital Status — married, single, unknown
Revenue by Job Type — businessman, white-collar, self-employed, govt, blue-collar, retirees
Customer Satisfaction Score — average score tracked by segment
Top 5 States by Revenue — geographic breakdown

🛠️ Tools Used

Power BI Desktop — dashboard design, data modeling, DAX calculations
PostgreSQL — source database for both transaction and customer tables
DAX — custom measures for week-over-week and current/previous week logic
Power Query (M Language) — data cleaning, type fixes, column transformations
Excel / CSV — initial data preparation before database import

💡 Key Insights

📅 Data filtered to Q4 | Week - 01 October 2023

1. Blue Card Dominates Revenue — by a Wide Margin
Blue card holders generated ₹843K in revenue out of the total ₹994K, making up roughly 85% of all card revenue. Silver was a distant second at ₹121K, followed by Platinum (₹19K) and Gold (₹10K). This shows the Blue card is the primary revenue driver and should be the focus for retention and upsell strategies.
2. Swipe Transactions Lead, But Online Is Underutilized
Swipe-based transactions generated ₹0.67M, significantly ahead of Chip (₹0.26M) and Online (₹0.06M). The very low share of online transactions (~6%) indicates a major opportunity to push digital adoption through targeted offers or cashback incentives.
3. Bills and Fuel Are the Top Spending Categories
Bills accounted for ₹0.25M and Fuel for ₹0.19M, together making up the largest share of transaction volume. Entertainment (₹0.16M), Grocery (₹0.14M), and Food (₹0.14M) followed closely. Travel (₹0.11M) had the lowest contribution — suggesting customers primarily use their cards for everyday essentials, not leisure.
4. Businessmen Are the Most Valuable Customer Segment
Businessmen contributed ₹299K in revenue — nearly double that of the second-highest group, Self-employed customers (₹161K). White-collar (₹149K) and Govt employees (₹149K) were nearly tied. Retirees generated the lowest revenue at ₹109K, making them the least profitable segment.
5. High-Income Group Generates the Most Revenue
High-income customers contributed ₹0.41M, compared to Medium (₹0.15M) and Low (₹0.21M) income groups. Interestingly, Low-income customers outperformed Medium — suggesting higher transaction frequency or revolving balance behavior in that segment worth investigating.
6. Married Customers Spend More Than Single Customers
Married customers generated ₹0.25M in revenue versus ₹0.20M from single customers. This ~25% gap suggests that married customers likely have higher household spending needs, making them a more valuable demographic for premium card offers.
7. The 40–50 Age Group Is the Highest-Revenue Age Segment
Customers aged 40–50 contributed ₹0.20M in revenue, followed by the 50–60 group (₹0.18M) and 30–40 group (₹0.16M). The 20–30 and 60+ groups contributed the least. Mid-career professionals in their 40s appear to be the most financially active credit card users.
8. Graduates Lead in Revenue Across Education Levels
Graduate customers generated ₹0.19M, the highest among all education groups, followed by Unknown (₹0.12M) and High School (₹0.11M). Post-graduates and Doctorate holders contributed the least — possibly due to smaller sample size or lower card usage frequency.
9. New York and California Are the Top Revenue-Generating States
NY led with a combined revenue of ₹0.26M (₹0.13M each across two segments), followed by CA (₹0.23M), FL (₹0.20M), and TX (₹0.18M). NJ had the lowest contribution among the Top 5 states. These 5 states together account for the majority of geographic revenue concentration.
10. Overall Dashboard KPIs at a Glance (Q4)
Total Revenue: ₹994K
Total Transaction Amount: ₹799K
Total Interest Earned: ₹138K
Total Transaction Count: ~12K
Average Customer Satisfaction Score: 4.19 / 5
Total Customer Income Pool: ₹10M

📚 Learning Outcomes

Learned how to connect Power BI directly to a PostgreSQL database and manage live data refresh settings
Built and applied time-intelligence DAX measures including week-over-week calculations using FILTER(), ALL(), and CALCULATE()
Understood the importance of data modeling — created a proper one-to-many relationship between cust_detail and cc_detail using client_num
Learned to create calculated columns for derived fields like AgeGroup and Income Group that are not present in raw data
Practiced report design principles — visual hierarchy, consistent color themes, and filter placement for usability
Understood how slicers and cross-filtering work together to enable interactive storytelling in dashboards

⚡ Challenges Faced
1. UTF-16 Encoded Schema Files
The Power BI template file (.pbit) stores its data model in UTF-16-LE encoding, which required careful handling when reviewing the underlying structure outside of Power BI.
2. DAX Week Filtering Logic
Writing the Current_Week_Revenue and Previous_Week_Revenue measures was tricky. Getting the FILTER + ALL + MAX combination right to isolate the correct week number took multiple iterations and testing.

🙌 My Efforts and Contributions

Sourced and structured the dataset independently, including setting up the PostgreSQL tables and writing import queries
Designed both dashboard pages from scratch — layout, color palette, visual selection, and filter placement
Wrote all DAX measures manually, including the week-over-week revenue logic
Created custom calculated columns (AgeGroup, Income Group) in Power Query to enable meaningful demographic segmentation

🧠 Skills Demonstrated
Power BI · DAX · Power Query · PostgreSQL · Data Modeling · Financial Analytics · KPI Dashboard Design · Time Intelligence · Data Cleaning · Business Intelligence · Data Storytelling · Segmentation Analysis

🏁 Conclusion
This project gave me practical, hands-on experience in building a business-grade analytics dashboard from raw transactional and customer data. Working through the full pipeline — from database to data model to final visuals — helped me understand not just the tools, but the thinking behind converting data into decisions.
As a BBA student with a strong interest in business analytics and finance, this project reflects my ability to independently take on a real-world BI problem, handle its technical challenges, and deliver a clean, insight-driven output. I plan to continue expanding this dashboard with forecasting visuals and customer churn indicators as I grow my skills further.


📬 Feel free to connect with me on LinkedIn - https://www.linkedin.com/in/palak-tripathi-37a56234a/  or reach out if you'd like to discuss this project further.
