# Sales Dashboard

---

## 1. Project Overview
This project presents a Sales Performance Dashboard built in Power BI to analyze revenue, profit, margin, and YoY revenue change.

It provides a centralized view of sales performance across customer segments, regions, and products, helping stakeholders track KPIs and identify growth opportunities.

---

## 2. Key Business Questions
This dashboard answers:

- What is the overall revenue, profit, margin, and YoY growth?
- How do monthly revenues compare to the budget?
- Which segments and regions generate the highest revenue and profit?
- What are the top 5 revenue-driving products?
- Where are the opportunities to improve profitability?

---

## 3. Power BI Features

### a) Data Modeling
- Designed a star schema:
  - Fact table: Sales
  - Dimension tables: Product, Customer, Location, Date
- Optimized relationships for faster filtering and accurate aggregations.

### b) DAX Measures
```DAX
Total Revenue = SUM(Sales[Revenue])
Total Profit  = SUM(Sales[Profit])
Margin        = DIVIDE([Total Profit], [Total Revenue])
Last year Revenue = CALCULATE ([Total Revenue],SAMEPERIODLASTYEAR ( 'Date'[Date] ))
YoY Revenue   = DIVIDE([Total Revenue] - [Last Year Revenue], [Last Year Revenue])
```

### c) Visuals and Interactivity

* KPI cards for revenue, profit, margin, and YoY change with conditional formatting.
* Combined column and line charts for monthly revenue, budget, and margin.
* Charts showing revenue, profit, and margin by customer segment.
* Charts showing revenue, profit, and margin by region.
* Top N filtering to highlight the top 5 products by revenue.
* Matrix for detailed insights by category, sub-category, and product name.

---

## 4. Project Structure

| File / Folder             | Description                    |
| ------------------------- | ------------------------------ |
| **README.md**             | Main project documentation     |
| **Sales\Dashboard.pbix** | Power BI dashboard file        |
| **Sales\Dashboard.png**                | Dashboard screenshot|

---

## 5. How to Use

### Option 1: Download the PBIX

1. Click on Sales Dashboard.pbix in this repository.
2. Click **View Raw** → **Download**.
3. Open it in **Power BI Desktop**.

### Option 2: View Screenshot

For a quick preview, click on Sales Dashboard.png in this repository.

