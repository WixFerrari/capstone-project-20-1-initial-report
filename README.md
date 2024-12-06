# Turbofan Engine Failure Time Predictor

## Research Question:

How can time series data be used to predict the maintenance needs of electric equipment in order to reduce downtime and to prevent failures?

## Why this question is important:

This question is important because unpredictable failures are a massive hinderance to electrical equipment industries. This model would allow companies to optimize repair schedules, increase equipment lifespan, reduce maintenance costs, and prevent unplanned downtime. If this question is unanswered, unpredictable failures will continue to occur which costs a lot of money to fix, not to mention it is a potential safety risk.

## Data source(s):

https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/Links to an external site.

Turbofan Engine Degradation Simulation

## The techniques used in this analysis:
* Feature Importance
* KNearest Regression
* Time series analysis
* Gradient Boosting with Lag Features
* Random Forest Regressor
* Grid Search

## Results:
1) Using the Random Forest Regressor, the MSE was found to be 2245.452 and the R2 was around 0.052.
Predicted time for all units averaged around 200 test cycles.
Feature importance was used and found that core speed correct was the most important feature.
Grid search was also used and the MSE was around 2212.62 and the R2 was around 0.066, which is an improvement to the model.

2) Using the KNearest Regressor, MSE was calculated to be 1552.76 with a R2 of -0.0339.
Correlation is negative which means there is basically no correlation.

3) Gradient Boosting with lag features was used to calculate the MSE for each unit separately. For the 100 units, the MSE were all hovering around 1.00 which is a good sign.
Predicted failure time for each unit varies from 58 to 175 test cycles.

## Next Steps:
* Improve the KNearest Regression and Random Forest Regressor so they calculate the MSE for each unit individually. As of right now, it seems like they may be calculating over 20000 units which caused the MSE to be very high and the R2 to be very low.
* Compare the predicted failure time to the known training data failure time.
* Potentially use the test data to predict the training data failure time, and then compare the results.



