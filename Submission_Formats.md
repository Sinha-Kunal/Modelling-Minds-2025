# Submission Format Guidelines

This document outlines the submission requirements for all problem statements in the Modelling Minds Hackathon. Please follow these guidelines carefully to ensure your submission is processed correctly.

## General Submission Requirements

### File Naming Convention
All submissions must follow the format: `{Team ID}_{Track ID}.csv`

Where:
- `Team ID`: Your assigned team identifier
- `Track ID`: The specific track identifier for the problem

### File Format
- All prediction files must be submitted as **CSV files**
- No additional headers or metadata beyond specified columns
- Ensure no missing values in prediction columns

---

## Classification Track

### CCF01X - Canes et Feles
**File Name:** `TeamID_CCF01X.csv`

**CSV Structure:**
```csv
image_file_name,predicted_class
...
```


**Requirements:**
- Predictions for all test images must be included
- Class labels must match the class names exactly
- No missing predictions allowed

---

### CCC01A - Codex of Conundrums
**File Name:** `TeamID_CCC01A.csv`

**CSV Structure:**
```csv
file_name,predicted_category,confidence_score
1.json,algebra,0.89
2.json,geometry,0.76
3.json,calculus,0.92
...
```

**Column Specifications:**
- `problem_id`: String - Unique identifier for each mathematical problem
- `predicted_category`: String - Predicted mathematical category
- `confidence_score`: Float - Model confidence score (0.0 to 1.0)
---

## Forecasting Track

### FBH002T - Bullish Horizons
**File Name:** `TeamID_FBH002T.csv`

**CSV Structure:**
```csv
date,predicted_price_daily_high,predicted_price_daily_low,daily_low_confidence_interval_lower,daily_low_confidence_interval_upper,daily_high_confidence_interval_upper,daily_high_confidence_interval_lower
...
```

**Column Specifications:**
- `date`: String - Date in YYYY-MM-DD format
- `predicted_price_high`: Float - Predicted high price
- `predicted_price_low`: Float - Predicted low price
- `daily_low_confidence_interval_lower`: Float - Lower bound of 90% confidence interval for `predicted_price_low`
- `daily_low_confidence_interval_upper`: Float - Upper bound of 90% confidence interval for `predicted_price_low`
- `daily_high_confidence_interval_lower`: Float - Upper bound of 90% confidence interval for `predicted_price_high`
- `daily_high_confidence_interval_upper`: Float - Upper bound of 90% confidence interval for `predicted_price_high`

**Requirements:**
- Predictions for all requested stock symbols and dates
- Confidence intervals must be mathematically valid (lower < predicted < upper)
- All prices must be positive values

---

### FCT001G - Contours in Time
**File Name:** `TeamID_FCT001G.csv`

**CSV Structure:**
```csv
timestamp,predicted_value,prediction_interval_lower,prediction_interval_upper
0.123,45.67,42.31,48.93
0.124,46.12,42.78,49.46
0.125,128.45,121.33,135.57
...
```

**Column Specifications:**
- `timestamp`: int - Time in Seconds
- `predicted_value`: Float - Predicted value at the timestamp
- `prediction_interval_lower`: Float - Lower bound of 90% prediction interval
- `prediction_interval_upper`: Float - Upper bound of 90% prediction interval

**Requirements:**
- Maintain chronological order within each series
- All timestamps must match the requested forecast horizon
- Prediction intervals must be statistically valid

---

## X-AI Track

### XAE001F - Atlas of Expressions
**File Name:** `TeamID_XAE001F.csv`

**CSV Structure:**
```csv
sample_id,cell_type,top_10_features,feature_importance_scores
...
```

**Column Specifications:**
- `sample_id`: String - Unique sample identifier, given in the barcodes.csv file
- `cell_type`: String - cell type given in the barcodes.csv file
- `top_20_features`: String - Comma-separated list of most important features (genes)
- `feature_importance_scores`: String - Comma-separated importance scores for top 20 features


---

### XRM0002K - Resilient Minds
**File Name:** `TeamID_XRM0002K.csv`

**CSV Structure:**
```csv
patient_id,risk_level,Score(SHAP/LIME/MRMR), risk_factors, issue_type(Depression/Anxiety etc.)
...
```

**Column Specifications:**
---

## Submission Checklist

Before submitting, ensure:
- [ ] File naming follows `TeamID_TrackID.csv` format
- [ ] All required columns are present with correct headers
- [ ] No missing values in prediction columns
- [ ] Data types match specifications
- [ ] CSV file should open correctly without formatting issues
- [ ] All predictions are within valid ranges/categories

## Submission Process

1. Validate your CSV file against the format requirements
2. Test that your file can be read by standard CSV parsers
3. Submit through the designated platform before the deadline
4. Retain a backup copy of your submission file

---

**Note:** Submissions that do not conform to these specifications will be disqualified. When in doubt, please contact the organizing committee.
