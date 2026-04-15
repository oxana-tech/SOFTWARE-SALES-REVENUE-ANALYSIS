# SOFTWARE-SALES-REVENUE-ANALYSIS
The project is an analytical dashboard based on a SaaS company’s transaction data for the period June 2022–May 2023 (123,195 payment records). The dashboard visualizes revenue trends by product, region, and customer type, allowing users to track growth, seasonality, and revenue structure. It was built in Tableau from scratch—from data preparation to the final layout.
Business Value
The dashboard answers key questions posed by management:

Which products and regions generate the most revenue?
How does MRR (monthly recurring revenue) change over time?
How important is the enterprise customer segment?
Are there any dips or anomalies that require attention?

This enables decision-making regarding sales prioritization, marketing budget allocation, and working with customer segments without the need to manually generate reports every month.
Key Findings and Insights
By region:

USA — the largest region in terms of absolute revenue ($643,880), but its share of total revenue is relatively stable (~8–10% monthly)
APAC shows a higher share at the beginning of the year (up to 15%), but a noticeable drop in the middle—which signals seasonality or churn
EMEA—the smallest region by volume ($240,170), but with good stability

By product:

Main App and Customer Success are the revenue leaders (~$400K each)
Publishing generates significantly less ($175K)—a possible candidate for a strategy or pricing review
Marketing Automation holds a steady second place among specialized products

By client:
 
Enterprise customers account for 33% of the customer base, but their average transaction value is higher (up to $25 vs. $10–15 for regular customers)—they are disproportionately important to revenue
This confirms the importance of the enterprise segment as a priority for growth


Dashboard Design Logic
Data source: CSV file saas_revenue.csv with the following fields: user_id, payment_date, location, software_name, is_enterprise_customer, revenue_amount
Calculated fields you created:

Payment month / Month of Payment date — for grouping by month
Revenue by Location — calculation of revenue share by region out of the total
New MRR / ARPPU — subscription business metrics
Positive% / Negative% — for analyzing percentage changes
Paid Users count — unique paying users in the period.
Compiled reports:
NEW MRR by month - Total revenue by month,
% Difference in Revenue - Change in revenue (percentage),
Payment in the first month - Cohort analysis of first payments,
KPI - Key metrics (MRR, ARPPU, Users),
% Revenue by Locations - Revenue share by region (APAC / EMEA / USA),
Distribution of transactions - Distribution of transactions,
Architectural solutions:

Used filters by Action (by date and location) for interactivity
Applied Measure Names / Measure Values to display multiple metrics on a single chart
Manually configured tooltips for a more informative hover effect
Split the dashboard into several thematic sheets instead of a single overloaded screen.



## Dataset
- <a href="https://drive.google.com/file/d/1ikLR1E1I0vYYJB3J92ZXv4kbDMvo4PXs/view?usp=sharing">Dataset</a>
## Dashboard
- <a href="https://public.tableau.com/views/__2_17530401782940/Softwaresalesrevenueanalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link">SOFTWARE SALES REVENUE ANALYSIS</a>
