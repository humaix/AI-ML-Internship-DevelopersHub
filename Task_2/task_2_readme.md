**📄 Task 2: Short-Term Stock Price Prediction (README)**

Predict Future Stock Prices (Short-Term)

**🎯 Objective**

To build a regression model that predicts the next day's closing price of a stock using historical market data.



**📂 Dataset**

Source: Yahoo Finance via the yfinance Python library.



Features: Open, High, Low, and Volume.



Target: Next day's Closing Price.



**🤖 Modeling Approach**

Preprocessing: Shifted the "Close" price column to create a target for the subsequent day.



Algorithm: Random Forest Regressor (chosen for its ability to handle non-linear stock market fluctuations).



Evaluation: Comparison of "Actual vs. Predicted" prices through time-series plotting.



**📈 Results**

The model successfully tracks the general movement of the stock.



The Mean Absolute Error (MAE) indicates how many dollars the prediction deviates from the actual price on average.

