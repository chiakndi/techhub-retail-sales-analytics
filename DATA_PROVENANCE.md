# Dataset and Figure Provenance

| Asset | Origin | What is supported |
|---|---|---|
| `reports/Original_Internship_Report.pdf` | User-supplied four-page internship report | Qualitative findings and embedded Tableau chart screenshots |
| `assets/tableau_original/` | Figures extracted from user-supplied report | Tableau chart shapes and the narrative descriptions, **not** the numerical synthetic results |
| `techhub_retail_data/*.csv` | Custom-generated simulated data based on report topics | Repeatable example of joins and KPI analysis; **not** original internship data |
| `outputs/analysis_exports/` | Calculated from the simulated CSVs | Synthetic analysis tables |
| `assets/simulated_kpi_dashboards/` | Designed using the simulated datasets | Illustrative KPI dashboard images, **not** Tableau originals |
| `reports/LinkedIn_2_Page_Showcase.pdf` | Curated portfolio presentation | Combines original figures and synthetic KPI demonstrations, labeled accordingly |

**Important:** The numeric metric displayed as “32” in the source PDF's customer-value illustration has insufficient unit/time-window context to translate into a predictive CLV or compare against the synthetic results. Do not present it as an independently verified lifetime value.

**Disclosure:** No original transaction-level company dataset or Tableau workbook is included; do not claim this repository reproduces the original company's revenue or customer metrics.
