
# Time Series Forecasting with SARIMAX

This repository demonstrates a practical implementation of time series forecasting using the **SARIMAX** (Seasonal Auto-Regressive Integrated Moving Average with eXogenous regressors) model. The dataset contains monthly sales data, and the goal is to predict future sales by analyzing the historical data.

---

## Features
- **Time Series Analysis**: Explores trends and seasonality in the data.
- **Stationarity Testing**: Uses the Augmented Dickey-Fuller (ADF) test to assess whether the data is stationary.
- **Differencing**: Implements first-order and seasonal differencing to make the series stationary.
- **Auto-Regressive Modeling**: Plots autocorrelation and partial autocorrelation to identify optimal ARIMA parameters.
- **Forecasting**: Uses the SARIMAX model to predict future values with dynamic forecasting.
- **Visualization**: Plots historical data and forecasts to visualize trends and predictions.

---

## Prerequisites
### Libraries Used:
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`

Install the required libraries using:
```bash
pip install pandas numpy matplotlib statsmodels
```

---

## Dataset
The dataset used is a CSV file named `perrin-freres-monthly-champagne-.csv` containing monthly sales data. Ensure this file is in the same directory as the script or update the path accordingly.

**Columns in the dataset**:
1. `Month`: The month of the observation (e.g., "1964-01").
2. `Sales`: Sales data for the corresponding month.

---

## Key Steps in the Script

1. **Data Loading and Preprocessing**:
   - Renames columns for easier access.
   - Converts the `Month` column to datetime format and sets it as the index.

2. **Stationarity Testing**:
   - Performs the ADF test and applies differencing if needed.

3. **SARIMAX Modeling**:
   - Fits the SARIMAX model using determined parameters.
   - Predicts and visualizes future sales.

4. **Dynamic Forecasting**:
   - Extends the time series into the future for prediction.
   - Plots both the historical and future forecasts.

---

## Results
- **Forecast Visualization**: The script generates plots comparing actual sales and forecasted values, providing insights into expected trends.

---

## Contributions
Feel free to contribute to this repository by:
- Improving the model or adding alternative time series techniques.
- Enhancing visualizations or adding interactive plots.
- Extending the script to include other datasets or additional features.

---

## Acknowledgments
The dataset used for this project is sourced from a time series forecasting tutorial. Special thanks to the open-source community for providing tools and resources for data analysis and modeling. 
