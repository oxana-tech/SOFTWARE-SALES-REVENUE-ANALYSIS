# SOFTWARE-SALES-REVENUE-ANALYSIS

## Executive Summary

Analyzed 123K SaaS transactions to identify key revenue drivers, segment performance, and growth opportunities.

#### Key results:
- Detected a sharp APAC revenue drop (−14%) → potential churn or seasonality issue
- Identified enterprise segment as a major revenue driver (33% users → >50% revenue)
- Revealed underperforming product (Publishing: −56% vs лидеров)

#### Impact:
The dashboard enables faster decision-making in sales prioritization, pricing strategy, and market focus.

## Tech Stack

- Tableau (data visualization, dashboards, calculated fields)
- SQL 
- Data modeling concepts (aggregations, LOD, table calculations)

## My Analytical Approach

1. Defined business questions with stakeholders
2. Cleaned and validated dataset (handled missing values, checked duplicates)
3. Built core metrics: MRR, ARPPU, revenue share
4. Performed segmentation:
   - by region
   - by customer type
   - by product
5. Identified trends and anomalies
6. Designed dashboard for decision-making

## Challenges & Solutions

- Issue: incorrect aggregation in % calculations
  Solution: used WINDOW_SUM and adjusted compute using

- Issue: tooltip inconsistency
  Solution: fixed level of detail using calculated fields

- Issue: multi-metric visualization
  Solution: used Measure Names / Measure Values

#### Result:
Reduced time for monthly reporting
- Enabled quick identification of revenue trends and anomalies
- Provided a single source of truth for product and regional performance

##### Key business impact:
- Identified APAC revenue drop (-14% mid-year) → potential churn or seasonality issue
- Confirmed enterprise segment generates disproportionately high revenue (33% users → >50% revenue impact)
- Highlighted underperforming product (Publishing) → candidate for pricing or positioning changes
- 
#### Business Value
The dashboard answers key questions posed by management:

Which products and regions generate the most revenue?
How does MRR (monthly recurring revenue) change over time?
How important is the enterprise customer segment?
Are there any dips or anomalies that require attention?

### Why This Project Matters

This project demonstrates my ability to:
- translate business questions into data analysis
- work with real SaaS metrics (MRR, ARPPU)
- build decision-support dashboards
- identify actionable insights, not just describe data

This enables decision-making regarding sales prioritization, marketing budget allocation, and working with customer segments without the need to manually generate reports every month.

## Key Findings and Insights

##### By region:

USA — the largest region in terms of absolute revenue ($643,880), but its share of total revenue is relatively stable (~8–10% monthly)
APAC revenue share drops from 15% to ~1% mid-year,
indicating a critical performance decline.
This may signal:
- customer churn
- сезонный фактор
- снижение маркетинговой активности
Recommendation:
- analyze retention and churn rate
- review acquisition channels
- run cohort analysis
EMEA—the smallest region by volume ($240,170), but with good stability

#### By product:

Main App and Customer Success are the revenue leaders (~$400K each)
Publishing generates 56% less revenue than the top-performing products (~$175K vs ~$400K),
which may indicate weak product-market fit or ineffective pricing.

Recommendation:
- Run pricing A/B test
- Analyze user adoption funnel for this product
- Review positioning vs competitors

#### By client:
 
Enterprise customers account for 33% of the customer base, but their average transaction value is higher (up to $25 vs. $10–15 for regular customers)—they are disproportionately important to revenue
This confirms the importance of the enterprise segment as a priority for growth


### Dashboard Design Logic
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
## Dashboard screenshot
- <a href="https://drive.google.com/file/d/1T1fpgOGoAgExAGEbNFe7V6XQuvPGtQuu/view?usp=sharing">Dashboard screenshot</a>

