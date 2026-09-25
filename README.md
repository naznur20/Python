# Block 3 — Sales Analysis and Its Dependence on Weather

A Jupyter notebook analyzing online store/retail chain sales data for the period January–August 2018.

## What the Notebook Does

1. **Data loading and preparation** — reading the source dataset (`data.csv`), converting the `Date` column to datetime format.
2. **Sales aggregation** — grouping data by date, counting the number of sales per day (`grouped_df`).
3. **Sales dynamics visualization** — a line chart of daily sales with analysis of seasonality and outliers.
4. **Statistical outlier detection** — identifying anomalous days using the IQR method.
5. **Warehouse analysis** — finding the top-selling product on Wednesdays during the summer months (June–August) for a specific warehouse.
6. **Weather analysis** — retrieving historical temperature data for Astana via the Open-Meteo API (ERA5 archive), merging it with sales data, and building a chart of the combined dynamics of `Number of Sales` and `Temperature`.

## Stack

* Python, pandas, numpy
* matplotlib, seaborn
* requests (for Open-Meteo API calls)

## Files

* `Блок_3.ipynb` — main notebook with the analysis
* `data.csv` — source sales data (date, warehouse, counterparty, item/nomenclature, quantity)

## Weather Data Source

[Open-Meteo Historical Weather API](https://open-meteo.com/en/docs/historical-weather-api) — a free ERA5 historical data API that requires no authorization.
