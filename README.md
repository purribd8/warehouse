# Warehouse Forecasting

This project is a time series forecasting tool designed to predict weekly warehouse item usage using historical consumption data. It leverages Facebook's Prophet library to model trends, seasonality, and future usage patterns for each unique item in a warehouse dataset.

🔍 Features
Forecasts weekly item usage for multiple inventory items

Automatically handles missing data and seasonal trends

Skips items with insufficient history (< 30 data points) for more reliable predictions

Outputs future forecasts with upper and lower confidence bounds

📊 Tech Stack
Python

pandas for data manipulation

Prophet for time series modeling

matplotlib (optional) for visualization

📁 Dataset
The model expects a CSV file (mock_warehouse_usage.csv) with the following columns:

date: Timestamp of usage

item_id: Unique identifier for each warehouse item

quantity_used: Amount of the item used on that date

🔮 Output
The script generates a forecast for each item, including:

yhat: Predicted usage

yhat_lower / yhat_upper: Confidence interval bounds

These predictions can be used for inventory planning, demand forecasting, or operational analytics.
