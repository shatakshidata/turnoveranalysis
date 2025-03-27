# 📊 Turnover Analysis

This repository contains the end-to-end analysis of employee turnover at XYZ Corp, aimed at supporting 2025 headcount planning through predictive and statistical analytics.

## 🧠 Problem Statement

XYZ aims to optimize hiring and retention strategies. We hypothesize that turnover is not uniform across departments, levels, and locations — and that certain groups (like hourly employees in S&OP) contribute disproportionately to attrition. 

## 🔍 Key Questions

- Which subgroups are most at risk of attrition?
- How do promotions, pay type transitions, and location influence tenure?
- Can we forecast attrition to inform 2025 hiring budgets?

---

## 📁 Data Overview

- **Timeframe:** May 2022 to Jan 2025 (panel format)
- **Scope:** Employees from 2018–2025
- **Features:** 
  - `employee_id`, `hire_date`, `effective_date`, `job_level`, `job_function`
  - `location`, `pay_rate_type` (Hourly/Salary), `role_volume_type`
  - Status flags like `turnover_flag`, `promotion_flag`, etc.

---

## 🧰 Methods & Tools

| Technique | Purpose |
|----------|---------|
| **Data Wrangling (pandas)** | Panel to cross-sectional transformation, time-lag features |
| **EDA & Viz (matplotlib, seaborn)** | Boxplots, heatmaps, tenure distributions |
| **ANOVA + Tukey HSD** | Statistical tests for tenure differences |
| **Chi-Square Tests** | Categorical significance for turnover |
| **Survival Analysis (lifelines)** | Kaplan-Meier & Cox models on tenure |
| **Time Series Forecast (Prophet)** | Department-level turnover projection for 2025 |
| **Fixed Effect Vs Random Effects** | Looking at within and between variations in panel data |
| **Scenario Testing** | "What-if" analysis: 10% reduction in turnover |
| **Dashboards** | Tableau and Power BI for stakeholder delivery |

---

## 📈 Results Snapshot

- **Strategy & Operations**: Lowest tenure; dominated by Hourly L2–L3 roles.
- **Hourly → Salary transitions**: Lead to improved retention.
- **L10 Engineers**: Unexpected mid-level turnover spike; requires deeper attention.
- **Locations like MoonMart 1 & 2**: Higher turnover due to S&OP-heavy staffing.
- **Cities like Seattle & NYC**: Engineering tenure lags behind other functions.

---

## 💡 Recommendations

- 🎯 Prioritize **retention for L10 Engineers** and senior technical talent.
- 🔄 Enable **Hourly→Salary internal mobility** — it's correlated with lower attrition.
- 📍 Deploy **location-specific strategies** in high-churn sites like MoonMart and Tempe.
- 📊 Use **forecasted data** to preempt hiring surges — especially in Strategy & Ops.
- 🧮 Consider **cost-benefit of attrition** vs. hourly-to-salaried transitions.


---

## 💼 Business Impact

This project enabled XYZ’s HR and Strategy teams to:
- Reduce reactive hiring by forecasting attrition hotspots.
- Improve internal mobility pathways via targeted role transitions.
- Elevate data-backed workforce decisions with clear visual storytelling.

---

## 🧑‍💻 Author

Shatakshi Bhatnagar  
Business Analyst | HR Data Science | Graph Analytics | LLM-based Modeling

---

