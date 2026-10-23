# Analyzer__

<div align="center">

<a href="https://github.com/chandnithadani960">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=217346&center=true&vCenter=true&width=700&lines=%F0%9F%94%B4+LIVE+Sales+Analyzer+Dashboard;%F0%9F%93%8A+200+Orders+%7C+7+Sheets+%7C+0+Macros;%E2%9A%A1+Live+Formulas+%E2%80%94+Update+Data%2C+Everything+Refreshes;%F0%9F%93%88+KPIs+%7C+Regression+%7C+What-If+%7C+Customer+Insights" alt="Live typing animation" />
</a>

# 🔴 LIVE · 📊 Sales Analyzer

<a id="an-interactive-formula-driven-excel-dashboard-for-sales-profit-customer-insights"></a>

### 🔴 LIVE · An interactive, formula-driven Excel dashboard for sales, profit & customer insights

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Formulas](https://img.shields.io/badge/100%25-Live_Formulas-blue?style=for-the-badge)
![Sheets](https://img.shields.io/badge/Sheets-7-orange?style=for-the-badge)
![Records](https://img.shields.io/badge/Orders-200-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-LIVE-brightgreen?style=for-the-badge&logo=statuspage&logoColor=white)

*Turn 200 raw orders into KPIs, charts, statistics, a regression model and a discount simulator — all without a single macro.*

</div>

---

<a id="table-of-contents"></a>

## 🔴 LIVE · 📑 Table of Contents

- [🔴 About the Project](#about-the-project)
- [🔴 Key Highlights](#key-highlights)
- [🔴 Workbook Structure](#workbook-structure)
- [🔴 Dashboard Preview](#dashboard-preview)
- [🔴 Sample Findings](#sample-findings)
- [🔴 Dataset Description](#dataset-description)
- [🔴 Excel Functions Used](#excel-functions-used)
- [🔴 How to Use](#how-to-use)
- [🔴 Skills Demonstrated](#skills-demonstrated)
- [🔴 Author](#author)

---

<a id="about-the-project"></a>

## 🔴 LIVE · 🎯 About the Project

**Sales Analyzer** is a complete business-analytics workbook built entirely in Microsoft Excel. It takes a transactional sales dataset (**200 orders, Apr 2024 – Apr 2025**) and converts it into a one-page executive dashboard, supported by customer segmentation, pivot-style summaries, descriptive statistics, a linear regression model and a what-if discount simulator.

Everything is **formula-driven** — change the data and every KPI, table, chart and written insight updates automatically.

---

<a id="key-highlights"></a>

## 🔴 LIVE · ✨ Key Highlights

| | Feature | Description |
|---|---|---|
| 📈 | **Executive Dashboard** | 12 KPI cards + 3 charts (bar, pie, line) on a single page |
| 🧠 | **Auto-written Insights** | 6 "data storytelling" sentences that rewrite themselves when data changes |
| 👥 | **Customer Analysis** | Ranking, tiers (*High Value* / *Regular*) and Top-10 leaderboard |
| 🧮 | **Pivot-style Summaries** | Region, Category and Region × Category tables built with `SUMIFS` |
| 🔮 | **What-If Simulator** | Test any discount rate and see the profit impact instantly |
| 📉 | **Regression Model** | Profit vs Sales with ANOVA, coefficients, p-values and a predictor |
| 📊 | **Descriptive Statistics** | ToolPak-style stats + histogram, written as live formulas |

---

<a id="workbook-structure"></a>

## 🔴 LIVE · 🗂️ Workbook Structure

```
📁 Analyzer.xlsx
│
├── 🏠 DASHBOARD          → KPIs, charts & key insights
├── 🔬 ANALYSIS           → Cleaned data + calculated columns
├── 👥 CUSTOMERS          → Customer ranking, tiers & Top-10 leaderboard
├── 📋 PIVOT TABLE        → Sales by Region, Category & Region × Category
├── 🎛️ WHAT IF            → Discount scenario & sensitivity table
├── 📐 REGRESSION         → Linear regression: Profit (Y) vs Sales (X)
└── 📊 DESCRIPTIVE STATS  → Mean, median, std. dev., skewness, kurtosis, histogram
```

<a id="sheet-by-sheet"></a>

### 🔴 LIVE · Sheet-by-sheet

<details>
<summary><b>🔴 LIVE · 🏠 DASHBOARD</b></summary>

- **Row 1 KPIs:** Total Sales · Total Orders · Total Profit · Profit Margin · Avg Order Value · Highest Sale
- **Row 2 KPIs:** Discount Given · Avg Discount · Top Customer · Best Region · Best Category · Best Month
- **Charts:** Bar chart, Pie chart, Monthly trend line chart
- **Key Insights:** 6 auto-generated sentences (top region, best category, best month, customer concentration, regression takeaway, discount what-if)
</details>

<details>
<summary><b>🔴 LIVE · 🔬 ANALYSIS</b></summary>

Pulls the raw dataset and adds calculated columns:

| Column | Formula idea |
|---|---|
| Discount Amount | `Sales × Discount` |
| Total Purchase | `Sales − Discount Amount` |
| Profit Margin | `Profit ÷ Sales` |
| Profit Status | `Profit` / `Break-even` / `Loss` (with conditional formatting) |
| Order Month | First day of the order's month (for trend analysis) |
| Timestamp | `NOW()` — shows when the report was last refreshed |
</details>

<details>
<summary><b>🔴 LIVE · 👥 CUSTOMERS</b></summary>

- Orders, Total Sales, Total Purchase, Total Profit and Avg Purchase per customer
- `RANK`-based leaderboard with **Customer Tier** flag
- 🟨 **Editable yellow cell** – change the Top-N cut-off for "High Value"
- Top-10 leaderboard with **% share of all purchases**; Top-10 rows highlighted green
</details>

<details>
<summary><b>🔴 LIVE · 📋 PIVOT TABLE</b></summary>

Three formula-driven tables (no manual refresh needed, unlike real PivotTables):
1. Sales & % share by **Region**
2. Sales & % share by **Product Category**
3. **Region × Category** cross-tab with grand totals
</details>

<details>
<summary><b>🔴 LIVE · 🎛️ WHAT IF</b></summary>

- 🟨 Enter a flat discount rate (default 10%)
- See the new discount cost, scenario profit and % change
- **Sensitivity table** for 0% – 30% discount, plus a line chart

> *Assumption: quantity sold and costs stay constant; only the discount changes.*
</details>

<details>
<summary><b>🔴 LIVE · 📐 REGRESSION</b></summary>

Replicates the Data Analysis ToolPak output using formulas: Multiple R, R², Adjusted R², Standard Error, ANOVA, coefficients with t-stats, p-values and 95% confidence intervals, a scatter chart with trendline, and a **🟨 prediction box** (enter a Sales value → get predicted Profit).
</details>

<details>
<summary><b>🔴 LIVE · 📊 DESCRIPTIVE STATS</b></summary>

For **Sales, Quantity and Profit**: mean, standard error, median, mode, std. deviation, variance, kurtosis, skewness, range, min, max, sum, count and 95% confidence level — plus a histogram.
</details>

---

<a id="dashboard-preview"></a>

## 🔴 LIVE · 🖼️ Dashboard Preview

> 💡 *Add your screenshots in a `/screenshots` folder and the images below will appear.*

| Dashboard | Regression | What-If |
|:---:|:---:|:---:|
| ![Dashboard](screenshots/dashboard.png) | ![Regression](screenshots/regression.png) | ![What-If](screenshots/whatif.png) |

---

<a id="sample-findings"></a>

## 🔴 LIVE · 🔎 Sample Findings

Results from the current dataset:

| Metric | Value |
|---|---|
| 💰 Total Sales | **195,218** |
| 🧾 Total Orders | **200** |
| 📈 Total Profit | **68,287** |
| 🎯 Profit Margin | **35.0%** |
| 🛒 Avg Order Value | **976** |
| 🏷️ Avg Discount | **9.9%** (19,273 given in total) |

**Headline insights**

1. 🌎 **West** is the top region (44,084 sales, 22.6% of total); **East** is the weakest.
2. 📚 **Books** lead all categories with 24.1% of sales; **Office Supplies** contribute least.
3. 📅 **Sep 2024** was the best month (20,534); **Apr 2025** the weakest.
4. 👑 The **Top 10 customers** generate **47.4%** of all purchases — **CUST015** is #1 (10,167).
5. 📐 **Regression:** `Profit = −1.03 + 0.3509 × Sales` with **R² = 0.60** (p < 0.05) — every extra 1 of sales adds ≈ 0.35 profit.
6. 🎛️ **What-if:** a flat 10% discount would change total profit by only **−0.4%**.

---

<a id="dataset-description"></a>

## 🔴 LIVE · 🗃️ Dataset Description

| Column | Type | Description |
|---|---|---|
| `Customer_ID` | Text | Unique customer code (e.g., CUST001) |
| `Customer_Name` | Text | Customer's name |
| `Region` | Category | Central · East · North · South · West |
| `Product_Category` | Category | Books · Clothing · Electronics · Furniture · Office Supplies |
| `Sales` | Number | Order value before discount |
| `Quantity` | Number | Units sold |
| `Discount` | % | Discount applied to the order |
| `Order_Date` | Date | Date of the order (10 Apr 2024 – 07 Apr 2025) |
| `Profit` | Number | Profit earned on the order |

---

<a id="excel-functions-used"></a>

## 🔴 LIVE · 🧰 Excel Functions Used

| Category | Functions |
|---|---|
| **Aggregation** | `SUM` `SUMIFS` `SUMPRODUCT` `COUNTA` `COUNTIF` `AVERAGE` |
| **Lookup** | `INDEX` `MATCH` |
| **Ranking** | `RANK` `LARGE` `MAX` `MIN` |
| **Logic** | `IF` `IFERROR` |
| **Date & Text** | `DATE` `YEAR` `MONTH` `NOW` `TEXT` |
| **Statistics** | `STDEV` `VAR` `MEDIAN` `MODE` `KURT` `SKEW` `TINV` |
| **Regression** | `SLOPE` `INTERCEPT` `RSQ` `CORREL` `STEYX` `LINEST` `FDIST` `TDIST` `DEVSQ` |
| **Visuals** | Conditional formatting · Bar / Pie / Line / Scatter charts · Merged KPI cards |

---

<a id="how-to-use"></a>

## 🔴 LIVE · 🚀 How to Use

1. **Download** `Analyzer.xlsx` and open it in Microsoft Excel (2016 or later recommended).
2. If prompted about **external links**, click **Update** (or *Enable Content*) so the dashboard can read the `Dataset` sheet.
3. Start on the **DASHBOARD** sheet for the big picture.
4. Play with the 🟨 **yellow input cells**:
   - `CUSTOMERS` → change the **Top N** cut-off
   - `WHAT IF` → change the **discount rate**
   - `REGRESSION` → enter any **Sales** value to predict Profit
5. To analyse your own data, replace the rows in the `Dataset` sheet (keep the same column order) — everything refreshes automatically.

> ⚠️ **Note:** The workbook formulas read from a sheet named `Dataset`. Keep this sheet (or the linked source file) in the same folder, otherwise Excel will show `#REF!` / link warnings.

---

<a id="skills-demonstrated"></a>

## 🔴 LIVE · 💡 Skills Demonstrated

- ✅ Data cleaning & calculated fields
- ✅ KPI design & dashboard storytelling
- ✅ Customer segmentation (RFM-style ranking)
- ✅ Dynamic, formula-based reporting
- ✅ Descriptive & inferential statistics
- ✅ Linear regression & hypothesis testing
- ✅ Scenario / sensitivity analysis
- ✅ Data visualization best practices

---

<a id="future-improvements"></a>

## 🔴 LIVE · 🔮 Future Improvements

- [ ] Add slicers for Region / Category / Month
- [ ] Add profit-by-category breakdown on the dashboard
- [ ] Multi-variable regression (Sales, Quantity, Discount → Profit)
- [ ] Forecasting with `FORECAST.ETS`
- [ ] Power Query / Power Pivot version

---

<a id="author"></a>

## 🔴 LIVE · 👩‍💻 Author

**Chandni Thadani**
📧 chandnithadani960@gmail.com

⭐ *If you found this project useful, please consider giving it a star!*

---

<div align="center">
Made with ❤️ and Excel
</div>
