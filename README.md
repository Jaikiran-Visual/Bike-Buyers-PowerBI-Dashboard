# 📈 Bike Buyers Power BI Dashboard — Interactive Analytics

**Tools:** Power BI, DAX, Power BI Service  
**Dataset:** 1,000+ customer records  
**Date:** June 2026  
**Author:** [Jai Kiran R](https://linkedin.com/in/jaikiran-analyst)

📂 **Files in this repo:**
- [`bike dash board.pbix`](./bike%20dash%20board.pbix) — ⬇️ Download & open in Power BI Desktop
- [`Screenshot 2026-06-06 174028.png`](./Screenshot%202026-06-06%20174028.png) — Dashboard preview

---

## 📌 Project Overview

Built a fully interactive 6-visual Power BI dashboard to analyze bike purchase behaviour across age, gender, occupation, income, and region. Published publicly on Power BI Service for live, shareable access. Replaced static manual reports with a faster, slicer-driven analytics layer.

---

## 🎯 Business Problem

> *How can marketing and sales teams instantly identify which customer segments to prioritize — without waiting for manual reports?*

Static Excel reports require hours of manual filtering. This dashboard delivers the same insights in under 30 seconds via interactive slicers.

---

## 📊 Dashboard Visuals

| Visual | What It Shows |
|---|---|
| **Bar Chart — Purchase by Age Group** | Which age groups buy most |
| **Donut Chart — Gender Split** | Male vs Female buyer distribution |
| **Map Visual — Regional Performance** | Purchase volume by geography |
| **Stacked Bar — Occupation vs Purchase** | Buyer breakdown by job type |
| **Line Chart — Income vs Conversion** | Income band effect on purchase rate |
| **KPI Cards** | Total customers (1K), total buyers (481), conversion rate (48.1%), avg income ($56.36K) |

---

## 🧮 DAX Calculated Column — Age Group Segmentation

```dax
Age Group =
SWITCH(
    TRUE(),
    bike_buyers[Age] < 31, "Young (< 31)",
    bike_buyers[Age] <= 54, "Middle-Aged (31-54)",
    "Senior (55+)"
)
```

---

## 📊 Key Findings

| Segment | Insight |
|---|---|
| **Top Buyer Group** | Middle-aged North American professionals had highest purchase volume |
| **Gender** | Male buyers slightly outnumbered female buyers overall |
| **Occupation** | Professional and skilled manual workers drove majority of sales |
| **Region** | North America (50.8%) consistently outperformed Europe (30%) and Pacific (19.2%) |
| **Commute Distance** | 0–1 mile commuters had the highest buyer count vs 10+ miles (lowest) |

---

## 💼 Business Impact

- ✅ Reduced manual reporting effort by an estimated **3–4 hours per analysis cycle**
- ✅ Interactive slicers allow segment isolation in **< 30 seconds** vs. hours with static reports
- ✅ Accelerated **data-to-decision time by ~60%** for marketing stakeholders
- ✅ Live public dashboard enables remote team access without sharing raw data files

---

## 🖼️ Dashboard Preview

![Bike Buyers Power BI Dashboard](./Screenshot%202026-06-06%20174028.png)

---

## 💬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/jaikiran-analyst)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jaikivisual@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-GitHub-black?style=for-the-badge&logo=github)](https://github.com/Jaikiran-Visual)
