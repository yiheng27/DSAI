# SC1015 (Data Science and Artificial Intelligence) Mini-Project

## About ##
This is a mini project for SC1015. We analysed a dataset on [Life Expectancy](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) after thinking about the aging population problem in Singapore.

## Contributors ##
Goh Yi Heng - Cleaning & Preparing Data, Correlation 
Anthony Soon - Linear Regression, Plotting of Train & Test Data
Benjamin Fernandez - New Machine Learning Technique

## Problem Definition ##
* How do different factors affect life expectancy?
* How can we explain Singapore’s aging population?

--------------------------------v-code-v------------------------------------------------------------
## Preparation of Dataset ##
We started by cleaning the dataset, by removing incomplete entries (NA and 0) and non-numerical rows. 

## Correlation Matrix ##
Then, we used correlation matrix to pick out the top 3 correlated factors to life expectancy.
After deciding on the 3 factors (Income Composition, Schooling, Adult Mortality) to use to study the relationship between them and Life Expectancy, the data was split into a 7:3 ratio for the train and test sets. 

## Linear Regression ##
The linear regression model learnt in this module is used on the train set first to derive the best suited constants for the linear equation. Then the equation is used on the test set to find the disparity between predicted and actual values of the test set. This is to determine the accuracy of the model used. 
To measure accuracy, the mean squared error(MSE) is calculated for both train and test sets for comparison. MSE is used as we wanted to put a greater weightage on larger errors.
These steps are repeated for the 3 factors to see which factor has the closest relationship to Life Expectancy with the least errors. Our findings show that “Income Composition” had the least amount of error, followed by ”Schooling” and lastly, “Adult Mortality”.

## New ML technique ##
This portion demonstrates the application of a new machine learning technique, specifically polynomial regression, to predict life expectancy based on factors such as adult mortality, schooling, and income composition of resources. The code iterates through polynomial degrees from 1 to 7 to find the best fitting model without overfitting. Overall, we found that polynomial regression with a degree of 3 was the best predictive model in predicting life expectancy in our test datasets.

Contents:
1. Introduction to Polynomial Regression
2. Sample code for applying Polynomial Regression
3. Model training and testing using Mean Squared Error (MSE)
4. Model evaluation and selection
5. Drawbacks of Polynomial Regression
6. Conclusion on factors affecting life expectancy

This portion helps us to improve on our predictive model and better understand the factors affecting life expectancy. We learn to apply polynomial regression for more accurate modeling while considering its drawbacks. The code provided in the repository displays the implementation of polynomial regression and how to select the best model out of the few.

## Conclusion ##

Overall, the factors that most greatly impact life expectancy are:

1. Income composition of resources
2. Quality of education
3. Adult Mortality

In Singapore, our income and quality of education has increased over the years and our adult mortality is low. 
This contributes to a longer life expectancy and explains an aging population.
For other countries that wish to boost its life expectancy, these are factors that they can focus on to do so.
