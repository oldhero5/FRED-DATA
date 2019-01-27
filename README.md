# Executive Summary
We recommend that the Federal Reserve set a target interest rate of 1.47% for the upcoming year. This is based on examining economic indicators from the most recent business cycle that began on December 01, 2007. We believe that, ceteris paribus, this will keep inflation around 2.5%. Additionally our model projects that unemployment will rise towards the end of next year to approximately 3.82%. Reducing the federal funds borrowing rate to from the 2.25% target rate from this year will help combat this rising unemployment rate. 
    
### Background

Paul Volcker took office as Chairman of the Board of Governors of the Federal Reserve on August 06, 1979. He enacted new ideas that set the foundations for US monetary policy today. To that end when predicting an effective federal funds rate we used monthly data from August 1979 to the Present.

### Preparing Data and R Packages
We use the programming language R to import all required data using the "quantmod" package. This package pull directly from the FRED Database. This method allows us to use raw data to create plots and make interpretations from the data sets.

# Forecasting the Federal Funds Rate

We use a step-wise logistic regression to find the ten most significant predictors of a recession from the required data sets. We then forecast these ten variables for the next 12 months using an Auto-Regressive Integrated Moving Average (ARIMA) model. Using these forecasts, we predict the next 12 months' effective federal funds rate using a Dynamic Regression Model.

The Volcker Era the Step-wise model is accurate in predicting 98.85% of recessions. Using this as a baseline we recognize that these economic indicators are predictive of potential recessions. As such, we use the ten most important features use these indicators to forecast a recommended Federal Funds rate for the next 12 months. These features include GDP, Real Exports, Housing Starts, Consumer Price Index for All Urban Consumers: All Items Less Food and Energy, Average Hours Worked, Unemployment Rate, University of Michigan: Consumer Sentiment, The 1-Year Treasury Maturity Rate, Total Non-Farm Payrolls, and The 10-Year Treasury Maturity Rate.
