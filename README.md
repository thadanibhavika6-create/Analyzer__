# Analyzer__

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b3d2a,50:107c41,100:33c481&height=260&section=header&text=SALES%20ANALYZER&fontSize=56&fontColor=ffffff&stroke=0b3d2a&strokeWidth=1&animation=twinkling&fontAlignY=36&desc=Excel%20Dashboard%20%7C%20KPIs%20%7C%20Regression%20%7C%20What-If&descAlignY=58&descSize=19" width="100%"/>

<img src="https://readme-typing-svg.demolab.com/?lines=Sales+Analyzer+Dashboard;7+Sheets+%E2%80%A2+200+Orders+%E2%80%A2+0+Macros;KPIs+%7C+Regression+%7C+What-If+%7C+Customer+Insights;Live+formulas+%E2%80%94+change+data%2C+everything+refreshes;Sales+%E2%80%A2+Profit+%E2%80%A2+Customers+%E2%80%A2+Statistics&font=Fira+Code&center=true&width=700&height=45&color=107C41&vCenter=true&size=22&pause=1200"/>

<br/>

![Excel](https://img.shields.io/badge/Microsoft-Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Sheets](https://img.shields.io/badge/Worksheets-7-1f6feb?style=for-the-badge)
![Orders](https://img.shields.io/badge/Orders-200-8957e5?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Intermediate-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

</div>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Project%20Overview&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Project Overview"/>
</div>

**Sales Analyzer** is a hands-on Excel project (`Analyzer.xlsx`) that turns **200 raw sales orders (Apr 2024 – Apr 2025)** into a one-page executive dashboard, backed by customer segmentation, pivot-style summaries, descriptive statistics, a **linear regression model** and a **what-if discount simulator**. Each sheet answers real business questions such as *"Which region earns the most?"*, *"Who are our top customers?"* and *"What happens to profit if we change the discount?"*

Everything is **formula-driven with zero macros** — change the data and every KPI, chart, table and written insight updates automatically.

> 📸 *Add your dashboard screenshot here:* `![Dashboard](screenshots/dashboard.png)`

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Workbook%20Structure&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Workbook Structure"/>
</div>


| # | Sheet | Records | What it covers |
|:-:|---|:-:|---|
| 1 | 🏠 `DASHBOARD` | 12 KPIs | KPI cards, 3 charts, 6 auto-written insights |
| 2 | 🔬 `ANALYSIS` | 200 | Cleaned data + calculated columns |
| 3 | 👥 `CUSTOMERS` | 30 | Ranking, tiers, Top-10 leaderboard |
| 4 | 📋 `PIVOT TABLE` | 3 tables | Sales by Region, Category & Region × Category |
| 5 | 🎛️ `WHAT IF` | 7 rates | Discount scenario & sensitivity table |
| 6 | 📐 `REGRESSION` | 200 | Profit vs Sales model with ANOVA & predictor |
| 7 | 📊 `DESCRIPTIVE STATS` | 3 vars | Full statistics + histogram |

### 1️⃣ `DASHBOARD`
| Section | Description |
|---|---|
| KPI Row 1 | Total Sales · Total Orders · Total Profit · Profit Margin · Avg Order Value · Highest Sale |
| KPI Row 2 | Discount Given · Avg Discount · Top Customer · Best Region · Best Category · Best Month |
| Charts | Bar chart, Pie chart, Monthly trend line chart |
| Key Insights | 6 "data storytelling" sentences that rewrite themselves when data changes |

### 2️⃣ `ANALYSIS`
| Column | Description |
|---|---|
| Discount Amount | `Sales × Discount` |
| Total Purchase | `Sales − Discount Amount` |
| Profit Margin | `Profit ÷ Sales` |
| Profit Status | `Profit` / `Break-even` / `Loss` with conditional formatting |
| Order Month | First day of the order month, used for trends |
| Timestamp | `NOW()` — shows when the report was last refreshed |

### 3️⃣ `CUSTOMERS`
| Feature | Description |
|---|---|
| Customer metrics | Orders, Total Sales, Total Purchase, Total Profit, Avg Purchase per order |
| Rank & Tier | `RANK`-based, flagged **High Value** or **Regular** |
| 🟨 Top-N cell | Editable yellow cell to change the High-Value cut-off |
| Leaderboard | Top 10 with % share of all purchases, highlighted green |

### 4️⃣ `PIVOT TABLE`
Three `SUMIFS` tables that refresh automatically: **Region**, **Product Category** and a **Region × Category** cross-tab with grand totals.

### 5️⃣ `WHAT IF`
Enter any flat discount rate (🟨 default 10%) to see the new discount cost, scenario profit and % change, plus a **0%–30% sensitivity table** and line chart.

### 6️⃣ `REGRESSION`
ToolPak-style output built with live formulas: Multiple R, R², Adjusted R², Standard Error, ANOVA, coefficients, t-stats, p-values, 95% confidence intervals, a scatter chart and a **🟨 prediction box**.

### 7️⃣ `DESCRIPTIVE STATS`
For **Sales, Quantity and Profit**: mean, standard error, median, mode, std. deviation, variance, kurtosis, skewness, range, min, max, sum, count, 95% confidence level and a histogram.

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Features%20%2F%20Operations%20Covered&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Features / Operations Covered"/>
</div>


<table>
<tr>
<td width="50%" valign="top">

**🔹 Aggregation & Lookup**
- `SUMIFS` for region / category / customer totals
- `SUMPRODUCT` for weighted average discount
- `COUNTIF`, `COUNTA`, `AVERAGE`
- `INDEX` + `MATCH` for "Best Region / Category / Month"

</td>
<td width="50%" valign="top">

**🔹 Ranking & Logic**
- `RANK` and `LARGE` for Top-10 leaderboard
- `IF` for Profit Status and Customer Tier
- `IFERROR` for safe results
- Conditional formatting highlights

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🔹 Statistical & Regression**
- `STDEV`, `VAR`, `MEDIAN`, `MODE`, `KURT`, `SKEW`
- `SLOPE`, `INTERCEPT`, `RSQ`, `CORREL`, `STEYX`, `LINEST`
- `FDIST`, `TDIST`, `TINV`, `DEVSQ`

</td>
<td width="50%" valign="top">

**🔹 Date, Text & Visuals**
- `DATE`, `YEAR`, `MONTH`, `NOW`, `TEXT`
- Auto-generated insight sentences
- Bar, Pie, Line and Scatter charts
- Merged-cell KPI cards

</td>
</tr>
</table>

### 🧮 Analysis Results

| Sheet | Task | Function | Result |
|---|---|---|:-:|
| Dashboard | Total sales | `SUM` | **195,218** |
| Dashboard | Total profit | `SUM` | **68,287** |
| Dashboard | Profit margin | `Profit ÷ Sales` | **35.0%** |
| Dashboard | Average order value | `Sales ÷ Orders` | **976** |
| Dashboard | Average discount | `SUMPRODUCT` | **9.9%** |
| Customers | Top customer | `INDEX` + `MATCH` | **CUST015** |
| Customers | Top-10 share of purchases | `LARGE` | **47.4%** |
| Regression | R² (Profit vs Sales) | `RSQ` | **0.60** |
| Regression | Slope | `SLOPE` | **0.3509** |
| What-If | Profit change at 10% flat discount | Scenario | **−0.4%** |

**📐 Regression equation:** `Profit = −1.03 + 0.3509 × Sales` *(p < 0.05)*

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Dataset%20Description&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Dataset Description"/>
</div>


| Column | Description |
|---|---|
| Customer_ID, Customer_Name | Unique customer code and name |
| Region | Central · East · North · South · West |
| Product_Category | Books · Clothing · Electronics · Furniture · Office Supplies |
| Sales | Order value before discount |
| Quantity | Units sold |
| Discount | Discount % applied to the order |
| Order_Date | 10 Apr 2024 – 07 Apr 2025 |
| Profit | Profit earned on the order |

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Tech%20Stack&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Tech Stack"/>
</div>


![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![Formulas](https://img.shields.io/badge/Live_Formulas-33c481?style=flat-square)
![Charts](https://img.shields.io/badge/Charts-107c41?style=flat-square)
![Regression](https://img.shields.io/badge/Regression-1f6feb?style=flat-square)
![Conditional Formatting](https://img.shields.io/badge/Conditional_Formatting-8957e5?style=flat-square)

> ⚠️ **Note:** The formulas read from a sheet named `Dataset`. Keep it (or the linked source file) with the workbook, otherwise Excel shows link warnings or `#REF!`.

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=How%20to%20Run&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="How to Run"/>
</div>


1. Download or clone this repository.
2. Open `Analyzer.xlsx` in Microsoft Excel (2016 or later).
3. If asked about external links, click **Update / Enable Content**.
4. Start on the `DASHBOARD` sheet, then explore other sheets from the tabs.
5. Try the 🟨 yellow cells: Top-N in `CUSTOMERS`, discount rate in `WHAT IF`, Sales value in `REGRESSION`.
6. Replace the rows in `Dataset` (same column order) to analyse your own data.

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Sample%20Insights&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Sample Insights"/>
</div>


- 🌎 **West** is the top region (44,084 sales, 22.6%); **East** is the weakest
- 📚 **Books** lead all categories with 24.1% of sales
- 📅 **Sep 2024** was the best month (20,534); **Apr 2025** the weakest
- 👑 **Top 10 customers** generate 47.4% of purchases; **CUST015** is #1 (10,167)
- 📐 Every extra 1 of Sales adds about **0.35 profit** (R² = 0.60)
- 🎛️ A flat 10% discount would change total profit by only **−0.4%**

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=File%20Structure&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="File Structure"/>
</div>


```
📦 Sales-Analyzer
 ┣ 📄 Analyzer.xlsx   # Main workbook (7 sheets)
 ┣ 📁 screenshots     # Dashboard images
 ┗ 📄 README.md       # Project documentation
```

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Future%20Improvements&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Future Improvements"/>
</div>


- [ ] Add slicers for Region / Category / Month
- [ ] Add profit-by-category breakdown on the dashboard
- [ ] Multi-variable regression (Sales, Quantity, Discount → Profit)
- [ ] Forecasting with `FORECAST.ETS`
- [ ] Build a Power Query / Power Pivot version

<br/>

<div align="center">

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=110&section=header&text=Author&fontSize=28&fontColor=ffffff&fontAlignY=38&animation=twinkling" width="100%" alt="Author"/>
</div>

**Bhavika Thadani**

Made with ❤️ to turn raw sales data into live business insights.

⭐ **If you found this project useful, consider giving it a star!**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:107c41,100:33c481&height=120&section=footer&text=Thanks%20for%20visiting!&fontSize=24&fontColor=ffffff&animation=twinkling&fontAlignY=65" width="100%"/>

</div>
