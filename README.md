## Investment Trends Analysis (2020–2025)

**Author:** Fuzail Ahmed
**Domain:** Finance & Data Analytics  
**Platform:** Google Colab (Python)  
**Dataset:** [Finance Trends 2020–2025 (Kaggle)](https://www.kaggle.com/datasets/ayeshasiddiqa123/finance-trends-2020-2025/data)

---

## Overview
This repository presents an analytical study of investor behavior using a 12,000‑record dataset covering preferences, objectives, expected returns, and engagement patterns. The cohort is predominantly 18–34 years old, with a balanced interest in both market‑linked and sovereign/bank instruments. Findings are positioned for finance and data‑analysis audiences—emphasizing investor profiles, motivations, and implications for product and advisory strategy.

---

## Key Findings
- **Demographics:** Ages 18–38 (mean 27.8). Gender split ≈ **62.4% Male**, **37.6% Female**.  
- **Primary avenues (single‑choice `Avenue`):** Fixed Deposits, Mutual Funds, PPF, Equity (near‑balanced shares).  
- **Instrument preference scores (1–7):** High affinity for **Debentures** and **Government Bonds**, moderate for **Equity**/**Mutual Funds**.  
- **Objectives & purpose:** **Capital Appreciation** and **Wealth Creation** dominate; **Income** is least reported.  
- **Horizon & monitoring:** Even distribution across **<1 yr**, **1–3**, **3–5**, **>5** years; monitoring is evenly split across **daily/weekly/monthly**.  
- **Expected returns:** Mean ≈ **20%**, median = **20%**, band **10–30%**.

> Note: The dataset includes respondents up to age 38. Claims about older cohorts (45–65+) should be qualified or paired with external evidence.

---

## Insights & Implications
- **Product:** Offer blended, goal‑based portfolios (equity + short‑duration debt/PPF) suited to growth‑seeking yet stability‑valuing young investors.  
- **Advisory:** Align ~20% return expectations with appropriate **risk budgeting** and **time‑horizon** education.  
- **Distribution:** Strengthen **advisor channels**; complement with **digital literacy** content.  
- **Engagement:** Provide **goal tracking**, **SIP nudges**, and **rebalancing prompts** for an actively monitoring cohort.

---

## Dataset Snapshot
Columns: 24 | Rows: 12,000  
Selected fields:  
- **Demographics:** `Gender`, `Age` (derived `Age_Group`).  
- **Single‑choice preference:** `Avenue` (Equity, Mutual Fund, PPF, Fixed Deposits).  
- **Instrument scores (1–7):** `Mutual_Funds`, `Equity_Market`, `Debentures`, `Government_Bonds`, `Fixed_Deposits`, `PPF`, `Gold`.  
- **Behavioral/context:** `Factor`, `Objective`, `Purpose`, `Duration`, `Invest_Monitor`, `Source`.  
- **Outcome:** `Expect` (cleaned to numeric `%` as `Expect_clean`).

Data quality notes: `Stock_Marktet` (typo in source); `Investment_Avenues` is binary (Yes/No) while `Avenue` contains the instrument names.

---

## Repository Contents
- `Investment_Trends_Report_Syed_Moiz_Husain.docx` – full narrative report with tables.  
- `FinanceTrends_cleaned.csv` – optional cleaned export (create in notebook).  
- `notebooks/` – Google Colab notebook or exported `.ipynb` (your analysis).  
- `assets/` – charts (optional).

---

## How to Reproduce (lightweight)
1. Open the notebook in **Google Colab**.  
2. Install essentials:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly
   ```
3. Load the CSV (update the path as needed) and run cells sequentially.  
4. Optional: export cleaned data with `df.to_csv('FinanceTrends_cleaned.csv', index=False)`.

---

## Limitations
- Age coverage is limited to 18–38; do not generalize to 45–65+ without external data.  
- No income or ticket‑size variables; findings focus on **preferences and expectations**, not allocation weights.

---

## Author
Fuzail Ahmed
Finance & Data Analytics  
[LinkedIn](https://www.linkedin.com/in/fuzailibnahmed)

---

*If you find this analysis useful, please ⭐ the repository.*
