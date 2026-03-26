End-to-End Sales Performance Analytics
SQL → Excel → Power BI
Domain: Pet Supplement Distribution (Herbsmith-style)
Tools: SQLiteOnline · Microsoft Excel Online · Power BI (coming soon)
Author: Sharon Paulraj — ERP Operations Analyst → Business Systems Analyst
Portfolio: github.com/sharonpaul604-wq

Project Overview
This project simulates a real business analytics scenario for a pet supplement distribution company. Starting from a custom-built sales database, I built a complete three-phase analytics pipeline — from SQL querying through Excel analysis to an interactive Power BI dashboard — mirroring the kind of work a Business Systems Analyst performs in a distribution or ERP environment.

📁 Repository Contents
FileDescriptionherbsmith_queries.sqlFive business SQL queries with full schemaherbsmith_sales_analytics.xlsxExcel workbook — 6 tabs of analysis and chartsREADME.mdThis file

🗂️ Phase 1 — SQL Analytics ✅
Tool: SQLiteOnline
Goal: Query a relational sales database to answer five business questions using SQL joins, aggregations, window functions, and conditional logic.
Database Schema
TableColumnsproductsproduct_id, product_name, brand, category, unit_pricecustomerscustomer_id, customer_name, region, channelordersorder_id, customer_id, product_id, order_date, quantity, total_amount

Query 1 — Revenue Ranking by Product
Problem: The business needed to identify which products were driving the most revenue to prioritize inventory and marketing spend.
Finding: The top 3 products accounted for over 60% of total revenue, revealing strong concentration in a few SKUs.
Recommendation: Protect and invest in high-ranking SKUs while monitoring mid-tier products for growth potential.

Query 2 — Brand Market Share
Problem: Leadership wanted to understand each brand's contribution to total sales to evaluate portfolio balance.
Finding: One brand held over 40% market share, indicating potential over-reliance on a single product line.
Recommendation: Evaluate supply chain risk and consider diversification strategies to reduce dependency on the top brand.

Query 3 — Regional Sales Analysis
Problem: The operations team needed to understand which regions were generating the highest revenue and order volume.
Finding: The West region led in order count, but the Northeast had the highest average order value.
Recommendation: Target Northeast customers with upsell and cross-sell campaigns to maximize revenue per transaction.

Query 4 — Channel Comparison (WooCommerce vs. Wholesale)
Problem: The business wanted to compare WooCommerce and wholesale channel performance to guide sales strategy.
Finding: Wholesale had fewer orders but significantly higher average order value than WooCommerce.
Recommendation: Invest in wholesale relationship management for higher ROI per transaction while growing WooCommerce volume.

Query 5 — Customer Segmentation (CASE WHEN)
Problem: The business lacked a clear view of which customers were high-value versus low-value for targeted engagement.
Finding: High-value customers (top 20%) drove approximately 70% of total revenue — a classic Pareto distribution.
Recommendation: Build a loyalty or early-access program targeting the High Value segment to improve retention and lifetime value.

SQL Skills Demonstrated

SQL joins — INNER JOIN across 3 tables
Aggregate functions — SUM, COUNT, AVG, ROUND
Window functions — RANK OVER
Conditional logic — CASE WHEN segmentation
Business insight communication — Problem → Finding → Recommendation


📊 Phase 2 — Excel Analytics ✅
Tool: Microsoft Excel Online
Goal: Transform raw sales order data into structured business insights using Excel formulas and charts across five analysis tabs.
Dataset Overview

15 sales orders across 4 regions, 2 channels, 3 brands, and 6 customers
10 columns: Order_ID, Customer_Name, Region, Channel, Brand, Product_Name, Category, Quantity, Unit_Price, Total_Amount
Total Revenue: $18,470


Tab 1 — Raw Data
Source data table with 15 rows and 10 columns, formatted as a structured Excel table and used as the reference range for all SUMIF and COUNTIF formulas across analysis tabs.

Tab 2 — Product Revenue
Business Question: Which products generate the most revenue?
Formula Used: SUMIF for revenue aggregation per product
Visual: Bar chart — "Product Revenue Performance"
BSA Insight: Hip & Joint Chews is the top-performing product, reflecting strong market demand for joint support supplements — a key category for Herbsmith's wholesale and online customers.

Tab 3 — Brand Share
Business Question: How is revenue distributed across brands?
Formula Used: SUMIF for revenue aggregation per brand
Visual: Pie chart with percentage labels — "Brand Revenue Percentage"
BSA Insight: Herbsmith-branded products lead in revenue share, confirming brand loyalty among buyers. Supporting brands represent an opportunity for co-marketing or bundle strategies.

Tab 4 — Regional Analysis
Business Question: Which regions drive the most revenue and order value?
Formulas Used: SUMIF, COUNTIF, and AOV division formula
Visual: Bar chart — "Regional Revenue Performance"
RegionTotal RevenueTotal OrdersAvg Order ValueWest$7,1945$1,438.80Northeast$6,3604$1,590.00South$2,5763$858.67Midwest$2,3403$780.00
BSA Insight: The West leads in total revenue, but the Northeast delivers the highest average order value at $1,590 — indicating premium purchasing behavior. The South and Midwest represent growth opportunities through targeted promotions or bundle pricing.

Tab 5 — Channel Comparison
Business Question: Which sales channel performs better — Wholesale or WooCommerce?
Formulas Used: SUMIF, COUNTIF, and AOV division formula
Visual: Bar chart — "Channel Revenue Comparison"
ChannelTotal RevenueTotal OrdersAvg Order ValueWholesale$11,2768$1,409.50WooCommerce$7,1947$1,027.71
BSA Insight: Wholesale is the dominant channel generating 61% of total revenue with a higher average order value. A dual-channel growth strategy — strengthening wholesale while scaling WooCommerce — would maximize overall revenue.

Tab 6 — Customer Segments
Business Question: Which customers are most valuable to the business?
Formulas Used: SUMIF, COUNTIF, and AOV division formula
Visual: Bar chart — "Customer Revenue Comparison"
CustomerTotal RevenueTotal OrdersAvg Order ValuePet Palace$4,6503$1,550.00FurEver Care$4,3163$1,438.67Healthy Paws$3,3603$1,120.00Tail Waggers$2,3942$1,197.00Green Pet Co$2,3102$1,155.00Paws & Play$1,4402$720.00
BSA Insight: Pet Palace and FurEver Care are the highest-value customers, both wholesale buyers placing consistent large orders. Paws & Play represents an account development opportunity. Green Pet Co and Tail Waggers show strong AOV relative to order count — making them strong candidates for upsell initiatives.

Excel Skills Demonstrated

SUMIF — conditional revenue aggregation
COUNTIF — conditional order counting
Calculated columns — Average Order Value (AOV)
Currency formatting with 2 decimal places
Bar charts and pie charts with professional formatting
BSA-style business insight writing per analysis tab

📊 Phase 3 — Power BI Dashboard
Herbsmith Sales Performance Dashboard
Tool: Power BI Desktop
Domain: Pet Supplement Distribution (Herbsmith-style)
Author: Sharon Paulraj — ERP Operations Analyst → Business Systems Analyst
Portfolio: github.com/sharonpaul604-wq

This is Phase 3 of the End-to-End Sales Performance Analytics capstone project.
Phase 1 (SQL) and Phase 2 (Excel) are documented in the main project README.


📌 Dashboard Overview
This Power BI report brings together all five business analysis areas — revenue performance, brand share, regional analysis, channel comparison, and customer segmentation — into a single 3-page interactive executive dashboard.
The report is designed to allow a Sales Manager or Operations Director to explore performance data through interactive slicers, without needing to run a separate report for each business question.

📁 Files
FileDescriptionherbsmith_sales_dashboard.pbixPower BI Desktop report — 3-page interactive dashboarddashboard_preview.pngScreenshot preview of the dashboard

🗂️ Report Structure — 3 Pages

Page 1 — Executive Summary
Purpose: High-level snapshot of overall business performance — the first page a leadership team would see.
KPI Cards (3 headline metrics):
CardMeasureTotal RevenueSum of all sales order amountsTotal OrdersCount of all orders placedAverage Order Value (AOV)Total Revenue ÷ Total Orders
Interactive Slicers (3 cross-page filters):
SlicerFieldWhat it doesRegionSales[Region]Filters all visuals by geographic regionChannelSales[Channel]Filters by Wholesale or WooCommerceBrandSales[Brand]Filters by product brand
Business Purpose: Selecting any slicer instantly updates all KPI cards so leadership can answer questions like "What is our total revenue from wholesale orders in the West?" in one click — no spreadsheet required.

Page 2 — Sales Breakdown
Purpose: A deeper view of revenue split across regions, brands, and channels.
📊 Bar Chart — Revenue by Region

X-axis: Total Revenue
Y-axis: Region (West, Northeast, South, Midwest)
Business Question: Which regions are driving the most revenue?
BSA Insight: Quickly reveals if one region is significantly outperforming others — useful for allocating sales rep coverage or planning regional promotions.

🥧 Pie Chart — Revenue Share by Brand

Legend: Brand
Values: Brand Revenue Share (%)
Business Question: How is revenue distributed across our product brands?
BSA Insight: A dominant slice signals over-reliance on a single brand — an important risk flag for supply chain and marketing strategy.

📊 Clustered Bar Chart — Channel Comparison

Axis: Channel (Wholesale / WooCommerce)
Values: Total Revenue + Total Orders (side by side)
Business Question: Which channel generates more revenue and more orders?
BSA Insight: Comparing revenue and order count together reveals whether one channel wins on volume but loses on order value — key for channel investment decisions.


Page 3 — Customer Insights
Purpose: Customer-level analysis to identify high-value accounts and support targeted engagement.
📊 Column Chart — Revenue by Customer

X-axis: Customer Name
Y-axis: Total Revenue
Business Question: Which customers contribute the most to overall revenue?
BSA Insight: Visually identifies the Pareto effect — where a small number of customers account for the majority of revenue. Supports prioritization for account management and retention efforts.

📋 Table Visual — Customer Detail View
A full customer breakdown table showing:
ColumnDescriptionCustomer NameAccount nameTotal RevenueSum of all orders for that customerTotal OrdersNumber of orders placedAverage Order Value (AOV)Revenue per order for that customer
BSA Insight: The table lets the sales team sort and compare accounts side by side — identifying which customers place fewer but higher-value orders versus those with high frequency but lower spend.

🧮 DAX Measures Used
All KPI cards and chart values are powered by the following DAX measures:
daxTotal Revenue = SUM(Sales[Total_Amount])

Total Orders = COUNTROWS(Sales)

Average Order Value (AOV) = DIVIDE([Total Revenue], [Total Orders], 0)

Brand Revenue Share =
    DIVIDE(
        [Total Revenue],
        CALCULATE([Total Revenue], ALL(Sales[Brand]))
    )

🔗 Data Model
The dashboard is built on a single flat table named Sales, containing all order, customer, product, and channel data in one structured source — consistent with how ERP export data is typically structured in a distribution environment.
FieldDescriptionCustomer_NameAccount nameRegionGeographic sales regionChannelWholesale or WooCommerceBrandProduct brandProduct_NameProduct SKU nameCategoryProduct categoryQuantityUnits orderedUnit_PricePrice per unitTotal_AmountLine total (Quantity × Unit_Price)

💼 Power BI Skills Demonstrated

DAX measures — Total Revenue, Total Orders, AOV, and Brand Revenue Share
KPI cards — Headline metrics for executive-level reporting
Interactive slicers — Region, Channel, and Brand cross-filtering all pages
Bar chart — Revenue by Region with ranked axis
Pie chart — Brand revenue share with percentage labels
Clustered bar chart — Side-by-side channel comparison (Revenue + Orders)
Column chart — Customer revenue ranking
Table visual — Multi-column customer detail breakdown
Multi-page report design — Clear narrative flow from summary to breakdown to customer detail


🚀 How to Open This Report

Download and install Power BI Desktop (free)
Clone or download this repository
Open herbsmith_sales_dashboard.pbix in Power BI Desktop
Use the slicers on Page 1 to filter the report by Region, Channel, or Brand
Navigate between pages using the page tabs at the bottom


📈 Full Capstone Project Roadmap
PhaseToolStatusPhase 1 — SQL AnalyticsSQLiteOnline✅ CompletePhase 2 — Excel AnalyticsExcel Online✅ CompletePhase 3 — Power BI DashboardPower BI Desktop✅ Complete

👩‍💻 About the Author
Sharon Paulraj
ERP Operations Analyst | Aspiring Business Data Analyst
Milwaukee, Wisconsin

💼 Background in ERP systems (Sage 100), WooCommerce operations, and business process analysis
📊 Building expertise in SQL, Power BI, and Excel for business analytics
🎯 Transitioning into Business Systems Analyst and Business Data Analyst roles

🔗 GitHub Portfolio
