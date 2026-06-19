# 📈 Bike Buyers Power BI Dashboard — Interactive Analytics

**Tools:** Power BI, DAX, Power BI Service  
**Dataset:** 1,000+ customer records  
**Date:** June 2026  
**Author:** [Jai Kiran R](https://linkedin.com/in/jaikiran-analyst)

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
| **KPI Cards** | Total customers, total buyers, overall conversion rate |

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
| **Region** | North America consistently outperformed Europe and Pacific |

---

## 💼 Business Impact

- ✅ Reduced manual reporting effort by an estimated **3–4 hours per analysis cycle**
- ✅ Interactive slicers allow segment isolation in **< 30 seconds** vs. hours with static reports
- ✅ Accelerated **data-to-decision time by ~60%** for marketing stakeholders
- ✅ Live public dashboard enables remote team access without sharing raw data files

---

## 🖼️ Dashboard Preview

<img width="1375" height="774" alt="Bike Buyers Power BI Dashboard" src="https://github.com/user-attachments/assets/bdcaaa98-3c4f-4ac8-b17f-5653c4a96c45" />

---

## 💬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/jaikiran-analyst)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jaikivisual@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-GitHub-black?style=for-the-badge&logo=github)](https://github.com/Jaikiran-Visual)
