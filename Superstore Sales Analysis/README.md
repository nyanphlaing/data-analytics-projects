# Superstore Sales Analysis

## Project Overview

Business performance analysis of a US retail superstore covering 9,994 transactions
across 4 years (2014-2017). Analysis performed using Python and SQL to identify
profitability drivers, regional performance gaps, and actionable cost-saving
opportunities.

## Dataset

- **Source:** [Superstore Dataset via Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **Size:** 9,994 transactions
- **Period:** 2014 to 2017

## Tools Used

- Python, pandas, Matplotlib, Seaborn, pandasql, Jupyter Notebook

## SQL Concepts Used

- GROUP BY, WHERE, ORDER BY, SUM, AVG, COUNT, DISTINCT
- CASE WHEN statements for discount banding
- Profit margin calculations across multiple dimensions
- Dual-metric analysis (Sales vs Profit simultaneously)

## Key Findings & Business Recommendations

**Finding 1: Central Region has a profitability problem**
The Central region generates $501k in sales but only a 7.92% profit margin —
nearly half of the West region's 14.94% despite similar sales volume. The East
and West regions are significantly outperforming Central on profitability.

_Recommendation: Conduct a pricing and discount audit in the Central region.
Sales volume is strong but margins suggest systematic over-discounting or
unfavourable product mix._

**Finding 2: Furniture is a near break-even category**
Furniture generates $742k in sales — comparable to Technology's $836k — but
produces only $18,451 in profit at a 2.49% margin vs Technology's 17.40%.
Furniture is consuming significant operational resources for minimal return.

_Recommendation: Review furniture pricing strategy and discount practices.
Consider reducing the furniture range to focus on higher-margin sub-categories,
or implement a minimum margin policy per transaction._

**Finding 3: Discounts above 20% consistently destroy profit**
Transactions with no discount average $66.90 profit per order. Orders with
20-40% discounts average a loss of $77.86 per order. Orders with 40%+ discounts
average a loss of $106.71 per order — costing the business an estimated $135,000
in avoidable losses across 1,393 orders.

_Recommendation: Implement a hard cap of 20% on all discounts. No discount
tier above this threshold generates positive returns. This single policy change
could recover $135,000 in annual profit._

**Finding 4: Revenue is growing but margin improvement is inconsistent**
Sales grew from $484k in 2014 to $733k in 2017 — a 51% increase. However profit
margin fluctuated between 10.23% and 13.43%, suggesting growth is not being
converted into proportional profit improvement.

_Recommendation: Prioritise margin management alongside revenue growth targets.
Sales growth without margin discipline produces diminishing returns._

**Finding 5: Home Office segment is the most profitable per order**
Despite being the smallest segment by volume, Home Office customers generate the
highest profit margin at 14.03% vs Consumer at 11.55%. Consumer customers
represent the largest segment (2,586 orders) but the lowest margin.

_Recommendation: Investigate discount practices in the Consumer segment.
Bringing Consumer margins in line with Corporate levels (13.03%) could
significantly improve overall profitability given the segment's scale._

## Files

- `superstore_analysis.ipynb` — Full analysis notebook
- `Sample - Superstore.csv` — Raw dataset
- `chart1_region_performance.png`
- `chart2_category_performance.png`
- `chart3_discount_vs_profit.png`
- `chart4_annual_trend.png`
- `chart5_segment_performance.png`
