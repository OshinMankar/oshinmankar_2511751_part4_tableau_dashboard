# Chart Selection Justification
## Dashboard Overview

The Retail Sales Performance Dashboard was designed to provide leadership with an executive summary of sales performance, profitability, customer behavior, operational efficiency, and return trends. Each visualization was selected based on the business question it answers while following visualization best practices, minimizing clutter, and ensuring easy interpretation.

## 1. Sales Trend View

### Chart Type: Line Chart

### Business Question

How are sales changing over time?

### Why this chart?

A line chart is the most effective visualization for time-series data because it clearly displays trends, seasonal fluctuations, and changes in sales over time. It enables leadership to quickly identify periods of growth or decline.

### Fields Used
Columns: Order Date (Month-Year)
Rows: SUM(Sales)
Label: SUM(Sales)
Filter: Order Date, Region, Customer Segment, Sub-Category
Design Principle Applied

A continuous Month-Year axis was used to accurately represent the passage of time and avoid misleading comparisons between different years.

### Mistake Avoided

Avoided using a bar chart, which is less effective for showing continuous trends. Also avoided displaying incomplete yearly data that could create misleading declines.

## 2. Regional Performance View

### Chart Type: Horizontal Bar Chart

### Business Question

Which region performs best?

### Why this chart?

A horizontal bar chart provides a clear comparison of sales across regions and makes ranking categories easy to interpret.

### Fields Used
Rows: Region
Columns: SUM(Sales)
Color: SUM(Sales)
Label: SUM(Sales)
Filter: Region, Customer Segment, Date
Design Principle Applied

Bars are sorted from highest to lowest sales so executives can immediately identify the strongest and weakest regions.

### Mistake Avoided

Avoided pie charts, which make comparisons between categories more difficult.

## 3. Category Profitability View

### Chart Type: Bar Chart

### Business Question

Which product sub-categories generate the highest profit?

### Why this chart?

Bar charts are ideal for comparing profitability across multiple categories. They clearly highlight top-performing and lower-performing product groups.

### Fields Used
Columns: Sub-Category
Rows: SUM(Profit)
Color: SUM(Profit)
Label: SUM(Profit)
Filter: Category, Region
Design Principle Applied

Consistent color encoding and sorted values improve readability and make high-profit products easy to identify.

### Mistake Avoided

Avoided treemaps because precise comparisons between product profits are easier with bar charts.

## 4. Customer Segment View

### Chart Type: Bar Chart

### Business Question

Which customer segment contributes the highest sales?

### Why this chart?

A bar chart enables straightforward comparison between customer segments and quickly communicates relative sales performance.

### Fields Used
Columns: Customer Segment
Rows: SUM(Sales)
Color: Customer Segment
Label: SUM(Sales)
Filter: Region, Date
Design Principle Applied

Limited categories and clear labels make comparisons easy without overwhelming the user.

### Mistake Avoided

Avoided stacked charts because they reduce the accuracy of comparing individual segment performance.

## 5. Discount vs Profit View

### Chart Type: Scatter Plot with Trend Line

### Business Question

How does discount affect profit?

### Why this chart?

A scatter plot is the most appropriate visualization for examining the relationship between two continuous variables. Adding a trend line makes the overall relationship easier to interpret.

### Fields Used
Columns: Discount
Rows: Profit
Detail: Sub-Category
Trend Line: Linear Trend
Filter: Region, Customer Segment
Design Principle Applied

The scatter plot allows individual observations to remain visible while the trend line summarizes the overall relationship.

### Mistake Avoided

Avoided using a line chart because discount values do not represent a time sequence.

## 6. Return Analysis View

### Chart Type: Horizontal Bar Chart

### Business Question

Which customer segment has the highest return rate?

### Why this chart?

A horizontal bar chart provides a clear comparison of return rates across customer segments and helps identify areas with higher operational risk.

### Fields Used
Rows: Customer Segment
Columns: Return Rate
Color: Return Rate
Label: Return Rate
Filter: Region, Date
Design Principle Applied

Simple bars and percentage labels allow leadership to compare return performance quickly.

### Mistake Avoided

Avoided pie charts because percentage differences are easier to compare using bars.

## 7. Shipping Performance View

### Chart Type: Horizontal Bar Chart

### Business Question

Which shipping mode has the longest delivery time?

### Why this chart?

A horizontal bar chart clearly compares average delivery days across shipping modes and highlights operational efficiency differences.

### Fields Used
Rows: Ship Mode
Columns: AVG(Delivery Days)
Color: Ship Mode
Label: AVG(Delivery Days)
Filter: Region, Date
Design Principle Applied

Average delivery time is displayed using a common numeric scale, making comparisons accurate and easy.

### Mistake Avoided

Avoided using counts of orders, which would not answer the business question regarding delivery performance.

## KPI Cards
### Business Question

What is the overall business performance?

### KPIs Included
Total Sales
Total Profit
Total Orders
Profit Margin
Design Principle Applied

KPIs are positioned at the top of the dashboard to establish a clear visual hierarchy and provide an executive summary before detailed analysis.

### Mistake Avoided

Avoided displaying large unformatted numbers by using abbreviated values (e.g., 217.02M) and percentages for readability.

## Overall Dashboard Design Principles
Clear visual hierarchy with KPIs first, followed by detailed analysis.
Consistent color usage to distinguish sales, profit, and operational metrics.
Minimal clutter through appropriate spacing and selective labeling.
Business-friendly formatting using millions (M) and percentage values.
Interactive filters (Region, Sub-Category, Customer Segment, and Date) enable focused analysis.
Dashboard action filters allow users to explore relationships across multiple visualizations.
Appropriate sorting and labeling improve readability and support faster executive decision-making.
