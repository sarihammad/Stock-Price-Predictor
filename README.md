# Stock Price Predictor

Inputs a stock and using machine learning and advanced time series analysis techniques predicts the future price of that stock based on historical data. The tool fetches historical stock data from Yahoo Finance, preprocesses the data, engineers features, and trains a neural network implemented with Keras to make predictions.

## Key Features

- **Data Retrieval:** Fetches historical stock data using the Yahoo Finance API.
- **Preprocessing:** Cleans and preprocesses the data, including the calculation of technical indicators such as SMA, EMA, MACD, and RSI.
- **Feature Engineering:** Creates additional features such as lagged prices, daily returns, and advanced time series analysis features.
- **Neural Network Model:** Utilizes a feedforward neural network implemented with Keras to predict future stock prices.
- **User Interaction:** Guides the user through inputting the stock ticker symbol, start and end dates, and provides predictions on future stock prices.
- **Logging:** Records important information and potential issues in a log file for reference.

## Instructions

1. Install dependencies:
   
```pip install -r requirements.txt```

2. Run the script:

```python stock_price_predictor.py```

3. Follow the prompts to input stock information and view the predicted stock price.

   
## Test Run

```console
Enter the start date (YYYY-MM-DD): 2021-01-01
Enter the end date (YYYY-MM-DD) or specify the number of days (e.g., +30): +365
[*********************100%%**********************]  1 of 1 completed
1/1 [==============================] - 0s 30ms/step
Mean Squared Error on Test Set: 190.5608208360235
1/1 [==============================] - 0s 6ms/step
Predicted Close Price for 2023-12-28: 182.92
The price is expected to move up by 3.01% from the last close.
```

**Note:** Currently programmed to only show the closing price for the next day.
