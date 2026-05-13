# E-Commerce Supply Chain Optimization
### Python · SQL · SQLite · Power BI · BRD

> Analyzing 100,000+ real e-commerce orders to identify supply chain 
> bottlenecks and deliver data-driven recommendations that protect 
> $19.8M in annual revenue at risk.

---

## Business Problem
ShopFast, a mid-sized e-commerce company, was experiencing rising fulfillment 
delays with no visibility into WHERE in the supply chain bottlenecks occurred. 
Manual reporting took 3 days to compile — making data stale before it reached 
management.

## Project Objective
Build a supply chain analytics solution that:
- Identifies top bottlenecks using SQL analysis on 100,000+ order records
- Tracks 6 operational KPIs including OTIF rate and fulfillment time
- Delivers an interactive Power BI dashboard for daily operations monitoring
- Provides 3 business recommendations with estimated revenue impact

---

## Tools & Technologies
| Tool | Purpose |
|------|---------|
| Python (pandas, matplotlib, seaborn) | Data loading, EDA, visualizations |
| SQL (SQLite) | KPI calculations, multi-table JOINs, CTEs |
| Power BI | Interactive supply chain dashboard |
| BRD | Business requirements documentation |

---

## Key Results
| KPI | Result |
|-----|--------|
| OTIF Rate | **92.15%** ✅ above 85% target |
| Avg Fulfillment Time | **12.48 days** |
| Order Cancellation Rate | **0.63%** ✅ |
| Worst Category Delay | **home_comfort: 16.67%** |
| Worst Seller Delay Rate | **32.10%** 🔴 |
| Annual Revenue At Risk | **$19.8M** 💥 |

---

## Project Structure
```
supply-chain-optimization/
│
├── 02_SupplyChain_Analysis.ipynb   ← Full SQL + EDA notebook
├── supply_chain_dashboard.csv      ← Final analytics dataset
├── supply_chain_dashboard.pbix     ← Power BI dashboard file
├── Screenshot 2026-05-13 145057.png        ← Dashboard preview
├── BRD_SupplyChain_ShopFast_ShrustiKhadji.docx
├── chart1_fulfillment_distribution.png
├── chart2_category_delays.png
├── chart3_otif_trend.png
└── chart4_seller_performance.png
└── README.md
```

---

## SQL Highlights
This project uses multi-table SQL JOINs across 9 relational tables:
- Calculated OTIF rate, delay rate, and fulfillment time using CTEs
- Identified top 10 worst-performing sellers by delay rate
- Analyzed delay patterns across 70+ product categories
- Flagged sellers with >25% delay rate for performance review

---

## Business Recommendations
1. **Seller performance scorecard** — Monthly OTIF thresholds with automated 
   warnings for sellers below 75% OTIF
2. **Category inventory buffer** — 20% safety stock increase for top 3 
   delay-prone categories during peak periods
3. **Regional fulfillment partner** — Northeast region fulfillment center 
   to reduce geographic delivery delays by 0.8 days

---

## Dashboard
[[View Power BI Dashboard →](https://app.powerbi.com/groups/me/reports/84df396c-f998-42bf-8a49-3951aae9080a/d7ab0c2432102de0e090?experience=power-bi)](#) 

---

## Business Requirements Document
Full BRD including stakeholder register, 6 KPI definitions, functional 
requirements, and success criteria available in files

---

*Dataset: Olist Brazilian E-Commerce Public Dataset (Kaggle) | Project by Shrusti Khadji*
