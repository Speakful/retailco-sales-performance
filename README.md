# RetailCo Sales Performance Analysis

Use case homework for Spaulding Ridge — Improving Sales Performance at a Retail Chain.

## What this covers
- Underperforming "stores" (customer city used as a proxy, since the dataset has no store-level data)
- Customer purchasing patterns
- Seasonal trends across 2023

## Data quality notes
- `customer_id` and `campaign_id` in transactions.csv carry an extra "1" prefix (e.g. C1001 vs C001) — corrected during cleaning
- Dates are in day/month/year format
- No store-level data exists in any file; city is used as a stand-in for store/region
- Campaign `target_audience` (e.g. "Gold Tier") cannot be verified since customers.csv has no tier field
- `stock_quantity` in products.csv is a single point-in-time snapshot, not a history

## Folder structure
- `data/raw/` — original CSV files as received
- `data/clean/` — cleaned/merged data after fixing the ID prefix and date format issues
- `notebooks/` — the analysis notebook (cleaning, merging, exploring, insights)
- `dashboard/` — dashboard files/exports (Power BI, Tableau, or similar)
- `slides/` — the 2-3 slide presentation

## How to run
1. Place raw CSVs in `data/raw/`
2. Open `notebooks/01_analysis.ipynb` and run top to bottom
3. Cleaned output lands in `data/clean/`
4. Open the dashboard file in `dashboard/` to explore visuals
