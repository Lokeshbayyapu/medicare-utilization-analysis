# Medicare Claims Cost & Utilization Analysis

## Business Question
*Which provider specialties and geographic regions drive the highest Medicare spending, and where does reimbursement efficiency break down?*

This project analyzes 9.7M+ Medicare Part B claims records from CMS to surface actionable insights for payers and health systems evaluating network performance, cost variation, and value-based care opportunities.

---

## Why This Matters
Medicare spends over $900B annually, yet reimbursement rates vary dramatically across providers and geographies — often without corresponding differences in quality. Identifying high-cost, low-efficiency patterns is foundational to risk adjustment strategy, network optimization, and ACO performance management.

---

## Key Findings
- *Top 10% of providers* account for a disproportionate share of total Medicare allowed amounts, signaling concentration risk
- *Geographic variation* in average reimbursement per service exceeds 40% across states for the same procedure codes
- *Specialist billing patterns* show higher charge-to-payment ratios compared to primary care, with significant outliers in surgical subspecialties
- *HCPCS code clustering* reveals opportunities to flag anomalous utilization patterns for audit prioritization

---

## Tools & Technologies
| Layer | Tool |
|---|---|
| Data Processing | Python (pandas, numpy) |
| Analysis | SQL, DAX |
| Visualization | Power BI, Tableau |
| Data Source | CMS Medicare Provider Utilization & Payment Data (Public) |

---

## Dashboard Features
- Provider-level drill-down by specialty, state, and HCPCS code
- Reimbursement efficiency ratio (avg Medicare payment ÷ avg submitted charge)
- Geographic heat maps of cost variation
- Top/bottom provider benchmarking by allowed amount per service

**[View Tableau Dashboard](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)**

---

## Analytical Approach
1. Ingested raw CMS public dataset (~9.7M records, 25+ fields)
2. Cleaned and standardized provider, HCPCS, and geography fields
3. Built calculated measures for reimbursement efficiency, utilization rate, and cost per beneficiary
4. Designed dashboards for both executive summary and operational drill-down use cases

---

## Domain Context
This analysis applies concepts central to *Medicare Advantage risk adjustment, **value-based care contracting, and **HEDIS/Stars program analytics* — areas where provider cost efficiency directly impacts plan performance and member outcomes.

---

## About
Built by *Lokesh Bayyapu*, PharmD, MS Health Data Science  
Healthcare Data Analyst | Medicare Advantage & Population Health  
[LinkedIn](https://www.linkedin.com/in/lokeshreddy1) | [Tableau Public](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)

--
