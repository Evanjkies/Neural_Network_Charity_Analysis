# Neural_Network_Charity_Analysis

## Overview of the Analysis
The purpose of this analysis was to use machine learning and neural networks to create a binary classifier that is campable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
- The target variable was the "Is_Successful"
- There feature variables in the model were the "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT" columns
- The variables that were removed from the data were the "EIN" and "NAME" columns since these columns are just there to identify and seperate each indivisual claim.

### Compiling, Training, and Evaluating the Model
- In the original attempt there were two hidden layers with 80 neurons in the first layer and 30 in the second. These amounts were chosen because they felt proportional to the amount of variables in the input layer.
- I was able to improve my performance slightly but I was not able to achieve the target accuracy score of 75%
- In the first attempt to improve the original model's performance I dropped a couple extra columns that I thought could be negatively influencing the model. In the second attempt I tried to add another hidden layer where I left the number of neurons the same in the first two layers and scaled the third to have half as many neurons as the second layer. In the third attempt I kept the third layer but I increased the number of neurons per hidden layer.

## Summary
Accuracy scores
- Original Attempt = .727
- First Optimization Attempt = .726
- Second Optimization Attempt = .729
- Third Optimization Attempt = .730

### Recommendation
When training the model on the data, the model didn't improve in any meaningful way after a coupld epochs in any of the itterations. This leads me to believe that the model may have been overfit. SVMs are less prone to overfitting beacuse they are trying to maximize the distance, rather than encompass all data within a boundary.
