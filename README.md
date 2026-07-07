# Operations KPI Anomaly Detection

This project demonstrates how data science can be used to monitor operational performance and detect unusual KPI patterns across sites, dates, throughput, utilization, downtime, and error rates.

The dataset is synthetic and designed to represent warehouse, robotics, or operations-style performance data without exposing any company information.

## Business Problem

Operations teams need to identify abnormal performance patterns early. A sudden drop in throughput, increase in downtime, high error rate, or unusual utilization pattern can indicate process issues, system instability, staffing constraints, equipment problems, or data quality issues.

This project builds an anomaly detection workflow to highlight site-day combinations that deserve review.

## Objectives

- Generate safe synthetic operations KPI data
- Explore site-level trends and KPI distributions
- Detect anomalies using rule-based and machine learning methods
- Rank anomalies by severity
- Translate results into operational insights

## Dataset

Example fields:

| Column | Description |
|---|---|
| date | Daily KPI date |
| site | Simulated operating site |
| throughput_units | Units processed |
| utilization_pct | Utilization percentage |
| downtime_minutes | Daily downtime |
| error_rate_pct | Error rate percentage |
| avg_cycle_time_seconds | Average operational cycle time |
| labor_hours | Labor hours |
| anomaly_label | Synthetic indicator for injected anomalies |

## Project Structure

```text
operations-kpi-anomaly-detection/
├── README.md
├── data/
│   └── sample/
│       └── synthetic_operations_kpi.csv
├── notebooks/
│   └── 01_operations_kpi_anomaly_detection.ipynb
├── src/
│   ├── generate_synthetic_data.py
│   └── detect_anomalies.py
├── reports/
│   └── figures/
├── requirements.txt
└── .gitignore
```

## Methods

- Exploratory Data Analysis
- KPI Trend Analysis
- Rule-Based Anomaly Detection
- Isolation Forest
- Severity Scoring
- Business Interpretation

## Why This Project Matters

This project connects machine learning to real operational decision-making. Instead of only reporting KPI values, anomaly detection can help teams prioritize investigation and respond before performance issues become larger business problems.

## Status

Project scaffold created. Next steps:

- Expand EDA notebook
- Add trend and anomaly visualizations
- Compare rule-based anomalies with Isolation Forest results
- Add recommendations for operations monitoring

## Tools

Python, pandas, NumPy, scikit-learn, matplotlib, anomaly detection, operations analytics

## Author

Aamer Javed  
GitHub: https://github.com/aamer-javed
Kaggle: https://www.kaggle.com/aamerjavedmce
