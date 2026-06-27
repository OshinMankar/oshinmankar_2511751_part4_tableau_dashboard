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

This flow enables executives to quickly identify growth opportunities, operational inefficiencies, and potential business risks.
