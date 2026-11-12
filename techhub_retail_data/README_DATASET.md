# TechHub Retail — Synthetic practice dataset

PROVENANCE: SYNTHETIC / SIMULATED DATA — NOT THE ORIGINAL DATASET USED IN THE INTERNSHIP REPORT.

Source: Custom-generated from the *description* and qualitative findings in the uploaded 4-page “project 4 internship Report..pdf”. The original row-level source data / Tableau workbook were not included. Values and records in these files are fabricated for reproducible practice; **do not present synthetic metrics as the original project results**.

Time range: 2024-01-01 through 2025-12-31 (simulated; the report describes 2025 strategy).
Currency: EUR, no tax; discounts are pre-applied to `revenue_eur`.

## Contents / Keys

- `sales.csv` — one row per order line. `sale_id` unique; `order_id` can repeat for multiple products. `customer_id` -> customers; `product_id` -> products. `revenue_eur = quantity × unit_price_eur × (1 - discount_pct)`; `cost_eur = quantity × unit_cost_eur`; `profit_eur = revenue_eur - cost_eur` (all rounded per line).
- `customers.csv` — one row per simulated customer. `age`, `age_group`, `region`, `loyalty_tier`, `signup_date`.
- `products.csv` — one row per product. `category`, `supplier_id` -> suppliers, `launch_date`, `list_price_eur`, `unit_cost_eur`.
- `suppliers.csv` — one row per supplier. `supplier_name`, `supplier_region`.
- `acquisition.csv` — one row per customer. `customer_id` -> customers, `acquisition_date`, `channel`, `campaign`, `acquisition_cost_eur`.

## Definitions

- Total Revenue = sum(`revenue_eur`).
- Total Profit = sum(`profit_eur`).
- Profit Margin (%) = 100 × Total Profit / Total Revenue.
- AOV = Total Revenue / number of **distinct orders** (`order_id`).
- Observed customer value = customer total recorded revenue during 2024–2025. This is **not a forecast** of true customer lifetime value.
- Product age at purchase (months) = month difference between `order_date` and `launch_date`.
- Marketing channel profitability can be approximated using observed customer profit; it is not causal marketing attribution.

## Notes / limits

Synthetic distributions were designed to provide examples of the report's themes (e.g., strong Q4, smartphones leading revenue, varying margin by product/supplier, variation in acquisition-channel customer value). These patterns are simulated, not verified original findings.

Use the downloadable notebook `TechHub_Retail_Analysis_Colab.ipynb` to analyze these files in Google Colab. Upload the ZIP when prompted.
