# 📈 Stock Price Prediction Using LSTM

This project implements a Long Short-Term Memory (LSTM) neural network to predict future stock prices using historical market data. It features complete exploratory data analysis (EDA), model training, evaluation, and future price forecasting.

---

## 🎯 Project Objectives

- Visualize and understand stock trends and trading behavior  
- Train an LSTM model using past stock data  
- Predict the next closing price  
- Forecast multiple future business days  
- Evaluate prediction accuracy using standard regression metrics

---

## 🗃️ Data Source

- 📦 Live data from [Yahoo Finance](https://finance.yahoo.com/)
- Downloaded using the `yfinance` Python package
- User can specify:
  - ✅ Any stock symbol (e.g., AAPL, GOOG, TSLA)
  - ✅ Any date range
- Features used:
  - `Open`
  - `High`
  - `Low`
  - `Close`
  - `Volume`

---

## 📊 Exploratory Data Analysis (EDA)

The notebook includes various plots and statistics for understanding the dataset:

- **Closing Price Trend** – Line plot of stock closing prices over time
- **Volume Trend** – Shows trading volume changes
- **Year-over-Year Returns** – Visualizes annual return percentages
- **Daily Return Distribution** – Histogram of daily percentage changes
- **Descriptive Statistics** – Summary of numerical columns (mean, std, etc.)

---

## 🧠 LSTM Model Architecture

- Uses `TensorFlow` and `Keras` APIs
- Trained on sequences of historical OHLCV data
- Input: Past N days (default: 60)
- Output: Next day’s closing price
- Layers:
  - 2 stacked `LSTM` layers (50 units each)
  - Dropout layers (optional)
  - 1 Dense layer for output
- Loss function: `Mean Squared Error`
- Optimizer: `Adam`

---

## 📈 Evaluation Metrics

The model is evaluated on test data using:

| Metric | Description |
|--------|-------------|
| MSE    | Mean Squared Error |
| RMSE   | Root Mean Squared Error |
| MAE    | Mean Absolute Error |
| R²     | Coefficient of Determination |

All metrics are printed in the notebook after testing.

---

## 🔮 Future Price Forecasting

- User can define how many future days to forecast (e.g., 10, 30, 50+)
- Rolling window approach: prediction is fed back into the model
- Inverse transformed predictions are plotted and printed date-wise


---
## 📬 Author

Made with ❤️ by **Rahul Goyal**  
🔗 GitHub: [@RAHULGOYAL9000](https://github.com/RAHULGOYAL9000)

