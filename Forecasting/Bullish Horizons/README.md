# Modelling Minds - VITMAS
# Bullish Horizons
# Track ID: FBH002T
**Dataset Link:** [Bullish Horizons Dataset](https://kaggle.com/datasets/f34b4815c62e18714dad96c0ccdf6426751bd5a821736bc2b3d0eb70454e23f8)
## Objective
Time series forecasting of stock prices to predict future stock values (both daily_high & daily_low) until November 5, 2024, using historical trading data with multiple price indicators and volume metrics.

## Dataset Description
This dataset contains historical stock trading data in CSV format with daily trading information including price movements and trading volumes. The task involves predicting future stock prices using time series forecasting techniques.

**Data Format:** CSV file containing historical stock trading data

**Columns (7 total):**
- **date**: The trading date
- **open**: Opening price of the stock
- **close**: Closing price of the stock  
- **high**: Highest price of the day
- **low**: Lowest price of the day
- **volume**: Total number of shares traded
- **adjclose**: Adjusted closing price

**Directory Structure:**
```
bullish horizons/
└──Bullish Horizons Train.csv
```

**Task Requirements:**
- Forecast stock prices until November 5, 2024
- Maintain the same time intervals as provided in the training CSV
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
