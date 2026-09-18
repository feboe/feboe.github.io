---
title: Smart Building Load Forecasting & Battery Optimization
context: Personal Project
category: energy
order: 1
featured: true
card_summary: Using real smart-building data, this project combines leakage-safe 24-hour load forecasting with physically constrained battery optimization. It achieved 8.21% WAPE and tested how operational assumptions change simulated storage value.
takeaway: Real smart-building data yielded 8.21% forecast WAPE and showed when optimized battery dispatch adds value—and how strongly assumptions affect it.
challenge: Use real measurements of building consumption, PV and CHP generation, grid import, and grid export to reconstruct a consistent energy balance, forecast 24-hour load, and evaluate battery-control strategies.
approach:
  - Built a PostgreSQL workflow from Engel et al.’s real-world smart-company-building dataset on Dryad and German day-ahead prices from SMARD.
  - "Forecasting workstream: reconstructed building load and evaluated leakage-safe 24-hour forecasts against daily- and weekly-naive baselines using chronological validation."
  - "Battery workstream: compared heuristic dispatch with a physically constrained rolling-horizon linear program and tested battery capacity, hourly versus 15-minute resolution, terminal state-of-charge valuation, auxiliary consumption, and self-discharge."
outcomes:
  - The Histogram Gradient Boosting model achieved 8.21% weighted absolute percentage error (WAPE) on the held-out 2021 period and outperformed both seasonal baselines.
  - "The building already self-consumed approximately 92% of local generation, limiting surplus-only storage value. Optimization added most value when dynamic prices and grid charging introduced timing decisions: €13.4k versus €9.4k simulated annual operating savings in the 1,000-kWh hourly reference case."
  - "Sensitivity experiments showed that estimated storage value is scenario-dependent: finer temporal resolution increased calculated savings, larger capacities produced diminishing marginal value, and auxiliary consumption materially reduced savings."
note: Battery savings are scenario results, not investment returns. They are measured against corresponding no-battery baselines and exclude purchase, installation, financing, maintenance, replacement, and demand-charge costs.
focus:
  - Time-series forecasting
  - Battery optimization
  - Linear programming
methods:
  - Time-series forecasting
  - Chronological validation
  - Histogram Gradient Boosting
  - Battery simulation
  - Linear programming
technologies:
  - Python
  - PostgreSQL
  - scikit-learn
  - PuLP
repository: https://github.com/feboe/smart-building-energy-optimization
repository_label: View project repository
images:
  - src: /assets/images/projects/smart-building-battery-strategies.png
    alt: Bar chart comparing simulated annual operating savings across battery dispatch strategies for a 1,000 kWh system.
    caption: Initial hourly strategy comparison for a 1,000-kWh system; optimization gains are largest with dynamic prices and permitted grid charging.
---
