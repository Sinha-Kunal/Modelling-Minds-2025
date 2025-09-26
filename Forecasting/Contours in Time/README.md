# Modelling Minds - VITMAS
# Contours in Time
# Track ID: FCT001G
**Dataset Link:** . 
## Objective
Time series forecasting to predict y values for the next 5 seconds, generating 1000 prediction points within that 5-second timeframe using historical temporal data.

## Dataset Description
This dataset contains temporal data in CSV format with time-value pairs. The task involves predicting future y values using time series forecasting techniques for a specific 5-second prediction window.

**Data Format:** CSV file containing historical time series data

**Columns (2 total):**
- **t**: Time in seconds
- **y**: Corresponding y values

**Directory Structure:**
```
contours in time/
└── contours_in_time.csv
```

**Task Requirements:**
- Predict y values for the next 5 seconds from the last data point
- Generate exactly 1000 prediction points within the 5-second window
- Focus on time series forecasting methodology

## Evaluation Metrics

### 1. RMSE (Root Mean Square Error)
**Formula:** RMSE = √(Σ(ŷᵢ - yᵢ)² / n)
### 2. R² (R-squared/Coefficient of Determination)
**Formula:** R² = 1 - (SS_res / SS_tot)
where SS_res = Σ(yᵢ - ŷᵢ)² and SS_tot = Σ(yᵢ - ȳ)²
### 3. MSE (Mean Squared Error)  
**Formula:** MSE = Σ(ŷᵢ - yᵢ)² / n

**Legend:**
- ŷᵢ: Predicted values
- yᵢ: Actual values
- ȳ: Mean of actual values
- n: Number of observations
- SS_res: Sum of squares of residuals
- SS_tot: Total sum of squares

## Submission Format
Submission has to be a CSV file. The file name must be **{team_ID}_{track_ID}.csv** 
The submitted file cannot be edited after 6:00 A.M. on 28th Sept. 2025.