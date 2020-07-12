# FDI-Analysis
This repository is dedicated to the work done for the analysis of FDI in India using time-series statistical models.

## Objectives

- To perform an analysis on various sectors of the economy of a country.
- To forecast the future value of FDI for a individual sectors.

## Approach & Implementation

-  We have obtained a univariate time series dataset which has the data of FDIs of individual sectors of the economy from a government website.
-  We have performed an exploratory data analysis on top five sectors of the economy.
-  Exploratory data analysis has been done  on the dataset and analyzed the top 5 sectors before and after the government change in 2014.
-  Computer Software & Hardware sector has gone up in FDIs replacing Construction development sector since BJP has taken over.
-  Convert the time series model from non-stationary to stationary using differencing of series.
-  Perform a Augmented Dickey Fuller test and check the p-value and the test statistics value to confirm stationarity.
-  We obtain the optimum value of the orders of the ARIMA model by using a simple grid search over parameters.
-  The value of ‘p’ and ‘q’ which gives the lowest AIC and BIC value will correspond to the best order for the ARIMA model.
-  After obtaining the optimum order, we fit the data to the model on these parameters.

## MODEL DIAGNOSTICS

Model diagnostic plots of a good model should:
-  Have no obvious structures in the residuals in the Standardized residual plot.
-  The KDE and N(0,1) lines in the Histogram plus estimated density should almost be the same.
-  Have dots lying along the red line in the Q-Q plot.
-  95% of the correlations for lag greater than 0 should not be significant in the Correlogram.

## FORECASTING

- We tested our model on a particular sector.
- We obtained a forecast on the services sector by using our ARIMA(0,1,2) model for the Services Sector. 

## Conclusion

- The proposed model is able to predict future trends in FDIs in a given sector with a given confidence. Although a huge amount of data is required for higher accuracy and the model requires a thorough hyper-parameter tuning before being deployed.

## Future works and Drawbacks 

- In future ,we would like to be able to have access to more data and perhaps hope to collect monthly or even weekly data for each sector.
- Due to unavailability of country wise FDI data  we couldn’t show any separate results or any foreign country wise dependencies.   
pertaining to the same fact we couldn’t mention any other features related to FDI such as GDP fluctuation year-wise or  potential for growth of economy .
- Arima model fails to capture the seasonal aspects in the data.Using a SARIMA model would also help us capture the seasonal  trends, doing so will help the country prosper in a great way by optimizing resource allocation and preparing of the budgets for upcoming financial years in a smart way.
- We also have to experiment with models like LSTM using Deep Learning techniques but for that we'll have to find a good amount of data first.
