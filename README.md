# Retail Sales Performance Dashboard

## Business Problem Summary

Retail leadership requires a centralized executive dashboard to monitor overall business performance and identify opportunities for growth and operational improvement. The objective of this project is to transform transactional retail data into an interactive Tableau dashboard that enables decision-makers to monitor sales, profitability, customer behavior, regional performance, shipping efficiency, discount impact, and return trends.

The dashboard is designed to answer key business questions, support strategic decision-making, and provide actionable insights through visual analytics.

---

# Dataset Description

The project uses a retail sales dataset containing order-level transactional information.

The dataset includes:

* Order Date
* Ship Date
* Order ID
* Customer Segment
* Region
* Category
* Sub-Category
* Sales
* Profit
* Discount
* Ship Mode
* Returned Orders

The data was cleaned and prepared in Tableau to ensure accurate analysis and visualization.

---

# Tableau Workbook Description

The Tableau workbook contains an executive dashboard consisting of multiple worksheets and KPI cards.

The workbook includes:

* Sales Trend View
* Regional Performance View
* Category Profitability View
* Customer Segment View
* Discount vs Profit View
* Shipping Performance View
* Return Analysis View
* Executive KPI Cards

The dashboard is fully interactive and designed for leadership reporting.

---

# Calculated Fields Created

The following calculated fields were created during the analysis:

### Profit Margin

```tableau
SUM([Profit]) / SUM([Sales])
```

Displays overall business profitability as a percentage.

---

### Delivery Days

```tableau
DATEDIFF('day',[Order Date],[Ship Date])
```

Calculates the number of days between order placement and shipment.

---

### Average Delivery Days

Uses:

```tableau
AVG([Delivery Days])
```

to compare shipping performance across shipping modes.

---

### Return Rate

Calculated using returned orders divided by total orders.

Used for analyzing return patterns across customer segments.

---

# Dashboard Components

The executive dashboard contains:

### KPI Cards

* Total Sales
* Total Profit
* Total Orders
* Profit Margin

### Visualizations

* Sales Trend (Line Chart)
* Regional Performance (Horizontal Bar Chart)
* Category Profitability (Bar Chart)
* Customer Segment Performance (Bar Chart)
* Discount vs Profit (Scatter Plot with Trend Line)
* Shipping Performance (Horizontal Bar Chart)
* Return Analysis (Bar Chart)

---

# Filters and Interactions Used

The dashboard includes interactive filters for:

* Order Date
* Region
* Customer Segment
* Sub-Category

Dashboard actions were implemented so that selecting values in one visualization filters related charts across the dashboard, enabling interactive business exploration.

---

# Key Business Insights

Major insights obtained from the dashboard include:

* Sales remain relatively stable throughout the reporting period.
* The South region generates the highest sales.
* Profit is concentrated in a few high-performing sub-categories.
* Home Office customers contribute the highest sales.
* Higher discounts are generally associated with lower profitability.
* Standard Class shipping has the longest average delivery time.
* Home Office customers exhibit the highest return rate.
* Opportunities exist to improve profitability by optimizing discount strategies, reducing returns, and strengthening lower-performing regions.

---

# Dashboard Story Summary

The dashboard provides executives with a complete overview of retail business performance.

Overall revenue and profitability remain healthy, supported by stable sales trends and strong-performing product categories. However, the analysis also identifies operational risks related to discounting, delivery performance, and customer returns.

Leadership can use the dashboard to prioritize regional growth initiatives, optimize pricing strategies, improve shipping efficiency, reduce return rates, and focus investments on high-profit product categories.

The dashboard combines multiple business perspectives into a single executive reporting tool that supports informed strategic decision-making.

---

# Assumptions and Limitations

## Assumptions

* Source data is complete and accurate.
* Sales, profit, and return information are correctly recorded.
* Historical performance reflects normal business operations.

## Limitations

* The dashboard is based on historical data and does not predict future performance.
* Relationships shown in the dashboard indicate association rather than causation.
* External factors such as competitor activity, marketing campaigns, inventory constraints, and economic conditions are not included in the analysis.
* Customer-level profitability and forecasting are outside the scope of this project.

---

# Screenshots Included

The project submission includes screenshots demonstrating the completed Tableau dashboard.

```
screenshots/full_dashboard.png
```

Additional worksheet screenshots may also be included to illustrate individual visualizations where required.

---

# Tools Used

* Tableau
* Microsoft Excel

---

# Project Outcome

The final dashboard successfully transforms retail transaction data into an executive decision-support system. It enables leadership to monitor key business metrics, evaluate operational performance, identify growth opportunities, and make data-driven business decisions through interactive visual analytics.
