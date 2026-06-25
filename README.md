# Medicare Claims Cost & Utilization Analysis

## Business Question
*Which healthcare service types and geographic regions drive the highest Medicare spending, and where does utilization efficiency break down across the US market?*

This project analyzes 558,852 Medicare records from the CMS Market Saturation and Utilization Dataset to surface actionable insights for payers and health systems evaluating network performance, cost variation, and value-based care opportunities.

---


## Why This Matters
Medicare spends over $4.24 Trillion across service types and geographies — yet utilization rates and provider access vary dramatically across states, often without corresponding differences in care quality. Identifying high-cost, low-efficiency patterns is foundational to risk adjustment strategy, network optimization, and care management program design.

---

## Key Findings
- *$4.24 Trillion in total Medicare payments* analyzed across 17 service types and all US states
- *Independent Diagnostic Testing* drives the highest Medicare spend at $1.24 Trillion — 2x the next highest service category
- *California, Texas, and Florida* account for the top 3 states by total Medicare spending
- *Dual eligible beneficiaries* represent the highest-risk population segment requiring targeted care management intervention
- *22+ Million providers* analyzed across all US states revealing significant market saturation variation
- *Provider access gaps* identified in states with the highest beneficiary-to-provider ratios

---

## Python Analysis Highlights
- Loaded and cleaned 558,852 CMS Medicare records using pandas read_csv() and dropna()
- Performed grouped aggregations using groupby() to identify top states and service types by total payment
- Built dual eligible risk segmentation using percentage calculations across beneficiary populations
- Generated 4 analytical visualizations using Matplotlib identifying key cost drivers and utilization patterns
- Applied median imputation for missing dual eligible values using fillna() with specialty-level medians

---

## Data Quality Challenges
- Resolved 103,855 missing Dual Eligible values using median imputation across beneficiary populations
- Removed aggregated national totals (--ALL--) to enable accurate state-level analysis
- Handled 194 missing Total Payment records using targeted row exclusion
- Standardized inconsistent state identifiers across 558,852 records for geographic analysis

---

## Tools & Technologies
| Layer | Tool |
|---|---|
| Data Processing | Python (pandas, numpy) |
| Analysis | Python (Google Colab) |
| Visualization | Power BI, Tableau |
| Data Source | CMS Market Saturation and Utilization Dataset (Public) |

---

## Dashboard Features
- Service type drill-down by Medicare spending and utilization across 17 categories
- State-level cost variation analysis across all US states
- Dual eligible high-risk population identification and segmentation
- Provider access and market saturation analysis by state

**[View Tableau Dashboard](https://public.tableau.com/app/profile/lokesh.reddy2043/viz/MedicareUtilizationAnalysis/Dashboard1)**

---

## Analytical Approach
1. Ingested raw CMS public dataset (558,852 records, 32 fields)
2. Cleaned and standardized state, service type, payment, and dual eligible fields
3. Built calculated measures for utilization rates, dual eligible percentages, and total payment by geography
4. Designed dashboards for both executive summary and operational drill-down use cases

---

## Recommendations
- Prioritize care management resources toward dual eligible populations — highest-risk segment identified across all states
- Investigate Independent Diagnostic Testing utilization patterns — $1.24 Trillion spend warrants audit prioritization
- Develop provider access scorecards for states with lowest provider-to-beneficiary ratios to support network expansion decisions
- Monitor high-cost states exhibiting significant payment variation for network renegotiation opportunities
- Reallocating 10% of spending from low-efficiency service categories could generate estimated $424B+ in savings annually, supporting reinvestment into value-based care initiatives and care gap closure programs

---

## Domain Context
This analysis applies concepts central to *Medicare Advantage risk adjustment, **value-based care contracting, and **HEDIS/Stars program analytics* — areas where provider cost efficiency directly impacts plan performance and member outcomes.

---

## About
Built by *Lokesh Bayyapu*, PharmD, MS Health Data Science
Healthcare Data Analyst | Medicare Advantage & Population Health
[LinkedIn](https://www.linkedin.com/in/lokeshreddy1) | [Tableau Public](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)
