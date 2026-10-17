# UK Retail Sales Analysis

Excel and Power BI analysis of 600 retail transactions across 5 UK regions, January to June 2025.

## Business question

Which regions and product categories drive the most revenue, and how does average order value differ by region? The aim was to show where the business is over- or under-performing so staffing, stock and marketing could be prioritised.

## Dashboard

![Overview](dashboard-overview.png)

Filtering to Electronics reorders the regions completely:

![Electronics filter](dashboard-electronics.png)

## Data cleaning

The raw file (605 rows) had three problems, all fixed before analysis:

- **Inconsistent region casing** ("LONDON" vs "London"): fixed with a case-sensitive Find & Replace
- **5 duplicate rows**: removed across the full row
- **Blank salesperson names**: labelled "Unknown" so they stayed in the totals

Result: 600 clean rows, £373,909 total revenue.

## Key findings

- **Bristol** led on revenue (£82,969), but Birmingham was within 2%. **London** was about 28% behind Bristol.
- **Birmingham** had the highest average order value (£637.67), so its revenue comes from fewer, bigger sales.
- **London** was weakest on every metric measured.
- Category strength differs by region: Bristol and Birmingham lead in Grocery, Manchester in Electronics and Home.
- Filtering to Electronics (£83.38K) moves Manchester to first and Bristol to fourth.

## Recommendations

- Test whether Bristol and Birmingham's Grocery approach works in Leeds and London.
- Investigate London's volume and order value problem.
- Grow Birmingham through transaction volume, not pricing.
- Use Manchester as the Electronics benchmark.

## Tools

Excel (pivot tables, SUMIFS, COUNTIFS, XLOOKUP, conditional formatting, Remove Duplicates, Find & Replace), Power BI Desktop (bar and stacked column charts, card, slicer, cross-filtering).

## Files

- `retail_sales_practice.csv`: raw data
- `retail_sales_cleaned.csv`: cleaned data
- `retail_sales_dashboard.pbix`: Power BI dashboard
- `UK-Retail-Sales-Analysis-Portfolio.docx`: full write-up

*Note: this uses a synthetic practice dataset built to mirror realistic retail sales data, created for portfolio development.*
