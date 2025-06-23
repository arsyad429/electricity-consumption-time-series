# 📈 Time Series Forecasting with Smoothing Methods

This project aims to forecast time series data using several popular smoothing methods, namely:

- Simple Exponential Smoothing (SES)
- Holt's Linear Trend Method
- Holt-Winters (Triple Exponential Smoothing)
- Seasonal Decomposition (Additive & Multiplicative)
- Stationarity Evaluation (ADF Test)
- Accuracy Evaluation using RMSE
## 📂 Dataset
The dataset used contains 157 rows of time series data with `Time` column as the time index and `Value` as the observed value. This data has been prepared in `.csv` format.
## 🔧 Metodologi

### 1. **Exploratory Data Analysis (EDA)**
- Historical trend visualization
- Outlier & extreme change detection

### 2. **Seasonal Decomposition**
Using `seasonal_decompose()` to separate:
- **Trend**
- **Seasonality**
- **Residual (Irregularity)**

### 3. **Exponential Smoothing Methods**
- **SES** is used for data without trends and seasonality.
- **Holt** for data with trends.
- **Holt-Winters** for data with trends and seasonality.

### 4. **Stasioneritas**
- Tested using **Augmented Dickey-Fuller Test (ADF)**
- Differentencing is performed if the data is not stationary
### 5. **Evaluasi**
- **Root Mean Squared Error (RMSE)** is used as a metric to assess the accuracy of forecasting results.

## 📊 Tools & Library
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `statsmodels`
- `scikit-learn` (for RMSE evaluation)

## 🧠 Main Results
- Holt-Winters gives the most stable and accurate results for this dataset because it is able to capture trends and seasonality.
- ADF Test shows that the data is not stationary, so transformation (eg differencing) is needed.
- RMSE shows that the average error is around ±4,000 from the original value, relatively small to the scale of the values.

## ✅ Conclusion
Smoothing methods are very useful in:
- Reducing data fluctuations (irregularities)
- Revealing trend and seasonal patterns
- Helping in building more stable and accurate predictive models
