# Time Series Analysis and Forecasting Project

A comprehensive time series analysis project implementing and comparing three different forecasting approaches: Seasonal ARIMA, Time-Series Regression, and Dynamic Linear Models (DLM). The project analyses 10 years of monthly sales data (2011-2020) to predict future sales trends.

## Project Overview
- Applied statistical analysis of time series data using R
- Implementation of multiple forecasting methodologies
- Comparative analysis of model performance
- Theoretical exploration of ARIMA models and seasonal effects

## Key Features
- Data preprocessing and exploratory analysis
- Model implementations:
  - Seasonal ARIMA modelling
  - Time-Series Regression with ARMA errors
  - Dynamic Linear Models
- Model diagnostics and validation
- Forecast generation and evaluation
- Theoretical proofs and mathematical foundations

## Repository Contents
- Project requirement with theoretical questions
- Raw data
- Project report with detailed methodology and findings
- R code for data analysis and visualisation
- Presentation slides
- Presentation video


## Technical Stack
### Core Technologies
- R Statistical Software (Version 4.x+)

### Key R Libraries
- `tseries`: For time series analysis and augmented Dickey-Fuller testing
- `forecast`: Implementation of ARIMA models and forecasting functions
- `dlm`: For Dynamic Linear Model implementation
- `knitr`: For table generation and report formatting
- `stats`: For linear regression and statistical testing
- `ggplot2`: For advanced data visualization
- `stlplus`: For seasonal decomposition of time series

### Statistical Methods & Techniques
- Time Series Decomposition
  - STL (Seasonal-Trend decomposition using LOESS)
  - Seasonal differencing
  - First-order differencing
- Diagnostic Testing
  - Augmented Dickey-Fuller test for stationarity
  - Box-Ljung test for residual autocorrelation
  - ACF and PACF analysis
- Model Selection Criteria
  - AIC (Akaike Information Criterion)
  - BIC (Bayesian Information Criterion)

## Results & Findings
### Model Performance Comparison
- Seasonal ARIMA: 
  - Best performing model (AIC: 739.4804, BIC: 750.1718)
  - Optimal configuration: ARIMA(0,1,1)(1,1,1)[12]
  - Strong performance in capturing both seasonal and trend components

- Time-Series Regression: 
  - Higher complexity scores (AIC: 830.7802, BIC: 875.3801)
  - Incorporated ARMA(1,1) residual modeling
  - Good for long-term trend capture

- Dynamic Linear Model:
  - Moderate performance (AIC: 783.6795, BIC: 797.6169)
  - Effective at handling evolving dynamics
  - Strong adaptive capabilities

### Key Insights
- Model diagnostics confirmed the presence of significant seasonal patterns
- First and seasonal differencing were necessary for achieving stationarity
- Successful convergence achieved in DLM parameter optimization
- All models showed consistent forecasting patterns, with Seasonal ARIMA providing the most efficient balance between complexity and accuracy
- Forecast reliability validated through out-of-sample testing on the final year of data

### Practical Applications
- Generated 6-month ahead forecasts (January to June 2021)
- Provided 95% prediction intervals for forecast uncertainty
- Demonstrated model robustness through multiple diagnostic checks
