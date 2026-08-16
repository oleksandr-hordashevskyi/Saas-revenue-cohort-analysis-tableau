# 💳 SaaS Financial Performance & Cohort Retention Analytics

[![Tableau Public Badge](https://img.shields.io/badge/Tableau_Public-Interactive_Dashboard-orange?style=flat&logo=tableau)](https://public.tableau.com/app/profile/oleksandr.hordashevskyi/vizzes)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

An end-to-end financial and subscription analytics project modeling Monthly Recurring Revenue (MRR), New MRR acquisition dynamics, and cohort revenue retention using Tableau Desktop.

---

## 📌 Business Context & Objective
Subscription-based (SaaS) businesses require granular tracking of revenue streams and cohort behavior to optimize customer acquisition costs and predict Lifetime Value (LTV).

**Key Analytical Objectives:**
- Track monthly recurring revenue growth rates and decompose revenue streams.
- Isolate and calculate **New MRR** via first-payment month cohort filtering.
- Construct a dynamic **Cohort Revenue Matrix** to monitor long-term customer retention and monetization decay.
- Provide executive-level filtering across subscription tiers, acquisition channels, and time horizons.

---

## 🖼 Dashboard Preview

![SaaS Revenue Dashboard Preview](images/dashboard_preview.png)

🔗 **Interactive Live Version:** [Open Dashboard on Tableau Public](https://public.tableau.com/app/profile/oleksandr.hordashevskyi/vizzes)

---

## 🛠 Technical Implementation & Key Skills
- **BI Platform:** Tableau Desktop / Tableau Public
- **Level of Detail (LOD) Calculations:** Engineered `{FIXED [User ID] : MIN([Payment Month])}` expressions to isolate initial acquisition periods and calculate true New MRR.
- **Table Calculations:** Configured dynamic cohort decay formulas and period-over-period revenue Growth Rates.
- **Visual Design & Heatmaps:** Applied customized gradient scales with baseline normalization for intuitive cohort matrix readability.
- **Data Modeling:** Structured transactional billing logs into a cohort-ready reporting layer.

---

## 🔍 Key Insights & Findings
1. **New MRR Expansion:** Acquisition revenue showed strong compounding growth driven by initial promotional cycles.
2. **Cohort Decay Curve:** The sharpest retention drop occurs in Month 2–3 post-acquisition, stabilizing into predictable baseline ARR by Month 6.
3. **High-Yield Cohorts:** Specific seasonal cohorts demonstrated higher average revenue per user (ARPU), highlighting target acquisition windows for marketing.

---

## 📂 Repository Structure

```text
├── dashboards/                  <- Tableau Packaged Workbook (.twbx)
├── images/                      <- Dashboard screenshots & visual assets
│   └── dashboard_preview.png
├── LICENSE                      <- MIT License terms
└── README.md                    <- Analytical documentation & case study
