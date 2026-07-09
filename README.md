# Telco Customer Churn - Milestone 2 (EDA + Preprocessing)

## Structure
```
data/            -> raw dataset (Telco-Customer-Churn.csv)
notebook/        -> telco_churn_eda_preprocessing.ipynb (full pipeline)
results/
  EDA_graphs/    -> 10 EDA plots (churn distribution, tenure, correlation, etc.)
  final_data/    -> X_train.csv, X_test.csv, y_train.csv, y_test.csv
```

## Pipeline covered in the notebook
- Load + inspect data, fix `TotalCharges` dtype
- Missing value handling (median imputation)
- Duplicate removal, drop `customerID`
- Outlier check (IQR) on tenure / MonthlyCharges / TotalCharges
- 10 EDA visualizations
- Encoding: binary map, ordinal (Contract), one-hot (nominal categorical cols)
- Train/test split (80/20, stratified)
- Standardization (fit on train only, applied to test - avoids data leakage)
- Final datasets saved to `results/final_data/`

## Push to GitHub
-> uploaded m
