# Time-series
.
Project Overview
The goal of this project is to predict the future values of the USD to AUD exchange rate using statistical time series models, specifically ARIMA (AutoRegressive Integrated Moving Average) and Exponential Smoothing. The project includes key tasks such as:

Loading and visualizing exchange rate data.
Checking stationarity and performing differencing if necessary.
Building ARIMA and Exponential Smoothing models.
Comparing the performance of the models using forecasting metrics like Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
Plotting diagnostics, ACF/PACF plots, and forecast results.
Data Description
The dataset used in this project contains exchange rates of USD to AUD with a date index. The data is in CSV format, and the main column of interest is labeled Ex_rate (Exchange Rate).

Data Columns:
date: Date of the exchange rate.
Ex_rate: Exchange rate of USD to AUD.
Installation
To run this project, you need to install the following dependencies:

pandas
numpy
matplotlib
seaborn
statsmodels
nltk
sklearn
You can install the required libraries using pip:

bash
Copy code
pip install pandas numpy matplotlib seaborn statsmodels nltk sklearn
Workflow
Data Preprocessing:

Data is read from a CSV file and processed.
Missing values are handled using forward fill.
Time series plots, boxplots, and descriptive statistics are displayed to understand the data.
Stationarity Testing:

The Augmented Dickey-Fuller (ADF) test is used to check the stationarity of the exchange rate data.
If the data is not stationary, differencing is applied.
ARIMA Model:

The ARIMA model is applied to the time series data, and diagnostics are plotted.
A 30-day forecast is made using the ARIMA model.
Exponential Smoothing Model:

An Exponential Smoothing model with additive trend is used to fit the time series data.
A 30-day forecast is made using the Exponential Smoothing model.
Model Comparison:

The Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) for both models are calculated to evaluate performance.
Forecast Results
Both ARIMA and Exponential Smoothing models are used to forecast the next 30 days of exchange rates. The forecasted values are plotted alongside the actual data for comparison.

Metrics
Mean Absolute Error (MAE): Measures the average magnitude of the errors between forecasted and actual values.
Root Mean Squared Error (RMSE): Measures the square root of the average of the squared differences between forecasted and actual values.
Challenges
Stationarity Issues: The exchange rate data may not be stationary, requiring differencing or other techniques.
Model Overfitting: ARIMA models can overfit if not tuned properly, especially when selecting parameters.
Accuracy of Forecasting: While both models give forecasts, external factors like market conditions can impact accuracy.
Insights
ARIMA Model: ARIMA is well-suited for modeling time series data with trends, but may not perform well with seasonal data.
Exponential Smoothing Model: Suitable for short-term forecasting and can handle data with trends effectively.
Future Work
Experiment with other time series models such as SARIMA for seasonal data.
Use more advanced techniques like Prophet or deep learning-based models for forecasting.
Incorporate external variables (such as interest rates or political events) to improve forecasts.
Author
[Your Name]
License
This project is licensed under the MIT License.
