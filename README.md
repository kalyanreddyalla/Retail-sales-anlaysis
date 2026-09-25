# Retail Sales & Profitability Analysis

Analysis of 8,399 orders from a multi-region retail chain (2009-2012), asking the question a real stakeholder would ask: **where are we making money, where are we losing it, and why?**

## What's in here

- `retail_sales_analysis.ipynb` — the full analysis: data cleaning, KPIs, profitability by sub-category, discount-vs-profit relationship, regional performance, monthly trend, and customer segment value.
- `data/superstore_sales.csv` — source dataset.

## Key findings

- Overall margin is **10.2%** on $14.9M in sales, but that average hides real problems underneath it.
- **4 of 17 product sub-categories are net loss-making** — Tables alone lost over $99k. Strong sales volume does not mean a category is profitable.
- **Discounts above 20% correlate with negative average profit per order.** Below that, discounting is roughly neutral to slightly positive. "Discount harder to sell more" isn't supported by this data as a blanket policy.
- Sales are concentrated in a few regions, and customer segment margins vary by several points — acquisition and retention spend isn't equally valuable everywhere.

## Tools

Python, pandas, matplotlib. No BI tool — deliberately built to show raw data manipulation and chart-building skill rather than relying on a point-and-click tool.

## How to run it

```bash
pip install pandas numpy matplotlib
jupyter notebook retail_sales_analysis.ipynb
```

The notebook is committed with outputs already rendered, so you can also just read it directly on GitHub without running anything.
