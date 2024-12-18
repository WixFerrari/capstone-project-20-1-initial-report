# Capstone Project
# Engine Systems Failure Time Predictor Final Report

## Problem Statement:
The goal of this project is to use a time series dataset to predict the failure time for engine systems, specifically turbofan engines.

## Importance of this topic:
This topic is important because unpredictable failures are a massive hinderance to electrical equipment industries. This model would allow companies to optimize repair schedules, increase equipment lifespan, reduce maintenance costs, and prevent unplanned downtime. If this question is unanswered, unpredictable failures will continue to cost companies money and will continue to pose as a serioues potential safety risk.

## Model Ouctomes or Predictions:
Regression classifiers were used to create the models in this project. The models were used to extrapolate the failure times and the failure times should match up to the original training set failure times. 

Supervised learning algorithms were used as the project involves predicting a specific target variable.

## Data Acquisition:
This dataset involves a set of sensored measurements that determine whether the engine was operational or not.

[https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/Links to an external site.](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/)

Turbofan Engine Degradation Simulation

## Data Preprocessing/Preparation:
The data was already predivided into training and test dataset. All that was needed to do was analyze the data by using feature importance to understand the significance of each individual feature. Also, to indentify patterns in the time series data to better understand the relationship between the input features and target variable.

## Modeling:
* Feature Importance
* KNearest Regression
* Time series analysis
* Gradient Boosting with Lag Features
* Random Forest Regressor
* Grid Search

## Model Evaluation:
For this project, regression and supervised learning were considered and implemented. By doing some research online and the information gained from this course, the models used were simply the most efficient and most accurate given the project's time frame.

## Results:
1) Using the Random Forest Regressor, the MSE was found to be 2245.452 and the R2 was around 0.052.
Predicted time for all units averaged around 200 test cycles.
Feature importance was used and found that core speed correct was the most important feature.
Grid search was also used and the MSE was around 2212.62 and the R2 was around 0.066, which is an improvement to the model.

2) Using the KNearest Regressor, MSE was calculated to be 1552.76 with a R2 of -0.0339.
Correlation is negative which means there is basically no correlation.

3) Gradient Boosting with lag features was used to calculate the MSE for each unit separately. For the 100 units, the MSE were all hovering around 1.00 which is a good sign.
Predicted failure time for each unit varies from 58 to 175 test cycles.

4) Random Forest Regressor produces the predicted failure time plot that is the most similar to the original training data failure time graph.
   
5) Gradient Boosting with lag features' predicted failure time plot has a similar pattern but the actual times are halved compared to the original training data.

## Next Steps:
* Improve the KNearest Regression and Random Forest Regressor so they calculate the MSE for each unit individually. 
* Find and use more models to see if better results can be had.
* Potentially use the test data to predict the training data failure time, and then compare the results.
* Instead of classifing using the failure time, classify using the features such as core speed, HPC temperature, etc., to see if these yeild better results.

## Recommendations:
Any help involving improving the current models or ideas on new models/ways to get better results would be appreciated.



