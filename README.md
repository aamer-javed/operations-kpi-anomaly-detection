# Operations KPI Anomaly Detection

**Anomaly Detection / Operations Analytics / Decision Support**

This project demonstrates how data science can be used to monitor operational performance and detect unusual KPI patterns across sites, dates, throughput, utilization, downtime, cycle time, and error rates.

The dataset is synthetic and designed to represent warehouse, robotics, or operations-style performance data without exposing any company information.

## Business Problem

Operations teams need to identify abnormal performance patterns early. A sudden drop in throughput, increase in downtime, high error rate, or unusual utilization pattern can indicate process issues, system instability, staffing constraints, equipment problems, or data quality issues.

This project builds an anomaly detection workflow to highlight site-day combinations that deserve review.

## Key Questions

- Which site-day records show abnormal operational behavior?
- Are anomalies driven by low throughput, high downtime, high error rate, or slow cycle time?
- Can rule-based thresholds and machine learning complement each other?
- How should anomalies be ranked for operational review?
- What actions should an operations team take from the results?

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

## Methods

- Exploratory Data Analysis
- Site-Level KPI Trend Analysis
- Rule-Based Anomaly Detection
- Isolation Forest
- Severity Scoring
- Operational Triage
- Business Interpretation

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

## How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Generate synthetic data:

```bash
python src/generate_synthetic_data.py
```

Run anomaly detection:

```bash
python src/detect_anomalies.py
```

## Why This Project Matters

Many analytics projects stop at reporting KPI values. This project moves toward decision support by helping teams identify which performance changes deserve attention first.

The workflow can support questions such as:

- Which site should be reviewed today?
- Is the issue throughput, downtime, error rate, or cycle time?
- Are the anomalies isolated events or recurring patterns?
- Should the team investigate process, equipment, staffing, or data quality?

## Portfolio Value

This project shows practical machine learning applied to operations analytics. It combines domain knowledge, statistical thresholds, anomaly detection, and business interpretation.

## Tools

Python, pandas, NumPy, scikit-learn, matplotlib, anomaly detection, operations analytics

## Author

Aamer Javed  
GitHub: https://github.com/aamer-javed  
Kaggle: https://www.kaggle.com/aamerjavedmce
