# Bike Share Demand & Weather Analytics

**Regression case study in R examining how weather conditions modify bike-share demand relationships**

## Executive Summary
This project analyzes bike-rental demand using weather condition, temperature, humidity, and windspeed. The strongest analytical feature is the use of **interaction terms** to test whether the relationship between weather variables and demand changes across weather situations.

The original repository called this project “forecasting.” The revised portfolio uses **demand analytics/modeling** because the coursework primarily demonstrates regression and logistic regression rather than a time-series forecasting design.

## Business Questions
- How does rental demand differ by weather condition?
- How is temperature associated with demand after controlling for humidity and windspeed?
- Does the temperature-demand relationship change under clear, cloudy, or wet conditions?
- How does interpretation change when demand is log-transformed?
- What weather conditions are associated with the odds of a very high-demand day?

## Methods Demonstrated
- Exploratory distribution analysis
- Categorical predictors
- Multiple linear regression
- Interaction effects
- Log transformation
- Prediction from fitted models
- Logistic regression
- Odds-ratio interpretation
- Translation of normalized temperature units into degrees Celsius

## Repository Structure
```text
bike-share-demand-analytics/
├── README.md
├── analysis/
│   └── bike_share_demand_analysis.Rmd
└── requirements_R.txt
```

## Data Note
The original coursework referenced a local `bikeshare.csv` file, but that dataset was not included in the uploaded repository. The cleaned notebook therefore expects the file at `data/bikeshare.csv`. Numerical results should be rerun before adding specific performance claims.

## Interview Talking Point
> I used regression to study bike-share demand as a function of weather, temperature, humidity, and windspeed. I then added interaction terms because I wanted to test whether the effect of temperature changes under different weather conditions. I also compared level and log-demand interpretations and used logistic regression to model the odds of a high-demand day. The project taught me that an interaction means the effect of one predictor depends on the level of another predictor.

## Limitations
This is explanatory/predictive regression work, not a time-series forecasting model. A true forecasting extension would incorporate temporal ordering, seasonality, trend, lagged demand, and time-based validation.
