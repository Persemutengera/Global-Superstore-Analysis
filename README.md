# Global Superstore Sales & Profitability Analysis

## Project Overview

This Excel portfolio project analyzes Global Superstore transaction data to understand sales performance, profitability, customer segments, product categories, markets, and monthly trends. The workbook uses cleaned transaction data, calculated fields, PivotTables, and a dashboard-oriented structure to turn raw sales records into business insights.

## Dataset

- **Rows analyzed:** 51,290 transaction lines
- **Order-date coverage:** 1 January 2011–31 December 2014
- **Fields:** order and shipping dates, order/customer/product IDs, segment, country, market, region, category, sub-category, sales, quantity, discount, profit, shipping cost, and calculated time/profit fields.
- **Data note:** 41,296 records have a blank Postal Code. This appears consistent with a global dataset in which postal codes are not available for many non-US records; it should not automatically be treated as an error.

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Sales | 12,642,501.91 |
| Total Profit | 1,467,457.29 |
| Overall Profit Margin | 11.61% |
| Total Quantity Sold | 178,312 |
| Distinct Orders | 25,035 |
| Average Order Value | 504.99 |
| Distinct Customers | 1,590 |
| Distinct Products | 10,292 |


## Main Findings

1. **Sales grew every year.** Annual sales rose from 2.26 million in 2011 to 4.30 million in 2014. Year-over-year sales growth was approximately 18.5% in 2012, 27.2% in 2013, and 26.3% in 2014.
2. **Technology led category sales and profit.** Technology generated 4.74 million in sales and 663,778.73 in profit, with an approximately 14.0% margin.
3. **Furniture needs a profitability review.** Furniture generated 4.11 million in sales but only 285,204.72 in profit, an approximately 6.9% margin. The Tables sub-category recorded a loss of 64,083.39 on 757,041.92 in sales (approximately -8.5% margin).
4. **Discounts warrant attention.** In this dataset, rows with discounts above 20% collectively generated negative profit in the 20–30%, 30–50%, and 50–100% discount bands. This is an association in the observed data, not proof that discounts alone caused the losses; category and product mix should also be checked.
5. **Consumers contributed the largest share of sales.** The Consumer segment generated 6.51 million, about 51.5% of all sales.
6. **APAC was the largest market by sales and profit.** APAC recorded 3.59 million in sales and 436,000.05 in profit. EMEA generated 806,161.31 in sales but a lower 5.45% margin, suggesting a need to investigate costs, discounts, and product mix.
7. **Sales were strongest toward year-end.** November and December were the highest-sales months in the four-year aggregate, at approximately 1.55 million and 1.58 million respectively. August and September were also strong.
8. **The highest-sales product is not automatically the most profitable.** Apple Smart Phone, Full Size led product sales at 86,935.78, while Canon imageCLASS 2200 Advanced Copier generated 25,199.93 in profit. Product decisions should consider both sales and profit.

## Recommendations

- Investigate the Tables sub-category and loss-making products; review pricing, procurement costs, shipping costs, and discount policies before making assortment decisions.
- Set discount guardrails and monitor profit margin by discount band, product, category, and market.
- Continue to study Technology and other high-profit product lines while checking that growth is profitable rather than sales-only.
- Investigate EMEA and Southeast Asia margins relative to sales; identify whether the gap is associated with discounting, product mix, shipping costs, or other factors.
- Prepare inventory and campaign plans ahead of the November–December sales peak.
- Keep monthly trend analysis sorted by a true date field or `Year_Month` so that months from different years are not incorrectly combined when a year-by-year trend is required.

## Workbook Structure

- `01_Raw_Data` — source transaction records
- `02_Clean_Data` — cleaned data and helper fields
- `03_Calculations` — KPI calculations
- `04_PivotTables` — summary tables supporting analysis
- `05_Dashboard` — dashboard worksheet
- `06_Insights` — written interpretation and recommendations

## Tools and Techniques

- Microsoft Excel
- Data cleaning and validation
- Excel Tables and calculated columns
- PivotTables and distinct counts
- KPI calculations
- Sales, profit, margin, product, customer-segment, market, and time-trend analysis
- Dashboard design and business recommendations

## How to Use

1. Open `Global_Superstore_Data_Analysis.xlsx` in Microsoft Excel.
2. Review `02_Clean_Data` and confirm that the calculated columns are populated.
3. Refresh PivotTables after changing or replacing source data.
4. Use the dashboard filters/slicers, if available in your Excel version, to explore specific years, regions, markets, categories, and segments.
5. Read the `06_Insights` worksheet alongside this README. The separate `Global_Superstore_Insights_Report.md` contains the evidence-based findings in a report format.

## Limitations

- The dataset is observational; the analysis describes patterns and associations rather than proving causation.
- Blank postal codes are common in the global data and should be assessed by country/market before deciding whether to impute or exclude them.

## Portfolio Skills Demonstrated

Excel data preparation, formula-based calculations, PivotTables, distinct-count KPIs, descriptive analysis, profitability analysis, time-series analysis, dashboard planning, and translating results into actionable recommendations.
