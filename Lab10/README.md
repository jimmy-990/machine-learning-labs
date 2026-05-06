# Lab10 Support Vector Machines — Iris Dataset

## Overview
Classifying Iris flower species using **Support Vector Machine (SVM)** with hyperparameter tuning via **GridSearchCV**.

## Dataset
- Loaded via seaborn: `sns.load_dataset('iris')`
- **150 samples** · 4 features · 3 species
- Target: `species` — *setosa, versicolor, virginica*

## Results
| Model | Performance |
|---|---|
| Base SVC | High accuracy — Iris is well separable |
| GridSearchCV SVC | Tuned `C` & `gamma` for optimal results |

> **Setosa** is the most separable species — forms a perfectly distinct cluster in all feature pairs.

## Libraries
`pandas` · `numpy` · `matplotlib` · `seaborn` · `scikit-learn`
