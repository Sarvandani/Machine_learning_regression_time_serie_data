# Machine_learning_regression_time_serie_data

# Stock Price Prediction Using LSTM with Technical Indicators

This project demonstrates how to predict stock prices using a Long Short-Term Memory (LSTM) neural network model enhanced with popular technical indicators. It downloads historical stock data, computes technical features, trains an LSTM model, and visualizes both test and future predictions.

---

## Features

- **Data Acquisition:** Automatically downloads historical stock data using the `yfinance` library.
- **Technical Indicators:** Calculates key indicators using the `ta` library, including:
  - Relative Strength Index (RSI)
  - Moving Averages (MA50, MA200)
  - Bollinger Bands (Upper and Lower Bands)
- **Data Preprocessing:** Scales features using `MinMaxScaler` for improved model training.
- **Model Architecture:** Implements a stacked LSTM model with dropout layers to avoid overfitting.
- **Prediction:**
  - Predicts stock prices on a held-out test set.
  - Generates future stock price predictions for the next 20 trading days.
- **Visualization:** Plots actual vs predicted stock prices and future predictions with `matplotlib`.

---

## Requirements

- Python 3.7+
- Libraries:
  - `yfinance`
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `tensorflow` (or `tensorflow-gpu`)
  - `ta`

You can install dependencies using pip:

```bash
pip install yfinance pandas numpy matplotlib scikit-learn tensorflow ta
