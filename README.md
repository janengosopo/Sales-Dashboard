# Sales Performance Dashboard

## Project Overview
This dashboard supports sales managers and team leads in monthly performance reviews by identifying revenue gaps, margin risks, and highlighting areas to focus on for improving profitability.  

It is designed to answer three key business questions:

1. **How are we performing?**  
   - Revenue vs budget  
   - Margin trend  

2. **Where are the main drivers of performance?**  
   - Segment, region, and product breakdown  

3. **Where should we act next?**  
   - Identify underperforming areas impacting profitability  

![Dashboard Screenshot](Dashboard%20Screenshot.png)

---

## Key Insights (2024)

1. **Growth achieved, but profitability was weak**  
   - Revenue exceeded budget by 1.1%, but margin was 5.6%, below the acceptable threshold of 7%.  
   - **Recommendation:** Review pricing strategy and cost structure to improve margin without sacrificing revenue.

2. **Sales performance was driven by H2**  
   - Budget was missed in H1 (except January). Recovery started in August, and H2 sales helped achieve the budget target.  
   - **Hypothesis:** Seasonal demand, campaigns, or discounting strategies influenced H2 performance.  
   - **Recommendation:** Identify key drivers behind H2 performance and replicate them earlier in the year.

3. **Furniture is the primary driver of low margin**  
   - Furniture shows a critically low margin of 3.9% (<4%), it significantly impacts overall profitability.  
   - **Recommendation:** Review pricing, discounting practices, and costs for the Furniture segment.

4. **Margin is borderline across all regions**  
   - All regions have margins between 5.3%–6%, this indicates systemic profitability issues.  
   - West region had the highest revenue but lowest margin (5.3%).  
   - **Recommendation:** Investigate whether high revenue is driven primarily by discounting.

5. **High-revenue products are not driving profit**  
   - Among the top 5 products by revenue, only 2 had healthy margins; others were <3%.  
   - **Recommendation:** Review pricing or deprioritize low-margin products to reduce profitability leakage.

6. **Low-performing products should be reviewed**  
   - Bottom 5 products combine low revenue (<25K) with critically low margins (<1%).  
   - **Recommendation:** Consider discontinuation or replacement with higher-margin alternatives.

---

## Business Impact (Simulated)
If applied in a real business context, this dashboard supports:

- **Sales managers:** Identifying underperforming segments and regions  
- **Product teams:** Reviewing low-margin and low-performing products  
- **Finance teams:** Monitoring budget performance and profitability risks  

---

## Technical Approach

- **Data preparation:** Cleaned and standardized source data to ensure quality  
- **Data modeling:** Designed a star schema for scalable analysis across segment, region, and product dimensions  
- **Analysis & metrics:** Developed DAX measures for margin calculations, YOY revenue, and performance tracking  
- **Visualization:** Built an interactive dashboard with consistent margin-based color coding for decision support  
- **Tools:** Power BI, Power Query, DAX  

---

## Caveats and Assumptions

- Budget allocation at sub-category level is estimated from historical revenue share, not actual targets  
- Margin thresholds (4%, 7%, 10%) are illustrative; it should be aligned with finance-defined targets for operational use  
- No pipeline or forecast data included; analysis is based on historical performance only  
- Dataset is based on the Superstore sample and used for demonstration purposes  

---

## Project Structure

| File / Folder            | Description                     |
|---------------------------|---------------------------------|
| README.md                 | Main project documentation      |
| Sales/Dashboard.pbix      | Power BI dashboard file         |
| Dashboard/Screenshot.png  | Dashboard screenshot            |

---

## How to Use

1. Download the PBIX file from this repository: `Sales/Dashboard.pbix`  
2. Click **View Raw → Download**  
3. Open the file in **Power BI Desktop**  
