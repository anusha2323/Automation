Automated Univariate Time-Series Forecasting System

Objective
The goal is to develop an automated system that applies multiple statistical and machine learning models to time-series datasets for multi-step forecasting. The system will then select and return the most accurate model's results. Designed for ease of use, this system caters to individuals regardless of their background (STEM or non-STEM), enabling anyone to perform time-series forecasting on their data. The system recommends the best-fit model for a given dataset, which users can then customize and fine-tune for improved performance.

Available Models

ARIMA (AutoRegressive Integrated Moving Average)
ARIMA is a generalization of the autoregressive moving average (ARMA) model. It is commonly used to model time series data for understanding trends or predicting future values. ARIMA is particularly useful for data showing non-stationarity in the mean, where differencing steps are applied to eliminate trends and make the data stationary.

Prophet
Prophet is an open-source forecasting tool developed by Facebook’s Core Data Science team. It is based on an additive model that fits non-linear trends with yearly, weekly, and daily seasonality, as well as holiday effects. It performs well with data that has strong seasonal patterns and multiple seasons of historical data. Prophet is robust to missing data and trend shifts, and it handles outliers effectively.

HWES (Holt-Winters Exponential Smoothing)
HWES, or Triple Exponential Smoothing, forecasts future data points as an exponentially weighted average of past observations, factoring in trends and seasonality. This model applies exponential smoothing three times to capture the seasonal variations—either multiplicative or additive—of the data. It is most effective when the data exhibits multiple high-frequency signals that need to be addressed through smoothing.

Forecast Recommender

The system includes the auto_forecast class from the forecast_recommender module, designed to automatically select the most suitable forecasting model. Users can specify an evaluation metric to assess the performance of the selected models.

Parameters:

evaluate_metric: An integer (1 to 8) representing the evaluation metric to be used.

Available Evaluation Metrics:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Percentage Error (MAPE)

Symmetric Mean Absolute Percentage Error (SMAPE)

Mean Forecast Error (MFE)

Normalized Mean Squared Error (NMSE)

Theil's U Statistic

This system offers a straightforward approach to time-series forecasting, providing results with minimal user input and the ability to further optimize the model for better accuracy.
