# E-Commerce Sales Analysis | Power BI

An interactive Power BI business intelligence project exploring **$900M in Adidas U.S. sales** across products, retailers, states, regions, and time. The report combines sales KPIs, profitability analysis, and year-over-year growth to make historical performance easier to explore.

## Business Problem

Sales totals alone do not explain how a business is performing. This project examines sales distribution alongside operating profit and margin to help answer:

- How does sales performance vary by state and region?
- Which products and retailers contribute to sales?
- How does sales change over time?
- How do operating profit and profit margin vary across products and retailers?
- What does year-over-year sales growth indicate about the periods being compared?

## Dashboard

The report contains two pages:

### 1. Sales Analysis

Explores sales performance across geography, products, retailers, and time.

**KPIs:** Total Sales, Total Operating Profit, Total Units Sold, Average Price per Unit, Average Operating Margin, and Sales YoY %.

**Views:** Sales by state, region, retailer, product, and month, with interactive filters and visual tooltips.

![Sales Analysis Dashboard](Screenshots/01%20-%20Sales%20Analysis.png)

### 2. Profitability Analysis

Focuses on operating profit and margin rather than sales value alone.

**KPIs:** Total Operating Profit, Profit Margin %, and Sales YoY %.

**Views:** Profit Margin by Product, Operating Profit by Retailer, and Operating Profit by Product.

![Profitability Analysis Dashboard](Screenshots/02%20-%20Profitability%20Analysis.png)


## Dataset

- **Source format:** Excel
- **Worksheet:** `Adidas Sales`
- **Coverage:** January 2020–December 2021
- **Records:** 9,648
- **Reported sales scale:** approximately $900M

The dataset includes retailer, retailer ID, invoice date, region, state, city, product, price per unit, units sold, total sales, operating profit, operating margin, and sales method.

## Tools & Techniques

- **Power BI:** interactive report and KPI presentation
- **Power Query:** data preparation and transformation
- **DAX:** explicit measures for sales, operating profit, units sold, pricing, margin, and year-over-year growth
- **Excel:** source dataset
- **GitHub:** version control and project documentation

## Headline Results

The report's overall headline values include approximately **$900M in sales**, **$332M in operating profit**, and a **36.9% operating margin**. The report also displays **294.2% Sales YoY for 2021**.

These are dataset/report-level figures, rounded for readability. Values may change when report filters are applied. Year-over-year growth should be interpreted in the context of the dataset's time coverage and the measure's definition.

## Workflow

1. Imported the Excel sales dataset into Power BI.
2. Prepared and transformed the data using Power Query.
3. Created explicit DAX measures for key sales and profitability KPIs.
4. Built separate Sales Analysis and Profitability Analysis pages.
5. Added interactive slicers, comparisons, and tooltips to support exploration.

## Repository Contents

```text
E-Commerce-Sales-Analysis/
├── Documentation/
│   └── project-overview.md
├── Screenshots/
│   ├── Sales-Analysis.png
│   └── Profitability-Analysis.png
├── E-Commerce Sales Analysis.pbix
├── E-Commerce Sales Data.xlsx
└── README.md
```

## How to Explore

1. Download or clone this repository.
2. Open `E-Commerce Sales Analysis.pbix` in Microsoft Power BI Desktop.
3. Explore both report pages and interact with the available slicers and filters.
4. Refer to `E-Commerce Sales Data.xlsx` for the source data.

## Scope & Limitations

This is a historical, descriptive analytics project. It helps users explore performance patterns but does not establish causation or forecast future sales.

## Author

**Ujjwal Prasad**  
Business Intelligence · Data Analytics · Data Visualization
Power BI | DAX | Power Query | Excel
