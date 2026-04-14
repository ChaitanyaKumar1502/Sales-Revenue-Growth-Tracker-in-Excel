# 📊 Sales & Revenue Growth Tracker in Excel

> **An industry-grade, job-ready Excel dashboard project for tracking sales performance, revenue growth, and business trends across regions, product categories, and time periods.**

---

## 🎯 Objective

To build a fully functional Excel-based Sales & Revenue Growth Tracker that helps sales managers, business analysts, and operations teams:
- Monitor real-time sales KPIs
- Visualize revenue trends by region, product, and time
- Compare actual performance vs targets
- Identify top-performing regions and products
- Support data-driven decision making

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Core tool — data, formulas, charts, dashboard |
| Pivot Tables | Data aggregation & summarization |
| Excel Charts | Visual analysis (Bar, Line, Pie, Column) |
| Slicers & Timelines | Interactive filtering |
| Conditional Formatting | Highlight performance gaps |
| Excel Formulas | KPI calculation (SUMIFS, XLOOKUP, IF, etc.) |

---

## 📁 Project Folder Structure

```
Sales-Revenue-Growth-Tracker/
│
├── 📊 Sales_Revenue_Growth_Tracker.xlsx    ← Main Excel file
├── 📄 README.md                            ← This file
├── 📸 screenshots/
│   ├── dashboard_overview.png
│   ├── kpi_summary.png
│   ├── revenue_by_region.png
│   └── pivot_tables.png
└── 📋 Sales_Project_Guide.docx             ← Full step-by-step guide
```

---

## 📊 Dataset Description

The dataset contains **657 real-world style sales transactions** from January–December 2024 across India.

| Column | Description |
|--------|-------------|
| Order ID | Unique transaction identifier |
| Date | Transaction date (DD-MM-YYYY) |
| Month | Month-Year label |
| Region | North / South / East / West |
| City | State/city of the transaction |
| Sales Executive | Name of the sales rep |
| Product Category | Electronics, Furniture, Apparel, Software |
| Product Name | Specific product |
| Units Sold | Quantity sold per order |
| Selling Price (₹) | Price per unit |
| Revenue (₹) | Units Sold × Selling Price |
| Cost (₹) | Cost of goods sold |
| Profit (₹) | Revenue − Cost |
| Customer Type | New / Existing |
| Sales Channel | Online / Offline |
| Target Sales (₹) | Monthly sales target |
| Achievement % | Revenue / Target × 100 |

---

## 📑 Sheet Structure

| Sheet | Purpose |
|-------|---------|
| `Raw_Data` | Original unmodified sales dataset (657 rows) |
| `Cleaned_Data` | Formula-linked clean dataset with Profit Margin % added |
| `KPI_Summary` | Key performance indicators + Regional & Category breakdown |
| `Formulas_Guide` | All Excel formulas explained with examples |
| `Dashboard` | Visual dashboard with KPI cards and 4 charts |
| `Pivot_Guide` | Step-by-step pivot table & chart creation guide |

---

## 📐 Key Excel Formulas Used

```excel
-- Total Revenue
=SUM(Cleaned_Data!K2:K658)

-- Revenue by Region (North example)
=SUMIF(Cleaned_Data!D:D,"North",Cleaned_Data!K:K)

-- Achievement %
=K2/P2

-- Profit Margin %
=IFERROR(M2/K2, 0)

-- Month-over-Month Growth %
=(CurrentMonth - PreviousMonth) / PreviousMonth

-- Average Achievement
=AVERAGE(Cleaned_Data!Q2:Q658)

-- XLOOKUP example
=XLOOKUP(A2, Raw_Data!A:A, Raw_Data!F:F)

-- Forecasting next month
=FORECAST.ETS(13, B2:B13, A2:A13)
```

---

## 📈 Key KPIs Tracked

- ✅ **Total Revenue** — Full-year revenue sum
- ✅ **Total Profit** — Full-year net profit
- ✅ **Total Orders** — Count of transactions
- ✅ **Total Units Sold** — Volume metric
- ✅ **Average Achievement %** — Target attainment rate
- ✅ **Online vs Offline Revenue** — Channel split
- ✅ **Revenue by Region** — North, South, East, West
- ✅ **Revenue by Category** — Electronics, Furniture, Apparel, Software

---

## 📊 Dashboard Visuals

| Chart | Type | Insight |
|-------|------|---------|
| Revenue by Region | Column Chart | Which region drives most revenue |
| Revenue by Category | Horizontal Bar | Best-performing product category |
| Sales Channel Distribution | Pie Chart | Online vs Offline split |
| Revenue vs Profit by Region | Clustered Column | Profitability comparison |

---

## 💡 Business Insights

Based on the dataset, the dashboard reveals:

- **South and North regions** typically generate the highest revenue due to metro concentration
- **Software category** has the highest profit margin (~70%) despite lower order volume
- **Online channel** drives higher order frequency; Offline drives higher ticket size
- **Electronics** dominates revenue volume due to high unit prices
- Sales executives with consistent achievement >100% are candidates for incentive programs

---

## 🖥️ Dashboard Layout

```
┌─────────────────────────────────────────────────────────┐
│         SALES & REVENUE GROWTH TRACKER — 2024          │
├──────────┬──────────┬──────────┬──────────┬────────────┤
│ TOTAL    │ TOTAL    │ TOTAL    │ UNITS    │ AVG ACHIEV │
│ REVENUE  │ PROFIT   │ ORDERS   │ SOLD     │ MENT %     │
├──────────┴──────────┼──────────┴──────────┴────────────┤
│ [Column Chart]      │ [Bar Chart]                       │
│ Revenue by Region   │ Revenue by Category               │
├─────────────────────┼───────────────────────────────────┤
│ [Pie Chart]         │ [Clustered Column]                │
│ Channel Split       │ Revenue vs Profit by Region       │
└─────────────────────┴───────────────────────────────────┘
```

---

## 📸 Screenshots

> Add your dashboard screenshots here after opening the Excel file.

```markdown
![Dashboard Overview](screenshots/dashboard_overview.png)
![KPI Summary](screenshots/kpi_summary.png)
![Revenue by Region](screenshots/revenue_by_region.png)
```

---

## 🚀 How to Use This Project

1. **Download** `Sales_Revenue_Growth_Tracker.xlsx`
2. **Open in Microsoft Excel** (2016 or later recommended)
3. Navigate to the **Dashboard** sheet to view charts and KPIs
4. Visit **KPI_Summary** for detailed breakdowns
5. Check **Formulas_Guide** to understand all calculations
6. Follow **Pivot_Guide** to recreate pivot tables yourself
7. Add your own data to **Raw_Data** — all formulas auto-update!

---

## 📝 Resume-Ready Project Descriptions

**One-Line Version:**
> Built a Sales & Revenue Growth Tracker in Excel with KPI dashboard, pivot analysis, and dynamic charts for 657 transactions across 4 regions and 4 product categories.

**2–3 Line Version:**
> Designed an advanced Excel-based Sales & Revenue Tracker analyzing 657+ transactions across regions, product categories, and sales channels. Implemented SUMIFS, XLOOKUP, and Pivot Tables to calculate KPIs including Total Revenue, Profit Margin, and Achievement %. Built an interactive dashboard with 4 chart types and conditional formatting for executive-level reporting.

**ATS-Friendly Version:**
> Developed a Sales & Revenue Growth Tracker in Microsoft Excel using advanced functions (SUMIFS, XLOOKUP, INDEX-MATCH, IFERROR) to analyze 657 sales transactions across 4 regions and 4 product categories. Created KPI Summary sheet tracking Total Revenue, Profit, Units Sold, and Achievement %; built interactive dashboard with column, bar, line, and pie charts. Applied conditional formatting, structured sheet architecture, and pivot table analysis to deliver business-ready reporting tool used for sales performance management and decision-making.

---

## ✅ GitHub Pre-Publish Checklist

- [ ] Excel file opens without errors
- [ ] All formulas calculate correctly (no #REF!, #DIV/0! errors)
- [ ] Dashboard charts are visible and properly labelled
- [ ] README.md is complete with all sections
- [ ] Screenshots folder has at least 2-3 dashboard images
- [ ] Repository is set to **Public**
- [ ] Repository description is filled in
- [ ] Relevant topics/tags added to the repo

---

## 🔗 Connect With Me

> https://www.linkedin.com/in/chaitanya-kumar-masagalla-45261a355/
> chaitanyakumarmasagalla@gmail.com
> https://github.com/ChaitanyaKumar1502

---

## 📌 Conclusion

This project demonstrates hands-on proficiency in Excel for business analytics — from raw data structuring to dashboard creation. It mirrors the kind of reporting tool used by Sales Analysts, Business Analysts, and Revenue Managers in companies like Unilever, Deloitte, Amazon, and Nestlé. Ideal for MBA students, data analytics learners, and anyone building a job-ready portfolio.

---

*Built with ❤️ using Microsoft Excel | Dataset: Simulated 2024 India Sales Data*
