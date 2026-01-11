# Multi-Company Stock Price Prediction

📈 This repository contains a **machine learning and deep learning model** for predicting stock prices of multiple companies. It supports **multiple algorithms (Linear Regression, Random Forest, SVR)** with **stacking ensemble** and optional **LSTM** for better prediction accuracy. The model is designed to work with **OHLCV data** for any company.

---

## Features

- Predict stock closing prices for multiple companies
- Uses historical OHLCV data + lag features
- Multi-algorithm ensemble:
  - Linear Regression
  - Random Forest
  - Support Vector Regressor
  - Stacking for improved accuracy
- Optional LSTM model for time-series prediction
- Fully scalable to new data
- Streamlit app for web-based predictions

---

## Data

- Input data format (CSV / DataFrame) should be **long format** (tidy data):

| Date       | Company | Open  | High  | Low   | Close | Volume |
|----------- |--------|-------|-------|-------|-------|--------|
| 2023-01-01 | AAPL   | 150   | 152   | 148   | 151   | 5000000 |
| 2023-01-01 | MSFT   | 300   | 305   | 298   | 303   | 4000000 |

- Lag features (`Close_lag_1`, `Close_lag_2`, …) are required for predictions.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/stock-prediction.git
cd stock-prediction
