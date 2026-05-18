# Credit Card Customer Segmentation

This project applies unsupervised machine learning to segment credit card customers based on their spending and usage behavior. The goal is to identify meaningful customer groups that can help a company understand its users better and create more targeted marketing strategies.

## Project Overview

Credit card companies deal with many types of customers. Some customers use their cards frequently for purchases, some rely more on cash advances, and others barely use their cards at all.

In this assignment, K-Means clustering is used to group customers based on similar financial behavior. Since the dataset does not contain predefined customer labels, this is an unsupervised learning problem.

## Dataset

The dataset used is `CC_GENERAL.csv`, which contains customer-level credit card usage information.

Each row represents one credit card customer. The features describe different behaviors such as balance, purchases, cash advance usage, payments, credit limit, and tenure.

Dataset source: Kaggle Credit Card Dataset  
https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data

## Main Steps

1. Imported the required libraries for data analysis, visualization, preprocessing, clustering, and evaluation.

2. Loaded the dataset using Pandas.

3. Explored the dataset by checking:
   - First five rows
   - Dataset shape
   - Data types and null values
   - Summary statistics

4. Cleaned the data by:
   - Removing `CUST_ID` because it is only an identifier and does not represent customer behavior
   - Handling missing values in `MINIMUM_PAYMENTS` and `CREDIT_LIMIT` using mean imputation

5. Performed exploratory data analysis using:
   - Histograms
   - Correlation heatmap
   - Scatter plots

6. Scaled the features using `StandardScaler` because K-Means is distance-based and features with larger values can dominate the clustering process.

7. Tested different values of K using:
   - Elbow method
   - Silhouette score

8. Built the final K-Means model using `K = 4`.

9. Added the cluster labels back to the dataset.

10. Analyzed the clusters using mean feature values for each group.

11. Used PCA to reduce the data into two components and visualize the final clusters in 2D.

## Machine Learning Method Used

The main algorithm used in this project is:

**K-Means Clustering**

K-Means groups customers by minimizing the distance between each customer and the center of their assigned cluster. It is useful when we want to discover hidden groups in data without using target labels.

Reference:  
https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html

## Evaluation Methods

Two methods were used to help choose the number of clusters:

### Elbow Method

The elbow method compares inertia values for different K values. Inertia measures how close data points are to their assigned cluster centers. A good K value is usually found where the decrease in inertia starts to slow down.

### Silhouette Score

The silhouette score measures how well-separated the clusters are. A higher score usually means better separation between clusters.

Reference:  
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.silhouette_score.html

## Final Number of Clusters

The final model used:

```python
K = 4
