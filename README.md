# Time Series Forecasting with ARIMA


# Introduction

Autoregressive Integrated Moving Average (ARIMA) is a widely used and powerful statistical method for time series 
forecasting. It combines autoregression, differencing, and moving averages to capture the underlying patterns and 
trends in time series data. ARIMA models are particularly effective for stationary time series data, where statistical 
properties like mean and variance remain constant over time.

ARIMA is denoted as ARIMA (p, d, q), where:

p: The order of the autoregressive component.

d: The degree of differencing required to make the time series stationary.

q: The order of the moving average component.

## Problem Description: 

In the ever-evolving landscape of financial markets, the ability to accurately predict stock 
prices stands as a critical challenge with profound implications for investors, traders, and financial analysts. 
This problem involves developing a sophisticated predictive model that can unravel the intricate patterns and trends 
within historical stock price data, ultimately providing insightful forecasts for future price movements.


## Solution: 

To develop a reliable and accurate forecasting model using the Autoregressive Integrated Moving Average (ARIMA) 
methodology to predict future stock prices. The goal is to provide stakeholders, including investors, traders, and financial 
analysts, with a powerful tool to anticipate future stock prices, navigating the complexities of the dynamic market environment. 
This model holds critical importance for various stakeholders, investors, traders, and financial analysts who are operating 
financial domain of the highly dynamic and often unpredictable stock market.

## Algorithm:

ARIMA Algorithm Steps:

•	Understand the Data: Examine the time series data to identify any patterns, trends, or seasonality. 
  Check for missing values and outliers that might affect the analysis.
  
•	Stationaries the Time Series: ARIMA models work best when the time series data is stationary,
  meaning that it has a constant mean and variance over time. If the data is not stationary, perform
  differencing to remove trends or seasonality. You may need to apply differencing multiple times until
  the data becomes stationary.
  
•	Identify Parameters (p, d, q): 

p: The order of the autoregressive component.

d: The degree of differencing required to make the time series stationary.

q: The order of the moving average component.
  
•	Fit the ARIMA Model: Use the identified values of p, d, and q to fit the ARIMA model to the training data.

•	Model Diagnostics: Checking whether there are no patterns or trends.

•	Make Forecasts: Once the model is fitted and validated, use it to make forecasts on the test data.

•	Evaluate the Model: Compare the predicted values with the actual values from the test set.

•	Tune the Model: If the model performance is not satisfactory, consider adjusting the parameters (p, d, q) and re-fit the model.

•	Forecast Future Values: Forecast future values by specifying the number of periods you want to predict.


## Summary

To forecast Google stock prices, we first need to collect the data using the Yahoo Finance API. After verifying that the 
data is seasonal and not stationary through data visualization and seasonal decomposition, we will use the ARIMA model to 
understand its application. Next, we will transition to the SARIMA model, which is better suited for our seasonal data. 
The values of p, d, and q parameters necessary for both models will be determined by plotting the autocorrelation and 
partial autocorrelation of the data. Specifically, d will be set to 1 because our data is seasonal.

## Technologies

1. Yahoo Finance API: For collecting Google stock price data.
   
2. Python: Programming language for implementing the models.
 
3. Pandas: For data manipulation and analysis.
 
4. Matplotlib/Seaborn: For data visualization.
 
5. Statsmodels: For implementing ARIMA and SARIMA models.
    
6. Numpy: For numerical operations.

## Outputs

### 1. Checking whether the dataset is static or dynamic.
   
![ML-1](https://github.com/user-attachments/assets/fc521270-6b49-47e8-9fb4-381b7871e92a)

### 2. Autocorrelation analysis
   
![ML-2](https://github.com/user-attachments/assets/cad8c996-ab2e-463e-90f3-04b2cc4f0a3b)

### 3. Partial Autocorrelation analysis
   
![ML-3](https://github.com/user-attachments/assets/c033b3d2-767d-4209-82e8-9d5306e596fe)

### 4. Arima Model fitting

![ML-4](https://github.com/user-attachments/assets/117b1a73-91ef-4f46-9dad-eb0b1d33ccd4)

### 5. Sarima Model fitting
   
![ML-5](https://github.com/user-attachments/assets/e6e30582-c1a3-4ca3-a97d-db7696895f10)

### 6. Model Evaluation

![ML-6](https://github.com/user-attachments/assets/60af7320-5c0a-44eb-abf0-2f3541c4246b)


### 7. Model Comparison Visualization

![ML-7](https://github.com/user-attachments/assets/a249262a-1bfc-4121-b54e-caa4e65c4a16)

