# Marketplace Startup Health Analysis  
**End-to-End Case Study on Growth, Retention, Unit Economics, and Scaling Strategy**

## Overview
This project analyzes a fictional labour marketplace startup using worker-level activity data and income statement data.  
The objective is to evaluate overall business health and answer core diligence questions around:

- Growth quality (MAW, Revenue, MoM trends)
- Worker retention (cohort analysis)
- Unit economics (LTV, CAC, LTV/CAC)
- Scaling readiness (market-level performance and EBITDA implications)

---

## Business Context
The startup operates a two-sided marketplace:
- Employers post/pay for shifts
- Workers fulfill shifts and are paid by the platform
- The platform earns **net take** per job

The analysis examines whether growth is becoming more efficient over time and which strategic levers could improve the path to profitability.

---

## Key Questions Solved

Q1 — How is the business trending?

- Tracked Monthly Active Workers (MAW), Revenue, and MoM growth

- Assessed whether growth is smooth vs bursty

- Built productivity and monetization indicators:

- take_rate = net_take / revenue

- revenue_per_active_worker

- net_take_per_active_worker

Q2 — What does worker retention look like?

- Built cohort retention matrix using first active month as cohort

- Calculated months since cohort and blended (weighted) retention curve

- Identified high early churn and long-tail retained worker base

Q3 — Are unit economics sustainable?

- Estimated LTV6 and LTV12 using:

- weighted retention by cohort age

- net take/revenue per active worker by cohort age

- Computed blended CAC from worker marketing spend / new workers

- Evaluated:

  - LTV6/CAC

  - LTV12/CAC

- conservative gross-margin adjusted LTV/CAC

Q4 — What is interesting if the company scales?

- Compared market-level LTV (6-month and 12-month) by acquisition market

- Linked financial scaling trends (Revenue vs EBITDA, worker-pay pressure)

- Proposed a scale roadmap focused on high-LTV, high-volume markets first

---

## Data Engineering

- Standardized monthly time keys and cohort logic

- Built worker-month panel with active flag

- Aggregated financial line items into month-level analysis views

## Analytical Framework

- Cohort retention and retention curve analysis

- Unit economics framework: LTV, CAC, payback lens

- Market segmentation for prioritization under scaling constraints

- Profitability pressure diagnostics using income statement trends

---

## Main Insights (Summary)

- Growth is strong but volatile — MAW and revenue scale up, with bursty MoM patterns.

- Early churn is the biggest leak — retention drops quickly in the first few months, then stabilizes into a long-tail core.

- Unit economics are workable over 12 months — LTV/CAC improves meaningfully by month 12 vs month 6.

- Scaling is not automatically margin accretive — revenue growth currently coincides with more negative EBITDA, so retention, take rate, and acquisition efficiency are key to break-even path.

---

## Tech Stack

- Python: pandas, numpy, matplotlib

- Excel / Google Sheets: validation, financial views, quick pivots

- Slides: case narrative and executive synthesis

---

## Notes

- This is a case-study simulation for analytical practice.

- Company/data are fictional and used only for structured business analysis.
