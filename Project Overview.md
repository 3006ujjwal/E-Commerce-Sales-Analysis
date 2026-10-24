# Project Overview — E-Commerce Sales Analysis

## 1. Project Summary

This project uses Microsoft Power BI to analyze Adidas U.S. sales data from January 2020 through December 2021. The dataset contains 9,648 records and approximately $900M in sales. The report is organized into two pages—**Sales Analysis** and **Profitability Analysis**—to examine sales performance and operating profitability across products, retailers, geography, and time.

The purpose is to turn a tabular sales dataset into an interactive report that supports historical performance analysis and business exploration.

## 2. Business Problem

Sales revenue is only one part of business performance. A useful analysis should also show where sales occur, how products and retailers contribute, how performance changes over time, and how sales relate to operating profit and margin.

This project addresses the following questions:

- How are sales distributed across states and regions?
- How do sales contributions compare across products and retailers?
- How does sales change across the reporting period?
- How do operating profit and profit margin vary by product?
- How does operating profit compare across retailers?
- What does the year-over-year sales measure show for the periods compared?

## 3. Dataset

| Attribute | Details |
|---|---|
| Dataset | Adidas U.S. sales data |
| Source file | `E-Commerce Sales Data.xlsx` |
| Worksheet | `Data Sales Adidas` |
| Period covered | January 2020–December 2021 |
| Number of records | 9,648 |
| Approximate total sales | $900M |
| Approximate operating profit | $332M |

### Fields used

The source dataset includes the following fields:

- `Retailer`
- `Retailer ID`
- `Invoice Date`
- `Region`
- `State`
- `City`
- `Product`
- `Price per Unit`
- `Units Sold`
- `Total Sales`
- `Operating Profit`
- `Operating Margin`
- `Sales Method`

These fields support analysis of sales value, sales volume, geography, product and retailer performance, pricing, profitability, and time.

## 4. Tools and Technologies

- **Microsoft Power BI** — report development and interactive visual analysis
- **Power Query** — data preparation and transformation
- **DAX** — explicit KPI and analytical measures
- **Microsoft Excel** — source dataset
- **Git/GitHub** — version control and portfolio presentation

## 5. Data Preparation and Analysis Workflow

The project workflow is:

1. **Import:** Load the Excel source data into Power BI.
2. **Prepare:** Use Power Query for data cleaning and transformation required for reporting.
3. **Measure:** Create explicit DAX measures for key business metrics.
4. **Visualize:** Build visuals for sales, geography, products, retailers, time, and profitability.
5. **Organize:** Separate the report into Sales Analysis and Profitability Analysis pages.
6. **Explore:** Use report slicers, filters, and tooltips to investigate the data interactively.

Only transformations actually performed in Power Query should be described in more detail. This document does not assume that duplicates, missing values, or outliers were removed unless that work is confirmed in the query steps.

## 6. Dashboard Page 1 — Sales Analysis

### Purpose

Explore the distribution and movement of sales across geographical areas, products, retailers, and time.

### KPIs shown

- Total Sales
- Total Operating Profit
- Total Units Sold
- Average Price per Unit
- Average Operating Margin
- Sales YoY %

### Main analytical views

| View | Question addressed |
|---|---|
| Total Sales by State | How are sales distributed across states? |
| Sales by Region | How does sales performance differ by region? |
| Total Sales by Retailer | How does sales contribution compare across retailers? |
| Total Sales by Product | How does sales contribution compare across products? |
| Total Sales by Month | How does sales vary over time? |

Interactive filters allow users to focus on selected dates and regions. Tooltips provide additional context where configured.

## 7. Dashboard Page 2 — Profitability Analysis

### Purpose

Examine operating profitability and margin separately from sales volume and sales value.

### KPIs shown

- Total Operating Profit
- Profit Margin %
- Sales YoY %

### Main analytical views

| View | Question addressed |
|---|---|
| Profit Margin by Product | How does margin differ across products? |
| Operating Profit by Retailer | How does operating profit compare across retailers? |
| Operating Profit by Product | How does operating profit differ across products? |

This page supports comparison of absolute operating profit and margin. These metrics answer different questions: a product can contribute substantial sales or profit without necessarily having the highest margin.

## 8. DAX Measures and KPIs

The report uses explicit measures for the following metrics:

| Measure | Analytical purpose |
|---|---|
| Total Sales | Summarizes sales value |
| Total Operating Profit | Summarizes operating profit |
| Total Units Sold | Measures unit volume |
| Average Price per Unit | Supports pricing analysis |
| Average Operating Margin | Summarizes the operating margin measure |
| Profit Margin % | Supports profitability comparison |
| Sales YoY % | Compares sales across year-over-year periods |

The precise DAX definitions should be copied from the Power BI model if this document is expanded with formulas. In particular, the definition of `Profit Margin %` and the time logic used by `Sales YoY %` should be documented exactly as implemented rather than inferred from the measure names.

## 9. Headline Results

The report's headline values include:

- **Total Sales:** approximately $900M
- **Total Operating Profit:** approximately $332M
- **Operating Margin:** approximately 36.9%
- **Sales YoY for 2021:** 294.2%

These values are rounded and can change when report filters are applied. The year-over-year result should be interpreted according to the exact DAX definition and the two-year period covered by the dataset. It describes the comparison calculated by the report; it should not be treated as a forecast.

## 10. Business Use

The report can help a user:

- Compare product and retailer sales contributions.
- Explore geographical differences in sales.
- Review operating profit and margin across products and retailers.
- Investigate sales trends over time.
- Identify areas for further analysis or business investigation.

The dashboard is a descriptive decision-support tool. It identifies patterns in the historical data but does not establish why those patterns occurred or predict future outcomes.

## 11. Limitations

- The analysis is limited to the fields and period available in the source dataset.
- Results depend on source-data quality and the definitions used in the Power BI measures.
- Year-over-year growth can be sensitive to the periods being compared and should be interpreted in context.
- The report does not perform predictive modeling or causal analysis.

## 12. Files

- `E-Commerce Sales Analysis.pbix` — Power BI report
- `E-Commerce Sales Data.xlsx` — source dataset
- `README.md` — short project summary and navigation
- `Screenshots/` — exported images of the report pages

## 13. How to Open the Project

1. Open `E-Commerce Sales Analysis.pbix` in Microsoft Power BI Desktop.
2. Navigate to **Sales Analysis** to explore sales performance.
3. Navigate to **Profitability Analysis** to explore operating profit and margins.
4. Use the available filters and slicers to investigate the data.
5. Consult the Excel source file for the underlying data.

## 14. Summary

This project demonstrates an end-to-end Power BI reporting workflow: preparing sales data, defining explicit DAX measures, and building an interactive report around sales and profitability questions. Its central strength is the separation of sales performance from profitability analysis, enabling a more rounded exploration of historical business performance.
