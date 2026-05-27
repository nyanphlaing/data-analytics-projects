# E-Commerce Sales Analysis

## Project Overview

Exploratory data analysis of a UK-based online retailer's transaction data containing 541,909 records across 37 countries. The goal was to identify revenue trends, top performing products, customer behaviour patterns, and peak trading periods.

## Dataset

- **Source:** [UCI E-Commerce Dataset via Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
- **Size:** 541,909 transactions
- **Period:** December 2010 to December 2011

## Tools Used

- Python, pandas, matplotlib, seaborn, Jupyter Notebook

## Data Cleaning

- Removed 144,025 rows including cancelled orders, missing customer IDs, and invalid prices
- Converted date column to datetime format
- Created a Revenue column (Quantity x UnitPrice)

## Key Findings

**1. The UK dominates revenue**
The UK generated £7.3 million — over 25x more than the second highest country (Netherlands at £285,000), indicating the business is heavily UK-dependent with limited international penetration.

**2. Strong seasonal peak in Q4**
Revenue climbs steadily from August, peaking at £1.15 million in November driven by Christmas gift purchasing. February and April show consistent dips.

**3. Top selling products are novelty and homeware items**
Paper Craft Little Birdie and Medium Ceramic Storage Jar lead volume at 80,000+ units sold, suggesting strong demand for low-cost decorative items.

**4. Peak trading hours are 10am to 1pm**
Revenue is concentrated in business hours with a noon peak, consistent with a B2B wholesale customer base rather than individual consumers.

**5. Revenue is concentrated in top customers**
Customer 14646 alone generated £280,000 — nearly 3x the 10th highest customer, indicating high dependency on a small number of accounts.

## Files

- `analysis.ipynb` — Full analysis notebook
- `data.csv` — Raw dataset
- `chart1_revenue_by_country.png`
- `chart2_monthly_revenue.png`
- `chart3_top_products.png`
- `chart4_revenue_by_hour.png`
- `chart5_top_customers.png`
