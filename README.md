# Project Title

Parameter Optimization for ETS models

## Source

One of the forecasting methods is ETS model were E,T,S stand for Error, Trend, Seasonality respectively. First of all, decompose the given time series into its constituent elements/parts (Trend, Seasonality, Residuals). Depending on how trend and seasonality terms are (additive or multiplicative) select smoothing equations. 

**ETS models**

* Simple exponential smoothing
* Holt's Linear Trend method
* Exponential Trend method
* Holt Winter's Seasonality method

Each of the smoothing equations require a set of parameters to be passed depending on the method you choose. For selecting the best set of parameters, I have used **Basin Hopping** algorithm available in Scipy which minimizes the RMSE. The goodness of the fit is measured in MAPE (Mean Absolute Percent Error). For furthur understanding of working of ETS models read this [tutorial](https://grisha.org/blog/2016/01/29/triple-exponential-smoothing-forecasting)

## Prerequisites
```
numpy
pandas
matplotlib
scipy
```
