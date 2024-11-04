# Sales Management Dashboard Project 

## Table of Contents

- [Business Request](#business-request)
- [Overview](#overview)
- [User Stories](#user-stories)
- [Data Cleansing & Transformation](#data-cleansing--transformation)
  - [SQL Scripts](#sql-scripts)
  - [Data Cleansing Steps](#data-cleansing-steps)
  - [Finalized Tables](#finalized-tables)
- [Data Model in Power BI](#data-model-in-power-bi)
- [Sales Management Dashboard](#sales-management-dashboard)
- [Appendix](#appendix)

---

## Business Request

**Request from:** Steven, Sales Manager  
**Objective:** Move from static sales reports to an interactive dashboard to better visualize internet sales performance, customer engagement, and product metrics over time.  
**Requirements:** Create a Power BI dashboard using historical sales data (two years back) and compare performance against a provided 2021 budget.

---

## Overview

**Primary Systems Involved:** Power BI, CRM System  
**Data Source:** Sales budgets delivered in Excel for 2021, other sales data sourced from CRM system.

---

## User Stories

| No | Role                | Requirement                            | Value                                         | Acceptance Criteria |
|----|----------------------|----------------------------------------|-----------------------------------------------|---------------------|
| 1  | Sales Manager       | Overview of internet sales             | Track top customers and products              | Power BI dashboard with daily updates         |
| 2  | Sales Representative | Detailed customer sales view          | Monitor high-value customers for follow-up    | Filterable Power BI dashboard by customer     |
| 3  | Sales Representative | Detailed product sales view           | Focus on top-selling products                 | Filterable Power BI dashboard by product      |
| 4  | Sales Manager       | Sales vs. budget over time            | Analyze performance against budget            | Graphs and KPIs in Power BI showing budget comparisons |

---

## Data Cleansing & Transformation

To prepare data for the analysis, the following tables were created and cleansed using SQL.

### SQL Scripts

#### `DIM_Calendar`
A clean calendar dimension used to enable date-based analysis.

![DIM_Calendar SQL](link-to-dim_calendar-image)

#### `DIM_Customers`

![DIM_Customers SQL](link-to-dim_customers-image)

#### `DIM_Products`

![DIM_Products SQL](link-to-dim_products-image)

#### `FACT_InternetSales`

![FACT_InternetSales SQL](link-to-fact_internetsales-image)

*SQL scripts are also available as images if needed.*

---

## Data Model in Power BI

The data model created in Power BI incorporates `FACT_InternetSales`, `DIM_Customers`, `DIM_Products`, and `DIM_Calendar`, along with the sales budget data imported from CSV files. This setup allows for robust cross-table analysis and visualizations.

**Data Model Diagram:**  
_Screenshot of Power BI data model goes here._

---

## Sales Management Dashboard

The dashboard consists of:

- **Overview Page:** High-level metrics, trends, and KPIs on internet sales.
- **Customer Insights:** Detailed customer sales performance, with filtering options.
- **Product Insights:** Focused view on product sales, with filtering by product category.

Each page allows drill-down capabilities for specific time frames, customers, or products as needed by user roles.

---

### Recommendations

- Implement periodic reviews to align dashboard metrics with sales goals.
- Use insights from the dashboard to adjust sales strategies based on customer/product performance.

--- 

Let me know if this layout helps or if you need any additional refinements!
