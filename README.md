# Advanced Regression - Surprise Housing - Price Prediction


A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

 

The company wants to know:

1. Which variables are significant in predicting the price of a house, and

1. How well those variables describe the price of a house.

 

Also, determine the optimal value of lambda for ridge and lasso regression.


## Business Goal
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Table of Contents
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)



## Conclusions
We have done EDA, data preparation, dummy variable creation, finding optimal alpha values using grid search and finally built models using the best alpha values (for both ridge and lasso methods).

We also answered a few subjective questions and did analysis based on those questions as well.

### Ridge Regression

The optimum alpha value for ridge regression is 7.0.

Here are the key predictors for the ridge regression

| Features              | Beta Coefficients  |
|-----------------------|--------------------|
| GrLivArea             | 0.139              |
| TotalBsmtSF           | 0.102              |
| OverallQual_Excellent | 0.088              |
| OverallQual_Very Good | 0.081              |
| 2ndFlrSF              | 0.075              |


Here is the error metrics for ridge

|           | Train | Test  |
|----------:|------:|-------|
| R-Squared | 0.948 | 0.899 |
|       RSS | 3.862 | 3.199 |
|       MSE | 0.004 | 0.007 |
|      RMSE | 0.062 | 0.085 |

### Lasso Regression

The optimum alpha value for lasso regression is 0.0005

Here are the key predictors for lasso regression

| Features              | Beta Coefficients |
|-----------------------|-------------------|
| GrLivArea             | 0.292             |
| OverallQual_Excellent | 0.133             |
| TotalBsmtSF           | 0.127             |
| Age                   | -0.100            |
| OverallQual_Very Good | 0.099             |



Here are the key error metrics for lasso


|           | Train | Test  |
|----------:|------:|-------|
| R-Squared | 0.938 | 0.897 |
|       RSS | 4.618 | 3.261 |
|       MSE | 0.005 | 0.007 |
|      RMSE | 0.067 | 0.086 |



## Technologies Used
- Pandas
- Matlibplot
- Python
- Seaborn
- StatsModel
- Scikit-learn
- Numpy
- Jupyter Lab


## Contact
Created by - [harish-babu](https://github.com/harish-babu)