# Stock-price-prediction

Project Overview

In this project, we focused on developing an LSTM model for forecasting financial time series data. The specific target for our predictions was the 'VWAP' (Volume Weighted Average Price), a key indicator in financial analysis, representing the average price a security is traded at, weighted by volume.

Data Preparation and Analysis

The dataset, representing a financial time series, underwent initial cleaning and preprocessing. This included handling missing values, setting the 'Date' column as the index, and calculating rolling means and standard deviations for various financial metrics (like 'High', 'Low', 'Volume', etc.) over different window sizes. These calculations were instrumental in enriching the dataset with additional features that potentially capture more complex trends in the data.

LSTM Model Development

Given the sequential nature of time series data and the intricate patterns often present in financial markets, we chose an LSTM model for this task. LSTMs are well-suited for time series forecasting due to their ability to capture long-term dependencies and learn from the order in the data.

The LSTM model was trained on the processed data, with 'VWAP' as the dependent variable and the engineered features as independent inputs. The data was first normalized to ensure efficient training of the LSTM network. The model comprised several layers, including LSTM layers and Dense layers, and was trained to minimize the mean squared error of its predictions.

Forecasting and Model Evaluation

After training, the model was used to forecast 'VWAP' values for the length of the test data. The model's performance was evaluated using several metrics, including Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE). These metrics provided a comprehensive view of the model's accuracy and error magnitude.

Results

The LSTM model demonstrated a promising performance, as indicated by the calculated error metrics. The MAPE, in particular, was around 3.25%, suggesting a relatively high accuracy of the model in percentage terms. This performance suggests that the LSTM model was effective in capturing the underlying trends and patterns in the financial time series data.

Conclusion

This project highlighted the effectiveness of LSTM models in handling complex time series data, especially in the domain of financial forecasting. The model's ability to incorporate a multitude of features and learn from the sequential nature of the data made it a powerful tool for predicting financial time series. Future work might include further tuning of the model, exploration of additional features, or comparisons with other forecasting methodologies.

