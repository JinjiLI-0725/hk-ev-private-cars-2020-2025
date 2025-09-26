# HK Private Cars 2020–2025 — EV Adoption & Brand Shares

A compact portfolio project that scrapes, cleans, and analyzes Hong Kong *private car first registrations* (2020–2025), with a focus on **EV adoption** and **brand performance**.

**What’s inside**

- **Python**: requests + pandas for scraping & cleaning, matplotlib for charts  
- **SQL**: ad-hoc analysis with DuckDB/SQLite (via `pandas.read_sql_query`)  
- **Visualization**: ready-to-publish images; Tableau recipes included  
- **Reproducible notebooks**: end-to-end from raw HTML to insights

---

## Highlights

|  |  |
|---|---|
| **EV share — 2020–2025** | **EV volume (12-month rolling)** |
| ![EV share](images/Overall_EV_share_trend_2020-2025.png) | ![EV volume 12m](images/EV_volume_12month_rolling.png) |
| **Top brands (2025 H1)** |  |
| ![Top brands 2025H1](images/top_ev_brands_2020_2025H1.png) |  |


**Quick takeaways**
- EV share rose rapidly post-2021, with a brief cooldown and re-acceleration in 2025H1.  
- The 12-month rolling series smooths monthly volatility and shows the structural uptrend.  
- 2025H1 brand leaderboard is led by **BYD**, **TESLA**, and **TOYOTA** (registrations).

---

## Project structure
├─ hk_cars_scraping_cleaning_2020_25.ipynb # Scrape + clean + export tidy tables
├─ hk_ev_trend_analysis .ipynb # (Exploratory) pandas + matplotlib analysis
├─ hk_ev_trend_SQL_analysis.ipynb # SQL queries (DuckDB/SQLite via pandas)
├─ ev.db # (optional) a small DB used by the SQL notebook
├─ webbsite_hk_private_cars_by_month.xls # Brand x fuel x month (cleaned)
├─ webbsite_hk_private_cars_monthly_SUM_2020_2025.xls
└─ images/
├─ Overall_EV_share_trend_2020-2025.png
├─ EV_volume_12month_rolling.png
├─ top_ev_brands_2020_2025H1.png
├─ top_ev_brands_panel_2021_2025.png
├─ tesla_ev_share_trend.png
├─ Tesla_share_of_EV_12_monthrolling.png
└─ ev_monthly_tesla_vs_byd.png
## License
- Code: MIT © 2025 Jinji Li
- Charts & images (folder `/images`): CC BY 4.0 © 2025 Jinji Li
- Data source: Hong Kong Transport Dept via webb-site (for research/educational use). Please follow the original site's terms.
