# Sales Dashboard

---

## 1. Project Overview

- Goal: To provide a centralized view of sales performance across customer segments, regions, and products, helping stakeholders track KPIs and identify growth opportunities.
- Tool: Power BI
- Project Type: Data cleaning, Data analysis, Data visualization
- Process: gathered data from Kaggle, cleaned, analysed, and visualised data in Power BI


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

### a. Data Modeling
- Designed a star schema:
  - Fact table: Sales
  - Dimension tables: Product, Customer, Location, Date
- Optimized relationships for faster filtering and accurate aggregations.

### b. DAX Measures
```DAX
Total Revenue = SUM(Sales[Revenue])
Total Profit  = SUM(Sales[Profit])
Margin        = DIVIDE([Total Profit], [Total Revenue])
Last year Revenue = CALCULATE ([Total Revenue],SAMEPERIODLASTYEAR ( 'Date'[Date] ))
YoY Revenue   = DIVIDE([Total Revenue] - [Last Year Revenue], [Last Year Revenue])
```

### c. Visuals and Interactivity

* KPI cards for revenue, profit, margin, and YoY change with conditional formatting.
* Combined column and line charts for monthly revenue, budget, and margin.
* Charts showing revenue, profit, and margin by customer segment.
* Charts showing revenue, profit, and margin by region.
* Top N filtering to highlight the top 5 products by revenue.
* Matrix for detailed insights by category, sub-category, and product name.

---

## 4. Insights of 2024 Performance

### a. Strong YoY Growth
- Revenue was up **17.8%** to **3.59M**, with profit at **0.20M**.  
- Growth was high, but margin was thin at **5.6%**.  

### b. Consumer Segment as Revenue Driver
- Consumer segment had the **highest revenue (1.63M)** and **profit (0.09M)**.  
- However, **margins were slightly lower** compared to other segments.  

### c. Regional Performance is Uneven
- **West region** achieved the **highest revenue (1.23M)** and **profit (0.06M)**.  
- **South region** had the **lowest revenue (0.57M)** and **profit (0.03M)**, significantly lower than the West region.* 

---

## 5. Project Structure

| File / Folder             | Description                    |
| ------------------------- | ------------------------------ |
| **README.md**             | Main project documentation     |
| **Sales\Dashboard.pbix** | Power BI dashboard file        |
| **Sales\Dashboard.png**                | Dashboard screenshot|

---

## 6. How to Use

### Option 1: Download the PBIX

1. Click on Sales Dashboard.pbix in this repository.
2. Click **View Raw** → **Download**.
3. Open it in **Power BI Desktop**.

### Option 2: View Screenshot

For a quick preview, click on Sales Dashboard.png in this repository.

