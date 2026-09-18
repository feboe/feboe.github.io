---
title: Negative Day-Ahead Price Analysis
context: Personal Project
category: energy
order: 2
featured: false
card_summary: A Python and PostgreSQL pipeline analyzes when negative German day-ahead prices occur and which system conditions accompany them. Results show growing frequency from 2022–2025, concentrated around spring and summer middays.
takeaway: Negative price hours grew from 2022–2025, clustering around spring and summer middays rather than becoming substantially longer events.
challenge: Determine when negative electricity prices occur in the German–Luxembourg bidding zone and which system and calendar conditions are associated with them.
approach:
  - Built a Python and PostgreSQL pipeline for SMARD price, demand, wind, solar, and calendar data from 2022–2025.
  - Created SQL quality and analysis views for residual load, negative-price hours, event duration, price intensity, and calendar patterns.
  - Documented the limits of the exploratory analysis, including simplified residual load and changes in market time resolution.
outcomes:
  - Negative-price hours increased across 2022–2025 and concentrated around midday, particularly in spring and summer.
  - Shares were higher on weekends and holidays and associated with low forecast residual load, though residual load did not explain every event.
  - Most continuous events lasted one to eight hours; the median rose only from 4.5 to 5.5 hours, indicating more frequent rather than much longer events.
focus:
  - Energy-market analysis
  - Time-series analysis
  - ETL
methods:
  - Exploratory data analysis
  - Time-series analysis
  - ETL
technologies:
  - Python
  - SQL
  - PostgreSQL
repository: https://github.com/feboe/energy-data-sql-pipeline
repository_label: View project repository
images:
  - src: /assets/images/projects/negative-price-patterns.png
    alt: Heatmap showing negative day-ahead price hours by month and local hour of day.
    caption: Negative-price hours in the German–Luxembourg bidding zone, 2022–2025; events concentrate around spring and summer middays.
---
