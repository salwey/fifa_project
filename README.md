# Fifa 21 Project - Week2 Day 1 and 2 and then some....
Group Fifa Project

This project brings together cleaning and prepping data, implementing a linear regression model, x/y testing and cross validation.

It contains 3 models, the main, cheeky and test.

- The main is using many of the columns to create our model and can be tweaked to test different outcomes. R Score of around 0.9
- Cheeky model is creating a new column taking the max of the scores and using that as the only feature. R Score of around 0.97/0.98
- Cheat model was a test taking the target as the feature. R Score is as expected: 1, MSE is not exactly 0 due to rounding

It is a bit of a mess with extra code, commented out code and checks, opted to leave these in for now.


Question remains:
If we don't drop some of the rows with NaNs in but set them to a mean instead, most predictions are good but where we have those replacements the predictions in our test are fine but in our cross validation are out by many magnitudes and as such so is the R2 Score and MEA. Not sure why this is since we are still handling the NaNs and would only expect a slight change in R2/MEA values.
