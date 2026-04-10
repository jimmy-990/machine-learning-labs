# Lab 6 - Linear Regression

This notebook applies Linear Regression to predict the yearly amount 
spent by e-commerce customers based on their app and website usage behavior.

## Dataset
- **File:** Ecommerce_Customers.csv
- **Rows:** 500 | **Columns:** 8

## What I did
I explored the dataset using pairplot and correlation heatmap which showed 
that Length of Membership and Time on App are the strongest predictors of 
yearly spending. I then trained a Linear Regression model and evaluated it 
using MAE, MSE, RMSE, and R2 Score.

## Results
The model achieved an R2 score of 0.989 meaning it explains 98.9% of the 
variance in yearly spending with an average error of only $9.

## Libraries
pandas, numpy, matplotlib, seaborn, scikit-learn
