### Submission

* Two Jupyter notebooks have been submitted titled "Main_time_series_analysis,ipynb" for the time series exercise and "Main_regression_analysis.ipynb" for the regression analyses exercise.

* "Main_README.md" summarizes the observations and findings and has been included for reference.

---

# Time-Series Forecasting

In this notebook, an analysis of historical CAD-JPY exchange rate data has been used to apply time series analysis and modelling to determine if there is any predictable behaviour.

The following are the observations based on the steps outlined in the time series starter notebook:

1. Plotting the Settle price to check for long or short-term patterns.
    - Based on the plot, over a long-term and medium basis basis, it is evident that the JPY has considerably strengthened compared to CAD. However, over a short term basis, the volatility is considerably high with no major observable trend.

2. Decomposition using a Hodrick-Prescott filter (decompose the settle price into trend and noise).
    - Over the long term, the price curve (in blue) and the trend line (in orange) superimpose each other, but the tend line highlights a declining trend over the 5.5 year period. 
    - Over the short term, the trend line discards the daily volatility (or noise). This could be an indication of an overvalued situation, where the price line is skewed higher than the trend line and imply a sell opportunity. Similarly, when the price line is lower than the trend line, it could imply a buy opportunity as the currency would be undervalued at that particular moment. 

3. Forecasting returns using an ARMA model.
    - For a model to be good fit, the p-value is required to be less than 0.05. Since the p-value in our example is 0.81, it can be concluded that the model is not a good fit.

4. Forecasting the exchange rate price using an ARIMA model.
    - The model predicts strengthening of JPY over the near term 

5. Forecasting volatility with GARCH.
    - Based on the forecast plot, the model forecasts a marginal increase in volatility in the near term

### Use the results of the completed time series analysis and modelling to answer the following questions:

1. Based on your time series analysis, would you buy the yen now?
    * Based on the time series analysis, the ARMA and the ARIMA models, both have a P-value > 0.05, indicating that the models are not very accurate predictors of the exchange rates. As such, I would not be very confident in relying on these models to arrive at a decision of buying yen now.


2. Is the risk of the yen expected to increase or decrease?
     * Despite the ARMA and ARIMA models not being significant predictors of the for CAD-JPY exchange rate trends, the GARCH model has a very low P-values (way lesser than 0.05) indicating that the model is a good predictor of volatility in the short term. As per the model's forecasts, the volatility in the exchange rate is expected to increase over the near future, indicating increased risk of the yen. 


3. Based on the model evaluation, would you feel confident in using these models for trading?
    * Since the ARMA and ARIMA models have high P-values, their significance as accurate predictors is very low. Additionally, the accuracy of the GARCH model (P < 0.05) indicating high volatility over the near term indicates high risks over the near term. Considering these two factors, I would not be confident using these models for trading.



# Linear Regression Forecasting

In this notebook, the Scikit-Learn linear regression model is used to predict CAD/JPY returns with *lagged* CAD/JPY futures returns and seasonal effects 


Using the results of the linear regression analysis and modelling the following observations were made:

* Does this model perform better or worse on out-of-sample data compared to in-sample data?
    - The model performed better on Out-of-Sample data compared to In-Sample, considering Out-of-Sample data had lower RMSE among the two datasets

- - -

