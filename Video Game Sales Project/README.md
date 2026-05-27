# Video Game Sales Analysis

## Project Overview

Exploratory analysis of global video game sales data covering 16,327 games across platforms,
genres, and publishers from 1990 to 2016. Analysis performed using both Python and SQL to
identify market trends, top performers, and industry patterns.

## Dataset

- **Source:** [Video Game Sales via Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales)
- **Size:** 16,598 records (16,327 after cleaning)
- **Period:** 1980 to 2020 (analysis focused on 1990 to 2016)

## Tools Used

- Python, pandas, Matplotlib, Seaborn, pandasql, Jupyter Notebook

## Data Cleaning

- Removed 271 rows with missing Year values
- Converted Year column from float to integer format

## Key Findings

**1. Action dominates all genres**
Action games generated 1,722 million units in global sales — 31% more than Sports in
second place at 1,309 million.

**2. PS2 is the best selling platform of all time**
PS2 leads with 1,233 million units sold across 2,127 games, ahead of Xbox 360 at
969 million and PS3 at 949 million.

**3. Nintendo is the dominant publisher by a wide margin**
Nintendo generated 1,784 million in global sales — 63% more than Electronic Arts
in second place at 1,093 million.

**4. Industry peaked in 2008 then declined sharply**
Global sales peaked at 678 million units in 2008 driven by the Wii era and casual
gaming boom, before declining as the market shifted toward mobile and digital
downloads not captured in this dataset.

**5. Wii Sports is the best selling game of all time**
Wii Sports sold 82.74 million units — more than double Super Mario Bros. in second
place at 40.24 million. Four of the top 5 best selling games are Nintendo titles.

## SQL Queries

This project demonstrates SQL skills alongside Python, using pandasql to query
DataFrames with GROUP BY, WHERE, ORDER BY, COUNT, SUM, and LIMIT clauses.

## Files

- `vgsales_analysis.ipynb` — Full analysis notebook with Python and SQL
- `vgsales.csv` — Raw dataset
- `chart1_sales_by_genre.png`
- `chart2_sales_by_platform.png`
- `chart3_sales_by_publisher.png`
- `chart4_sales_by_year.png`
- `chart5_best_selling_games.png`
