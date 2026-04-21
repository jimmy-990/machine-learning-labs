# Lab 8 - K Nearest Neighbors Project

This notebook applies the KNN algorithm to classify data points into 
two target classes using a scaled feature set.

## Dataset
- **File:** KNN_Project_Data.csv
- **Rows:** 1000 | **Columns:** 11

## What I did
I explored the dataset using a pairplot then standardized the features 
using StandardScaler. I trained a KNN model starting with K=1, then used 
the elbow method to find the optimal K value. Retraining with K=23 improved 
accuracy from 72% to 83%.

## Results
- K=1 accuracy: 72%
- K=23 accuracy: 83%

## Libraries
pandas, numpy, matplotlib, seaborn, scikit-learn
