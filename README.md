# Sales-Analysis-Dashboard
# 📊 Sales Performance Dashboard — Power BI

An end-to-end sales analytics project built with **Power BI**, **Excel**, and **Python**.  
Covers revenue trends, regional quota attainment, product performance, and channel breakdown across **2023–2024**.

---

## 📸 Dashboard Preview

### Page 1 — Executive Overview
![Dashboard Page 1](screenshots/report1.png)

### Page 2 — Product & Regional Deep Dive
![Dashboard Page 2](screenshots/report2.png)

---


---

## 📊 Dataset Overview

**File:** `data/sales_data.csv` · **2,000 rows** · Jan 2023 – Dec 2024

| Column | Type | Description |
|--------|------|-------------|
| Date | Date | Transaction date |
| Region | Text | North / South / East / West |
| Sales_Rep | Text | 12 sales representatives |
| Product | Text | ProSuite X1, DataKit Pro, CoreLink 200, Starter Bundle, Accessory Pack |
| Category | Text | Software / Hardware / Bundle / Accessories |
| Quantity | Integer | Units per order (1–20) |
| Unit_Price | Decimal | List price |
| Discount | Decimal | Discount applied (0–15%) |
| Revenue | Decimal | Net revenue after discount |
| Returned | Text | Yes / No |
| Channel | Text | Online / Retail / Direct |

---

## 📈 Key KPIs (FY 2024)

| Metric | Value | vs 2023 |
|--------|-------|---------|
| Total Revenue | $48,40,300 | ↑ 20.6% |
| Units Sold | 61,340 | ↑ 11.2% |
| Avg Order Value | $78.50 | 2024 full year |
| Return Rate | 3.1% | All years combined |

---

## 📋 Dashboard Pages

### Page 1 — Executive Overview
| Visual | Description |
|--------|-------------|
| **4 KPI Cards** | Total Revenue, Units Sold, Avg Order Value, Return Rate — each with YoY context |
| **Monthly Revenue Trend** | Line chart comparing 2024 vs 2023 month-by-month (Jan–Dec) |
| **Revenue by Region** | Donut chart — North leads, followed by West, South, East |
| **Revenue by Channel** | Column chart — Online ($1.6M+) > Retail > Direct |
| **Revenue by Category** | Pie chart — Software dominates, followed by Hardware, Bundle, Accessories |
| **Quarterly Performance** | Grouped bar chart comparing Q1–Q4 across 2023 and 2024 |

### Page 2 — Product & Regional Analysis
| Visual | Description |
|--------|-------------|
| **Revenue by Channel** | Bar chart breakdown across Online, Retail, Direct |
| **Revenue by Category** | Pie chart — Software, Hardware, Bundle, Accessories share |
| **Quarterly Performance** | 2023 vs 2024 grouped comparison across all four quarters |
| **Top Products by Revenue** | Table with Product, Category, Revenue, Units, YoY % badge (ProSuite X1 leads at $11,18,240, +22%) |
| **Regional Quota Attainment** | Table showing Revenue vs Quota with attainment % — North 109.4% ✅, South 111.4% ✅, West 93.0% ⚠️, East 82.1% ⚠️ |

---

## 🔧 How to Use

### 1. Load the Data in Power BI Desktop
- **Get Data → Text/CSV** → import `data/sales_data.csv`
- Optionally import the `agg_*.csv` files as helper tables

### 2. Apply the Theme
**View → Themes → Browse for themes** → select `sales_theme.json`

### 3. Add DAX Measures
Open `dax_measures.dax` and copy each measure into Power BI via **New Measure**.

Key measures included:
- `Total Revenue`, `Total Revenue 2024`, `Total Revenue 2023`
- `YoY Revenue Growth %`
- `Avg Order Value`, `Units Sold`, `Return Rate %`
- `Quota Attainment %`
- Time intelligence: `Revenue MTD`, `Revenue QTD`, `Revenue YTD`, `Revenue PY`

---

## 🛠️ Tools & Skills

| Tool | Role |
|------|------|
| **Power BI Desktop** | Dashboard design, DAX measures, interactive visuals |
| **DAX** | KPI calculations, YoY growth, quota attainment, time intelligence |
| **Excel** | Supporting analysis and data validation |
| **Python / Pandas** | Data generation, cleaning, aggregated CSV exports |

---

## 🧠 Skills Demonstrated

- Power BI dashboard design across multiple report pages
- DAX measures: YoY growth, MTD/QTD/YTD, conditional KPI formatting
- KPI card design with trend context
- Cross-page visual consistency and colour theming
- Regional quota attainment tracking with conditional formatting
- Product-level revenue ranking with YoY badges
- Channel and category mix analysis
