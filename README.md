# SGD/USD Exchange Rate Forecasting — ARIMA Model

This is the time series analysis of the Singapore Dollar to US Dollar exchange rate
from 1995 to 2018, using ARIMA modelling to forecast future rates. ~5,978 daily exchange rate observations were analysed to identify trends,
achieve stationarity, and build a forecasting model. The final model
selected was ARIMA(0,1,22) based on AIC minimisation and Ljung-Box
diagnostic checks.

## Problem Statement
To build a model that will allow for reliable forecasting based on existing currency market dynamics.

## Key Findings
- The original data was non-stationary (ADF test p-value = 0.60)
- First-order differencing achieved stationarity
- ARIMA(0,1,22) produced the lowest AIC of -43,532.26
- Forecast output stabilises after h > 20 steps, likely due to overfitting
- Future improvements could explore Seasonal ARIMA or Exponential Smoothing

## Tools Used
Python — forecast, tseries, dplyr

## Data Source
Currency Exchange Rates - containing daily exchange rates for 51 currencies from 1995 to 2018
[Dataset Link](https://www.kaggle.com/datasets/thebasss/currency-exchange-rates?resource=download)
