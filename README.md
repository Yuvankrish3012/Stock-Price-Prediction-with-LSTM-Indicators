# Stock-Price-Prediction-with-LSTM-Indicators

# Stock Price Trend Prediction with LSTM

This project uses a Long Short-Term Memory (LSTM) neural network to predict future stock prices for Apple Inc. (`AAPL`) using historical time-series data from Yahoo Finance. We enhance the prediction by integrating technical indicators like the Moving Average and RSI.

---

## Features

- LSTM-based deep learning model
- Moving Average (MA20) & RSI feature engineering
- Evaluation: MAE, RMSE, R² Score
- Visualization of actual vs predicted price
- Clean and modular code (Jupyter Notebook)

---

##  Dataset

- Downloaded using [`yfinance`](https://pypi.org/project/yfinance/)
- Stock: `AAPL` (Apple Inc.)
- Duration: Jan 2015 – Dec 2024
- Features used: `Close`, `MA20`, `RSI`

---

##  Model Architecture

- 2 LSTM layers (50 units each)
- 1 Dense output layer
- Input shape: `(60, 3)` for 60 timesteps, 3 features
- Optimizer: `adam`
- Loss: `mean_squared_error`

---

##  Results

| Metric     | Value   |
|------------|---------|
| MAE        | 5.38    |
| RMSE       | 7.06    |
| R² Score   | 0.9301  |

---

## 📈 Visualizations

- 📉 Actual vs Predicted Stock Price
  
 ![image](https://github.com/user-attachments/assets/ccd4c862-d67d-4b2a-8e89-add7bb6df8f4)
 
- 🟠 Close Price with Moving Average

  ![image](https://github.com/user-attachments/assets/50d07265-9d84-4a5b-aac0-8a30647d29d5)

- 📊 RSI (Relative Strength Index)

  ![image](https://github.com/user-attachments/assets/e69f045c-8f11-4688-8982-016bc3a9f97e)



---

## ▶️ How to Run

1. Install requirements:
   ```bash
   pip install yfinance pandas numpy scikit-learn matplotlib tensorflow
Run the notebook:

bash
Copy
Edit
jupyter notebook stock_price_lstm.ipynb
