*My Role: Data Analysis*

<h1 align="center"><u>Cooking Fuel Sales Analysis</u></h1>  

A data-driven analysis to understand customer purchasing behaviour, identify the root cause of year-end sales decline, and build a predictive framework for targeted marketing.

---

## Problem
The business was experiencing a consistent decline in sales towards the end of the year with no clear understanding of what was driving it. Discounts were being given out without a measurable strategy, and there was no system in place to identify which customers were at risk of leaving or when each customer was likely to return.

## Goals
- Identify the root cause of the year-end sales decline
- Evaluate whether discounts were genuinely driving sales
- Understand individual customer purchasing cycles and predict next purchase dates
- Cluster customers into actionable segments for targeted marketing

## What I Did

- Performed **descriptive analysis** on monthly sales trends, state-level performance, product revenue, and new customer acquisition patterns across 1,632 transactions from 297 unique customers
- Conducted **diagnostic analysis** to systematically eliminate collection type, pricing, and discounts as root causes of the sales decline — ruling each one out through data before moving to the next
- Compared **discounted vs non-discounted orders** on quantity (2.94 vs 2.98 units) and revenue per transaction ($646.43 vs $647.21) to confirm discounts had no measurable impact on buying behaviour
- Analysed **individual customer purchase gaps** using median gap days and current gap days to classify every customer into Active, Due Soon, At Risk, Churned, and One-Time Churned status groups
- Applied **K-Means clustering** with the Elbow Method to segment 297 customers into four actionable groups — High Value, Loyal, At-Risk, and Lost
- **Predicted each customer's expected next purchase date** using personal and global median gap to enable time-based personalised marketing

🔗 **[Check out the full analysis here](https://github.com/)**

---

## Key Findings

- **91.2%** of customers are repeat buyers — a strong and loyal customer base
- New customer acquisition **effectively stopped after February**, identified as the primary driver of the year-end sales decline
- **$33,283.80** in discounts given away — representing **3.15% of $1,055,880.72 total revenue** — with no measurable return on customer behaviour or sales volume
- Georgia led all states with **86 transactions** while Virginia recorded only **25**, revealing a significant regional performance gap
- **39 customers are due soon** — an immediate and actionable revenue opportunity
- **147 customers (49.5%)** are currently active and purchasing within their normal expected cycle

## Customer Status Breakdown

| Status | Customers | % |
|--------|-----------|---|
| Active | 147 | 49.5% |
| At Risk | 44 | 14.8% |
| Churned | 41 | 13.8% |
| Due Soon | 39 | 13.1% |
| One-Time Churned | 26 | 8.8% |

## Customer Segments (K-Means)

| Segment | Customers | % |
|---------|-----------|---|
| Loyal Customers | 138 | 46.5% |
| At-Risk Customers | 75 | 25.3% |
| High Value Customers | 55 | 18.5% |
| Lost Customers | 29 | 9.8% |

## Recommendations
1. Launch structured new customer acquisition campaigns to replenish the pipeline consistently throughout the year — not just in January and February
2. Schedule personalised marketing emails **one week before** each customer's predicted next purchase date based on their individual purchase cycle
3. Tailor email content by cluster — premium messaging for High Value, warm reminders for Loyal, urgent incentive-led offers for At-Risk, and re-engagement campaigns for Lost customers
4. Discontinue broad unstructured discounting and redirect that budget into targeted customer recovery campaigns where it can drive measurable behaviour change
5. Invest in underperforming states like Virginia through localised campaigns to close the significant regional performance gap

## Tools Used
- **Python** — Analysis & Modelling
- **Pandas** — Data Manipulation
- **Matplotlib** — Data Visualisation
- **Scikit-learn** — K-Means Clustering & StandardScaler
- **Jupyter Notebook** — Development Environment
