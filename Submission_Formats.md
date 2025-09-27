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

## 🔍 Classification Track

### CCF01X - Canes et Feles (Animal Image Classification)
**File Name:** `TeamID_CCF01X.csv`

**CSV Structure:**
```csv
image_id,predicted_class
img_001.jpg,dog
img_002.jpg,cat
img_003.jpg,dog
...
```


**Requirements:**
- Predictions for all test images must be included
- Class labels must match the class names exactly
- No missing predictions allowed

---

### CCC01A - Codex of Conundrums (Mathematical Problem Classification)
**File Name:** `TeamID_CCC01A.csv`

**CSV Structure:**
```csv
problem_id,predicted_category,confidence_score
prob_001,algebra,0.89
prob_002,geometry,0.76
prob_003,calculus,0.92
...
```

**Column Specifications:**
- `problem_id`: String - Unique identifier for each mathematical problem
- `predicted_category`: String - Predicted mathematical category
- `confidence_score`: Float - Model confidence score (0.0 to 1.0)
---

## 📈 Forecasting Track

### FBH002T - Bullish Horizons (Stock Price Forecasting)
**File Name:** `TeamID_FBH002T.csv`

**CSV Structure:**
```csv
date,predicted_price,confidence_interval_lower,confidence_interval_upper
2025-09-29,180.45,175.20,185.70
2025-09-30,181.23,176.01,186.45
2025-09-29,2750.30,2700.15,2800.45
...
```

**Column Specifications:**
- `stock_symbol`: String - Stock ticker symbol
- `date`: String - Date in YYYY-MM-DD format
- `predicted_price`: Float - Predicted closing price
- `confidence_interval_lower`: Float - Lower bound of 95% confidence interval
- `confidence_interval_upper`: Float - Upper bound of 95% confidence interval

**Requirements:**
- Predictions for all requested stock symbols and dates
- Confidence intervals must be mathematically valid (lower < predicted < upper)
- All prices must be positive values

---

### FCT001G - Contours in Time (Time Series Forecasting)
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

### XAE001F - Atlas of Expressions (Gene Expression Analysis with XAI)
**File Name:** `TeamID_XAE001F.csv`

**CSV Structure:**
```csv
sample_id,cell_type,class_probability,top_10_features,feature_importance_scores
...
```

**Column Specifications:**
- `sample_id`: String - Unique sample identifier
- `cell_type`: String - cell type given in the barcodes.csv file
- `class_probability`: Float - Probability of predicted class (0.0 to 1.0)
- `top_20_features`: String - Comma-separated list of most important features
- `feature_importance_scores`: String - Comma-separated importance scores for top 20 features

**Requirements:**
- Feature importance scores must sum to ≤ 1.0 for top 20 features
- Explanations must be concise and scientifically meaningful

---

### XRM0002K - Resilient Minds (Mental Health Data Analysis with XAI)
**File Name:** `TeamID_XRM0002K.csv`

**CSV Structure:**
```csv
patient_id,risk_level,risk_probability,primary_risk_factors,risk_factor_weights,intervention_recommendation,explanation
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
