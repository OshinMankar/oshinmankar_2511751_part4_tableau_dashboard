# Business Insights

## Calculated Fields

### 1. Profit Margin

Formula

```
SUM([Profit]) / SUM([Sales])
```

Purpose

Measures profitability for every sales dollar generated.

Business Value

- Compare profitability across regions
- Identify low-margin categories
- Monitor overall financial health

---

### 2. Cost

Formula

```
SUM([Sales]) - SUM([Profit])
```

Purpose

Estimates total product cost.

Business Value

- Compare revenue versus cost
- Understand cost-heavy categories
- Analyze operational efficiency

---

### 3. Average Order Value

Formula

```
SUM([Sales]) / COUNTD([Order ID])
```

Purpose

Calculates average customer spend per order.

Business Value

- Evaluate customer purchasing behavior
- Compare customer segments
- Measure campaign effectiveness

---

### 4. Return Rate

Formula

```
SUM([Return Flag]) / COUNTD([Order ID])
```

Purpose

Measures percentage of returned orders.

Business Value

- Identify problematic products
- Detect quality issues
- Monitor customer satisfaction

---

### 5. Shipping Delay Bucket

Formula

```
IF [delivery_days] <=2 THEN "Fast (0-2 Days)"

ELSEIF [delivery_days] <=5 THEN "Standard (3-5 Days)"

ELSE "Delayed (6+ Days)"

END
```

Purpose

Groups deliveries into meaningful business categories.

Business Value

- Monitor shipping performance
- Identify logistics bottlenecks
- Compare ship modes

---

# Executive Dashboard Story

The dashboard is designed to guide leadership through a logical business narrative:

1. Overall business performance using KPI cards.
2. Monthly sales and profit trends.
3. Product category profitability.
4. Customer segment performance.
5. Geographic performance.
6. Impact of discounts on profitability.
7. Shipping efficiency.
8. Product return analysis.

9. # Business Insights

## Insight 1: Sales Trend

### Observation

Monthly sales remain relatively stable throughout the reporting period with moderate fluctuations. Sales range between approximately **6.30M** and **10.86M** per month.

### Data Evidence

* Highest monthly sales: **10.86M**
* Lowest monthly sales: **6.30M**
* Most months record sales between **8M–10M**.

### Business Interpretation

The business demonstrates consistent sales performance without extreme volatility. However, certain months experience noticeable declines, indicating possible seasonality or promotional effects.

### Recommended Action

Investigate the factors behind low-performing months and replicate strategies used during peak sales periods. Consider planning marketing campaigns ahead of historically weaker months.

---

# Insight 2: Regional Performance

### Observation

The **South** region generates the highest sales, while the **East** region records the lowest sales among all regions.

### Data Evidence

* South: **64.69M**
* North: **54.56M**
* West: **48.91M**
* East: **48.86M**

### Business Interpretation

Sales performance varies significantly across regions, suggesting differences in customer demand, market penetration, or sales effectiveness.

### Recommended Action

Study successful practices in the South region and evaluate whether similar sales strategies can be implemented in lower-performing regions, particularly the East.

---

# Insight 3: Category and Sub-Category Profitability

### Observation

Profitability is concentrated within a small number of product sub-categories.

### Data Evidence

* Highest profit sub-category: **Copiers (7.31M)**
* Other strong performers include **Accessories**, **Phones**, and **Machines**.
* Several sub-categories generate profits below **0.40M**.

### Business Interpretation

A significant portion of total profit comes from only a few product lines, while many sub-categories contribute relatively little.

### Recommended Action

Increase investment in high-profit sub-categories while reviewing pricing, product assortment, and demand for low-profit products.

---

# Insight 4: Customer Segment Behavior

### Observation

The **Home Office** customer segment generates the highest sales.

### Data Evidence

* Home Office: **74.50M**
* Consumer: **71.89M**
* Corporate: **70.63M**

### Business Interpretation

Although sales are fairly balanced across customer segments, Home Office customers contribute the greatest revenue.

### Recommended Action

Develop targeted promotions and loyalty programs for the Home Office segment while identifying opportunities to increase purchases from Consumer and Corporate customers.

---

# Insight 5: Discount Impact on Profit

### Observation

The scatter plot and regression trend line indicate a negative relationship between discounts and profit.

### Data Evidence

* Profit generally decreases as discount percentages increase.
* The trend line shows a downward slope across discount levels.

### Business Interpretation

Higher discounts appear to reduce profitability, indicating that excessive discounting may negatively affect business margins.

### Recommended Action

Review current discount policies and evaluate whether discounts are generating sufficient additional sales to justify lower profits. Consider targeted rather than blanket discount strategies.

---

# Insight 6: Shipping Performance

### Observation

Standard Class shipping has the longest average delivery time, while Same Day shipping is the fastest.

### Data Evidence

* Standard Class: **4.7 days**
* Second Class: **2.7 days**
* First Class: **1.8 days**
* Same Day: **0.4 days**

### Business Interpretation

Delivery performance aligns with expected shipping priorities. Customers selecting Standard Class experience substantially longer delivery times.

### Recommended Action

Monitor customer satisfaction for Standard Class deliveries and explore logistics improvements to reduce delivery times where operationally feasible.

---

# Insight 7: Return Pattern

### Observation

The Home Office customer segment has the highest return rate.

### Data Evidence

* Home Office: **5.67%**
* Corporate: **4.00%**
* Consumer: **3.91%**

### Business Interpretation

Higher return rates within the Home Office segment may indicate product suitability issues, customer expectations, or purchasing behavior unique to this segment.

### Recommended Action

Analyze returned products within the Home Office segment to identify recurring issues and implement corrective actions such as improved product descriptions, quality improvements, or customer support.

---

# Insight 8: Business Risk and Opportunity

### Observation

The dashboard highlights both strong revenue generation and opportunities for improving profitability through operational and pricing decisions.

### Data Evidence

* Total Sales: **217.02M**
* Total Profit: **33.31M**
* Profit Margin: **15.35%**
* Higher discounts correspond with lower profits.
* Profit is concentrated in a limited number of sub-categories.

### Business Interpretation

The business is financially healthy but relies heavily on a few profitable product lines. High discounts and elevated return rates in specific customer segments represent potential risks to long-term profitability.

### Recommended Action

Focus on expanding high-performing product categories, optimizing discount strategies, reducing return rates, and improving lower-performing regions. These initiatives can improve both profitability and sustainable business growth.


This flow enables executives to quickly identify growth opportunities, operational inefficiencies, and potential business risks.
