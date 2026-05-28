# Netflix Content Analysis

## Project Overview

Exploratory analysis of Netflix's content library covering 8,807 titles across
movies and TV shows. Analysis performed using Python and SQL to identify content
trends, country strategies, and genre patterns.

## Dataset

- **Source:** [Netflix Shows via Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Size:** 8,807 titles (8,790 after cleaning)
- **Period:** Content added up to 2021

## Tools Used

- Python, pandas, Matplotlib, Seaborn, pandasql, Jupyter Notebook

## Data Cleaning

- Filled 2,634 missing director values with 'Unknown' rather than dropping rows
- Filled 825 missing cast and 831 missing country values with 'Unknown'
- Dropped only 17 rows with missing rating, duration, and date_added values
- Extracted year and month from date_added for trend analysis

## Key Findings

**1. Netflix is predominantly a movie platform**
69.7% of Netflix content is movies (6,126 titles) vs 30.3% TV shows (2,664 titles).

**2. The US dominates content production**
The United States produced 2,809 titles — nearly 3x more than India in second
place at 972 titles, reflecting Hollywood's global content dominance.

**3. Netflix aggressively expanded its library from 2017 to 2019**
Titles added grew from 426 in 2016 to 2,016 in 2019. The drop in 2020 and 2021
reflects COVID-19 production shutdowns reducing new content availability.

**4. International Movies and Dramas lead all genres**
International Movies top the genre list at 2,752 titles, signalling Netflix's
deliberate strategy to invest in non-English content for global subscriber growth.

**5. Content strategy varies significantly by country**
India is movie-first (893 movies vs 79 TV shows) driven by Bollywood, while Japan
and South Korea are TV-first markets (167 and 158 TV shows respectively) reflecting
anime and K-drama dominance. The UK shows a near-equal split.

## SQL Concepts Used

GROUP BY, WHERE, COUNT, subqueries, IN operator, multiple column grouping

## Files

- `netflix_analysis.ipynb` — Full analysis notebook
- `netflix_titles.csv` — Raw dataset
- `chart1_content_type.png`
- `chart2_content_by_country.png`
- `chart3_content_per_year.png`
- `chart4_top_genres.png`
- `chart5_content_mix.png`
