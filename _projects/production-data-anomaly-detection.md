---
title: Production Data Anomaly Detection
context: Professional Project
category: decision-support
order: 4
featured: false
card_summary: Reusable statistical monitoring tools analyze production and defect data across components, batches, and defect categories. They surface candidate anomalies for engineering review, with live-operation calibration still required.
takeaway: Reusable monitoring tools surfaced candidate production anomalies for engineering review; live-operation validation remained necessary before rollout.
challenge: Identify unusual patterns in production and defect data without pre-existing labels marking known issue periods.
approach:
  - Implemented a transparent statistical detection method using z-scores around moving averages with dynamic upper and lower thresholds.
  - Analyzed individual components, batches, and defect categories at different aggregation levels.
  - Created 2D trend views, 3D defect-location visualizations, and Streamlit applications for exploratory analysis.
outcomes:
  - Produced a reusable monitoring backend and exploratory views that surfaced candidate anomalies for engineering review.
  - Supported analysis by component, batch, defect category, and aggregation level.
  - Live-operation validation and trigger calibration remained necessary before operational rollout.
focus:
  - Statistical anomaly detection
  - Moving statistics
  - 3D visualization
methods:
  - Statistical anomaly detection
  - Moving statistics
  - Production analytics
  - 3D visualization
technologies:
  - Python
  - Streamlit
---
