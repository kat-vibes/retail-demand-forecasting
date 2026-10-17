# Retail Sales Analytics for Inventory Planning

Descriptive retail sales analysis using the M5 dataset. The project focuses on practical inventory questions rather than AI or demand forecasting models.

## Questions explored

- Which categories and stores generate the most sales?
- How does demand change by weekday and month?
- Do recorded holidays and events coincide with different sales levels?
- Which products drive the largest share of unit volume?
- How can ABC analysis support inventory prioritization?

## Contents

- `01_data_overview.ipynb` — dataset overview, sales dynamics, seasonality, events, prices, top products and ABC analysis.

## Data

The analysis uses the public [M5 Forecasting dataset](https://www.kaggle.com/competitions/m5-forecasting-accuracy/data). Raw CSV files are not included in this repository because of their size. Download them from Kaggle and place them in `data/raw/`.

## Tools

Python, pandas, NumPy, Matplotlib, Seaborn and Jupyter Notebook.

## Main findings

FOODS has the largest unit volume, sales differ substantially by store, weekends are stronger than most weekdays, and a relatively focused group of products accounts for most units sold. These patterns support store-specific replenishment, closer monitoring of A-items and preparation for recurring demand peaks.
