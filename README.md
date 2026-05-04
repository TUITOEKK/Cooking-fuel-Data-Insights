*My Role: Data Analysis*

<h1 align="center"><u>Cooking Fuel Sales Analysis</u></h1>

A Python data analysis project to understand customer purchasing behaviour, identify the root cause of year-end sales decline, and build a predictive framework for targeted marketing across 1,632 transactions from 297 unique customers.

---

## Project Overview

This project presents a sales analysis for a cooking fuel distribution business selling 
different varieties. The project is designed to deliver actionable insights into customer behaviour, product performance, and sales trends. The analysis covers three layers:

- **Descriptive Analysis** — understanding what happened
- **Diagnostic Analysis** — understanding why it happened
- **Predictive Analysis** — anticipating what will happen next

The objective is to support data-driven decision-making and highlight both opportunities and risks within the business.

🔗 **[Check out the full analysis here](https://github.com/TUITOEKK/Cooking-fuel-Data-Insights/blob/main/final.ipynb)**

---

## Business Problem

The cooking fuel business operates in a repeat consumption market where customer retention and purchasing consistency are critical to sustaining revenue. The business requires clear visibility into:

- Monthly sales trends and seasonal patterns
- Customer purchasing cycles and return behaviour
- Product and size performance across all segments
- Discount effectiveness and its true impact on revenue
- Regional sales distribution across states

Without structured insights, the business risks:

- Over-reliance on discounts without measurable returns
- Missing customers who are due to return or at risk of churning
- Inability to forecast demand and plan inventory effectively
- Continued decline in sales with no clear root cause identified

---

## Business Objectives

- Understand monthly sales dynamics and identify performance drivers
- Identify high and low performing states and regions
- Analyse product level performance fairly across all segments
- Evaluate the true impact of discounts on sales volume and revenue
- Predict each customer's next purchase date
- Cluster customers into actionable segments for targeted marketing

---

## Key Findings

### 1. Monthly Sales Trends
February recorded the highest sales at **174 transactions** while November was the weakest month at **94**. Sales remained fairly stable between April and July, ranging between 144 and 155, before declining steadily from August through to year end. This pattern points to strong early demand, stable mid-year performance, and a notable softening in the final quarter.

### 2. Regional Performance
Georgia led all states with **86 transactions**, followed by North Carolina with **84** and Tennessee with **78**. At the other end, Virginia recorded only **25 transactions** which is less than one third of Georgia's volume, highlighting a significant and uneven distribution of sales activity across the country.

### 3. New Customer Acquisition
January and February dominated new customer acquisition with **134** and **129** new customers respectively. From March onwards, acquisition dropped sharply to single digits and effectively reached zero by August. This reveals that sales from mid-year through December were sustained almost entirely by the existing customer base, with no fresh demand entering the pipeline.

### 4. Collection Type
Both Delivery and Pickup mirrored each other throughout the year, peaking and declining in unison. Collection type was therefore **ruled out** as a contributing factor to the year-end decline.

### 5. Pricing & Size
Prices remained completely consistent across all five  size categories 1lb, 20lb, 33lb, 100lb and 420lb throughout every month of the year. Pricing had **no influence** on sales fluctuations.

### 6. Discount Effectiveness
Discounted orders averaged **2.94 units** per transaction compared to **2.98** for non-discounted orders with a negligible difference of 0.04 units. Average revenue per transaction was virtually identical at **$646.43** versus **$647.21**. Despite this, the business gave away **$33,283.80** in discounts representing **3.15%** of total revenue of **$1,055,880.72**, with no measurable return in customer behaviour or sales uplift.

### 7. Customer Status Classification

Using each customer's personal median purchase gap and current gap since last purchase, all 297 customers were classified into five status groups:

| Status | Customers | % |
|--------|-----------|---|
| Active | 147 | 49.5% |
| At Risk | 44 | 14.8% |
| Churned | 41 | 13.8% |
| Due Soon | 39 | 13.1% |
| One-Time Churned | 26 | 8.8% |

### 8. Customer Segmentation — K-Means Clustering

K-Means clustering using purchase frequency, total spent, median gap days and current gap days identified four distinct segments:

| Segment | Customers | % |
|---------|-----------|---|
| Loyal Customers | 138 | 46.5% |
| At-Risk Customers | 75 | 25.3% |
| High Value Customers | 55 | 18.5% |
| Lost Customers | 29 | 9.8% |

---

## Key Problems Identified

- Near complete absence of new customer acquisition from March onwards
- Unstructured discount strategy with no measurable impact on behaviour
- Significant number of at-risk and churned customers requiring re-engagement
- Heavy reliance on existing customer base to sustain full-year revenue
- Large performance gap between top and bottom performing states

---

## Recommendations

**1. New Customer Acquisition** :
The business must urgently address the near-complete stop in new customer acquisition after February. Structured acquisition campaigns targeting new geographic areas, digital marketing investment, and referral incentives for existing loyal customers are needed to replenish the customer pipeline consistently throughout the year.

**2. Time-Based Personalised Marketing**:
Since each customer's expected next purchase date is now known, the business should schedule targeted marketing emails to be sent **one week before** each customer is due. Email content should be tailored by cluster segment — premium retention messaging for High Value customers, warm refill reminders for Loyal customers, urgent incentive-led offers for At-Risk customers, and re-engagement campaigns for Lost customers.

**3. Restructure Discount Strategy**:
The current discount approach was proven to have no impact on purchase quantity or revenue per transaction. The business should discontinue broad unstructured discounting and redirect that **$33,283.80** budget into targeted, purposeful campaigns tied to measurable outcomes particularly for At-Risk and Lost customer recovery.

**4. Regional Growth**:
The significant gap between top states like Georgia (86 transactions) and bottom states like Virginia (25 transactions) represents an untapped growth opportunity. Localised campaigns and improved distribution coverage in underperforming states could meaningfully grow overall transaction volume.

**5. Seasonal Planning**:
The consistent year-end slowdown in November and December should be anticipated in advance. Inventory and operational costs should be planned accordingly, and the quiet period used to run re-engagement campaigns targeting churned and at-risk customers ahead of the January peak.

---

## Final Conclusion

This project confirms that strong repeat purchase rates and customer loyalty alone are not sufficient to sustain long-term business growth. The near-complete absence of new customer acquisition from March onwards was identified as the **primary driver** of the year-end sales decline is not pricing, collection type, or discount activity. The business has a solid and predictable existing customer base, with **91.2%** of customers returning to purchase more than once, but urgently needs a structured strategy to grow that base. By combining purchase cycle forecasting with cluster-based personalised marketing, the business can maximise revenue from existing customers while building a sustainable pipeline of new ones.

---

## Tools Used

| Tool | Purpose |
|------|---------|
| **Python** | Analysis & Modelling |
| **Pandas** | Data Manipulation |
| **Matplotlib** | Data Visualisation |
| **Scikit-learn** | K-Means Clustering & StandardScaler |
| **Jupyter Notebook** | Development Environment |

---

## Why This Project Stands Out

- Covers the full analytical stack descriptive, diagnostic and predictive
- Identifies the true root cause of sales decline through systematic elimination of factors
- Delivers cluster-based personalised marketing recommendations grounded in data
- Demonstrates end-to-end analytical capability from raw data to actionable business strategy
