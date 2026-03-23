# End-to-End Sales Performance Analytics — SQL
**Domain:** Pet Supplement Distribution (Herbsmith-style)  
**Tool:** SQLiteOnline  
**Part of:** End-to-End Sales Performance Analytics (SQL → Excel → Power BI)

---

## Project Overview
This project simulates a real business analytics scenario for a pet supplement distribution company.
Using a custom-built SQLite database with orders, products, and customer tables, I wrote five 
business-focused SQL queries covering the full sales analysis pipeline — from product revenue 
ranking to customer segmentation.

---

## Database Schema
- **products** — product_id, product_name, brand, category, unit_price  
- **customers** — customer_id, customer_name, region, channel (WooCommerce / Wholesale)  
- **orders** — order_id, customer_id, product_id, order_date, quantity, total_amount

---

## Business Queries & Insights

### Query 1 — Revenue Ranking by Product
**Problem:** The business needed to identify which products were driving the most revenue to prioritize inventory and marketing spend.  
**Finding:** The top 3 products accounted for over 60% of total revenue, revealing strong concentration in a few SKUs.  
**Recommendation:** Protect and invest in high-ranking SKUs while monitoring mid-tier products for growth potential.

### Query 2 — Brand Market Share
**Problem:** Leadership wanted to understand each brand's contribution to total sales to evaluate portfolio balance.  
**Finding:** One brand held over 40% market share, indicating potential over-reliance on a single product line.  
**Recommendation:** Evaluate supply chain risk and consider diversification strategies to reduce dependency on the top brand.

### Query 3 — Regional Sales Analysis
**Problem:** The operations team needed to understand which regions were generating the highest revenue and order volume.  
**Finding:** The West region led in order count, but the Northeast had the highest average order value.  
**Recommendation:** Target Northeast customers with upsell and cross-sell campaigns to maximize revenue per transaction.

### Query 4 — Channel Comparison (WooCommerce vs. Wholesale)
**Problem:** The business wanted to compare WooCommerce and wholesale channel performance to guide sales strategy.  
**Finding:** Wholesale had fewer orders but significantly higher average order value than WooCommerce.  
**Recommendation:** Invest in wholesale relationship management for higher ROI per transaction while growing WooCommerce volume.

### Query 5 — Customer Segmentation (CASE WHEN)
**Problem:** The business lacked a clear view of which customers were high-value versus low-value for targeted engagement.  
**Finding:** High-value customers (top 20%) drove approximately 70% of total revenue — a classic Pareto distribution.  
**Recommendation:** Build a loyalty or early-access program targeting the High Value segment to improve retention and lifetime value.

---

## Skills Demonstrated
- SQL joins (INNER JOIN across 3 tables)
- Aggregate functions (SUM, COUNT, AVG, ROUND)
- Window functions (RANK OVER)
- Conditional logic (CASE WHEN segmentation)
- Business insight communication (Problem → Finding → Recommendation)

---

## Next Phase
➡️ **Phase 2 — Excel:** Data cleaning, SUMIF summaries, pivot tables, and trend analysis  
➡️ **Phase 3 — Power BI:** 3-page interactive executive dashboard with KPIs and DAX measures
