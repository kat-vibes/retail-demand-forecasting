# Retail Sales and Inventory Planning

A Python notebook project using M5 retail sales data. I compare sales across stores, categories and dates, group products by unit volume, and work through a simple stock calculation.

## Notebooks

1. `01_data_overview.ipynb`: sales, calendar and price tables; category and store totals; events and ABC groups.
2. `02_sales_dynamics.ipynb`: daily sales and weekday and monthly averages.
3. `03_inventory_prioritization.ipynb`: category and store shares, plus product ABC groups.
4. `04_inventory_planning.ipynb`: a 28-day mean baseline for the next week, a reorder point and a weekly order-up-to calculation.

## Run locally

Use Python 3.10 or newer. Install the packages in `requirements.txt`, then start Jupyter from the project folder and run each notebook from top to bottom. Each notebook loads its own data.

Download the [M5 competition data](https://www.kaggle.com/competitions/m5-forecasting-accuracy/data) and put these files in `data/raw/`:

- `sales_train_validation.csv`
- `calendar.csv`
- `sell_prices.csv`

The CSV files are not included in the repository. Use the validation sales file: it contains 1,913 observed days. The evaluation file covers a different period.

## What the analysis covers

FOODS leads in total units, store volumes differ, and aggregate sales vary by weekday. These are descriptions of recorded sales, not estimates of lost sales or profit. Monthly comparisons do not separate seasonality from trends and sample coverage. Event-day comparisons do not measure causal effects.

ABC groups use units rather than revenue and combine all stores. The stock calculation uses one high-volume example, assumed lead times and a hypothetical inventory position. Forecast accuracy has not been evaluated on held-out dates, so the calculated order quantity is an example rather than a purchasing recommendation.
