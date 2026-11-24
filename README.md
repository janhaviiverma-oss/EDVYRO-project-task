# Customer Churn — Data Quality and Exploratory Analysis

## Project objective
Audit and clean the supplied synthetic customer churn dataset, document quality decisions, validate the cleaned data, calculate summary statistics, and inspect initial patterns.

## Dataset
- Source file: `customer_churn_sample.csv`
- Shape: 15 rows × 11 columns
- Records are synthetic and intended for practice.

## Key findings
- Missing cells: 0
- Duplicate rows: 0
- Churned customers: 7
- Retained customers: 8
- Observed churn rate: 46.7%
- IQR-screened numeric outliers: 0

## Cleaning and validation
Text values were trimmed and repeated spaces normalized. Numeric data types were enforced. No rows were removed and no missing values were imputed because the initial audit found no missing cells or duplicate rows. The 1.5 × IQR rule flagged no numeric outliers. All customer IDs are unique. `TotalCharges = MonthlyCharges × TenureMonths` for all supplied records.

## Initial patterns
- Contract churn rates: Month-to-Month: 100.0%, One Year: 0.0%, Two Year: 0.0%
- Average tenure: churned 7.0 months; retained 29.1 months.
- Average support tickets: churned 4.29; retained 1.00.

## Files
- `customer_churn_cleaned.csv`
- `customer_churn_analysis.xlsx`
- `customer_churn_data_quality_report.pdf`
- `README.md`
- `customer_churn_sample.csv` (original source dataset)

## Limitations
This is a 15-row synthetic sample. The observed patterns are descriptive, not causal, and should not be generalized to a real customer population.

## Submission
Upload this folder or its ZIP to a GitHub repository or Google Drive folder. Set access to public or anyone-with-the-link viewer, then submit that single repository/folder URL.
