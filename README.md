## Time-series
ARIMA

About
=====
In Time-series I explore the ability to predict future car counts in a parking lot using only past data. I can unfortunately not share the data but the notebook is made to show the common steps used in time-series analysis. 

Steps
=====
#### Problem definition
- What is it we want to know? 
#### Data Analysis/Cleaning
- Missing values?
- Does the data fall within reasonable ranges?
- Are there potential outliers? 
- Interpolate the missing values with mean or some other method. 
- Unusual data (outliers) flagged, are they unreasonable and should be removed? 
#### Stationary
- Visually inspect for recognizable patterns, such as trends, seasonal patterns or other cyclic components (data smoothing to see trends)
- Stationary time series are a lot easier to model. Eliminate trend and seasonal aspect of data. 
- One way to get rid of trend-fit a regression model. 
- Get rid of non-time stationary variance by a log transformation of the data.
#### Model selection
- Understand if the data is stationary meaning mean, variance, covariance does not change considerable with time. 
- Develop a model for the residuals, possibly using ARIMA. 
#### Model validation 
- Proper test such as RMS, ME, MAD, MSE. 
- Ideally forecast errors are gaussian white noise. Otherwise try to understand why they are not. 


Dependencies
------------

Time_series_predict is tested to work under Python 3

## Resources:
[Beginners guide to forecasting in Python](https://www.analyticsvidhya.com/blog/2016/02/time-series-forecasting-codes-python/)

 [Montgomery, D.C., C.L. Jennings and M. Kulahei (2015). *Time series analysis and forecasting 5th ed.*. Wiley](https://www.wiley.com/en-us/Time+Series+Analysis%3A+Forecasting+and+Control%2C+5th+Edition-p-9781118674918)
