# SaaS Revenue & Churn Analysis

## Overview

This project focuses on analyzing subscription and revenue data for a B2B SaaS company to understand churn patterns, revenue trends, and unit economics. The goal is to move beyond surface-level metrics and identify what is actually driving customer attrition — and where the business has the strongest opportunity to improve retention and profitability.

The dataset covers CloudTask Pro, a project management platform that has grown to 600 customers since 2022. Despite consistent revenue growth, churn has become a concern at the leadership level. This analysis was built to give the CFO and board a clear, data-backed picture of the business heading into their next review.

---

## Objectives

- Understand how churn has trended month over month across four years and whether the situation is improving
- Identify which subscription plans and billing cycles carry the highest churn risk
- Surface the most common reasons customers leave and examine whether those reasons vary by plan or company size
- Calculate Customer Lifetime Value (CLV) and compare it against Customer Acquisition Cost (CAC) to assess the profitability of each plan tier
- Define a feature usage threshold that flags at-risk customers and estimate the current exposure

---

## Dataset

**`subscriptions.csv`**
Customer-level records including subscription plan, billing cycle, acquisition channel, company size, NPS score, feature usage percentage, and churn status.

**`monthly_revenue.csv`**
Monthly summary of new MRR, churned MRR, and net revenue from 2022 through the present.

---

## Tools

- **SQL** — core analysis, segmentation, and metric calculations
- **Excel** — summary tables and exploratory checks
- **Power BI** — dashboard and visual reporting for stakeholders

---

## Methodology

The analysis was structured in five stages.

**Data Exploration** — Both datasets were loaded and reviewed for completeness. Field definitions were confirmed, missing values were assessed, and the overall shape of the customer base was mapped before any calculations were run.

**Churn Analysis** — Churn rates were calculated across multiple dimensions: plan type, billing cycle, acquisition channel, and company size. This segmentation was essential for identifying which groups were driving the overall churn number versus which were relatively stable.

**Revenue Trends** — Monthly MRR was tracked over time and net revenue retention was calculated by subtracting churned MRR from new MRR each month. Periods with notable movement were flagged for closer review.

**Unit Economics** — Average CLV was computed per plan using average MRR and average customer lifespan. This was then compared against CAC to produce a CLV:CAC ratio for each plan — a clearer measure of long-term profitability than revenue alone.

**At-Risk Segmentation** — Feature usage and NPS scores were analyzed in relation to churn outcomes. A usage threshold was defined to identify customers at elevated risk of churning, and the number of current active customers falling below that threshold was estimated.
