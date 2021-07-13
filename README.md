# BlueBike Daily Ridership Forecast
> "By failing to prepare, you are preparing to fail" 
> by Benjamin Franklin

In every business, planning holds an important key to their success. We can gauge the maturity of the management in the company based on how they plan for the business and if the company achieved according to the plan. For every important planning, it's necessary to have a good forecast to allocate resources, and to anticipate problems that may arise. 

**Objectives** In this project, we are exploring forecasting through different  algorithms: traditional algorithms (such as Moving Average, Simple Exponential Smoothing, Holt's Method, Winter Holt's Method) & Machine Learning (Seasonal Arima, univariate and multivariate). 

**Data** We took real-data from Blue Bikes company in Boston https://www.bluebikes.com/system-data and our objective is to predict the daily forecast with window of 1 month and assess the performance of each algorithm.

### Result

The best performant model is Seasonal ARIMA with AR order of 0, MA order of 1 and seasonality of 12 months, with MAD of 55215.6 and MAPE of 53.1%. Considering that this is a univariate model (based on the historical data only), the model is performing well.

In the daily ridership (section 4), multivariate Seasonal ARIMA is performing better than normal Seasonal ARIMA improving 5.4% in terms of MAPE (from 56.3% to 50.9%). 

![Arima Univariate and multivariate.jpg](/f3_arima_univariate_multivariate.jpg)

### Conclusion

Univariate model of ARIMA able to perform well only by looking at the historical data, and able to decompose the historical data into Trend, Seasonal and Cyclical. With more data added, it can improve the performance of Model. This forecasting method will definitely help for the Blue-bike company to make better decision in their planning stage.

### Tools used on this notebook:
#### Time Series
- Moving Average
- Simple Exponential Smoothing
- Holt's Method
- Winter Holts' Method
- SARIMA
- SARIMA With Exogenous Variable

This is part of NUS Master in Business Analytics Project in DBA5106 Foundation in Business Analytics 2020.
