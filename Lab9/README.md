# Lab9 Random Forest Project — LendingClub Loan Data

## Overview
Predicting whether a borrower will fully repay their loan using **Decision Tree** and **Random Forest** classifiers on LendingClub data *(2007–2010)*.

## Dataset
- **Rows:** 9,578 loans · 14 features
- **Target:** `not.fully.paid` — *0 = paid, 1 = defaulted*

## Results
| Model | Accuracy | Class 1 Recall |
|---|---|---|
| Decision Tree | 73% | 0.22 |
| Random Forest *(600 trees)* | 85% | 0.02 |

> Random Forest wins on accuracy, but both models struggle with class imbalance (~16% defaulted).

## Libraries
`pandas` · `numpy` · `matplotlib` · `seaborn` · `scikit-learn`
