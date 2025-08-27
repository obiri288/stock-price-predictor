# Stock Price Predictor (Time Series Forecasting)

This project is an introduction to time series forecasting using a simple linear regression model. The goal is to predict the next day's closing price of a stock (Apple, AAPL) based on its historical data.

**Disclaimer:** This model is for educational purposes only and should not be used for actual financial trading.

## 🚀 Methodology
1.  **Data Acquisition**: Historical stock data for AAPL was downloaded using the `yfinance` library.
2.  **Feature Engineering**: To predict the price at time `t`, the following features were created from past data:
    * Lag features (price at `t-1`, `t-2`, `t-3`)
    * A 5-day moving average
3.  **Train-Test Split**: The data was split chronologically to simulate a real-world forecasting scenario (trained on data before 2024, tested on data from 2024 onwards).
4.  **Modeling**: A simple Linear Regression model from Scikit-learn was used as a baseline.

## 🛠️ Tools Used
* **yfinance** for downloading stock data.
* **Pandas** for data manipulation and feature engineering.
* **Scikit-learn** for the regression model.
* **Matplotlib** for visualization.
