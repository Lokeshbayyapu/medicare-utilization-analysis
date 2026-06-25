# Medicare Claims Cost & Utilization Analysis

## Business Question
*Which provider specialties and geographic regions drive the highest Medicare spending, and where does reimbursement efficiency break down?*

This project analyzes 9.7M+ Medicare Part B claims records from CMS to surface actionable insights for payers and health systems evaluating network performance, cost variation, and value-based care opportunities.

---

## Why This Matters
Medicare spends over $900B annually, yet reimbursement rates vary dramatically across providers and geographies — often without corresponding differences in quality. Identifying high-cost, low-efficiency patterns is foundational to risk adjustment strategy, network optimization, and ACO performance management.

---

## Key Findings
- *Identified $2.3B in annual allowed amounts* concentrated among the top 10% of providers across all specialties
- *Geographic variation* in average reimbursement exceeds 40% across states for identical HCPCS procedures
- *Specialist billing patterns* show higher charge-to-payment ratios compared to primary care, with significant outliers in surgical subspecialties
- *HCPCS code clustering* reveals opportunities to flag anomalous utilization patterns for audit prioritization

---

## Python Analysis Highlights
- Ranked providers by allowed amount within specialty using pandas rank() and groupby()
- Identified top decile providers using quantile(0.9) for concentration analysis
- Built reimbursement efficiency ratio (avg Medicare payment ÷ avg submitted charge)
- Performed HCPCS-level aggregation and provider-level trend analysis using pivot_table()

---

## Data Quality Challenges
- Resolved inconsistent provider specialty classifications across multiple CMS extracts
- Standardized HCPCS reporting formats and removed duplicate NPI entries
- Handled missing reimbursement values using specialty-level median imputation

---

## Tools & Technologies
| Layer | Tool |
|---|---|
| Data Processing | Python (pandas, numpy) |
| Analysis | Python (Google Colab) |
| Visualization | Power BI, Tableau |
| Data Source | CMS Medicare Provider Utilization & Payment Data (Public) |

---

## Dashboard Features
- Provider-level drill-down by specialty, state, and HCPCS code
- Reimbursement efficiency ratio (avg Medicare payment ÷ avg submitted charge)
- Geographic heat maps of cost variation
- Top/bottom provider benchmarking by allowed amount per service

**[View Tableau Dashboard](https://public.tableau.com/app/profile/lokesh.reddy2043/viz/MedicareUtilizationAnalysis/Dashboard1)**

---

## Analytical Approach
1. Ingested raw CMS public dataset (~9.7M records, 25+ fields)
2. Cleaned and standardized provider, HCPCS, and geography fields
3. Built calculated measures for reimbursement efficiency, utilization rate, and cost per beneficiary
4. Designed dashboards for both executive summary and operational drill-down use cases

---

## Recommendations
- Prioritize audit review for providers with reimbursement efficiency ratios below threshold
- Investigate high-cost states exhibiting >40% payment variation for network renegotiation
- Develop provider scorecards to support network contracting discussions
- Monitor high-utilization HCPCS clusters for potential overuse patterns

---

## Domain Context
This analysis applies concepts central to *Medicare Advantage risk adjustment, **value-based care contracting, and **HEDIS/Stars program analytics* — areas where provider cost efficiency directly impacts plan performance and member outcomes.

---

## About
Built by *Lokesh Bayyapu*, PharmD, MS Health Data Science  
Healthcare Data Analyst | Medicare Advantage & Population Health  
[LinkedIn](https://www.linkedin.com/in/lokeshreddy1) | [Tableau Public](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)
