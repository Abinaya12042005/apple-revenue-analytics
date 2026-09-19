# Apple Revenue Analytics Dashboard

Power BI dashboard analyzing Apple's revenue across 8 fiscal years (FY2018-2025) 
and 5 geographic segments, built using real data sourced from Apple's SEC filings.

## Overview
- **Data Source:** Apple 10-K filings and quarterly earnings releases (SEC EDGAR)
- **Tools:** Power BI, Python (Pandas) for data cleaning, DAX for calculations
- **Scope:** Category revenue (iPhone, Mac, iPad, Wearables, Services) and 
  Geography revenue (Americas, Europe, Greater China, Japan, Rest of Asia Pacific)

## Key Insights
- Services revenue grew from $39.7B (2018) to $109.2B (2025) — nearly 3x growth
- iPhone remains ~53% of total revenue, showing concentration risk
- Greater China revenue dipped in FY2024 before partial recovery
- Total revenue grew 57% over 7 years ($265.6B → $416.2B)

## Data Pipeline
1. Extracted quarterly/annual segment data from SEC 10-K and 8-K filings
2. Cleaned and validated using Python (cross-checked Category totals vs 
   Geography totals per year to catch data entry errors)
3. Modeled in Power BI with a dedicated Date table and DAX measures
4. Built custom Apple-branded theme (dark page background, light contrast cards)

## Dashboard Preview
![Dashboard Screenshot](dashboard/screenshots/dashboard_overview.png)

## Files
- `data/apple_revenue_annual.csv` — Verified annual revenue by category and geography
- `data/apple_revenue_quarterly_template.csv` — Quarterly breakdown (partial, ongoing)
- `dashboard/apple_revenue_dashboard.pbix` — Power BI file
- `data_validation.py` — Python script for cleaning and cross-validation checks
