
# Credit Card Fraud Detection 

## Objective
The Credit Card Fraud Detection Problem includes modeling past credit card transactions with the knowledge of the ones that turned out to be fraud. 
This model is then used to identify whether a new transaction is fraudulent or not. 
Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications.

## Observations
* The data set is highly skewed, consisting of 492 frauds in a total of 284,807 observations. This resulted in only 0.172% fraud cases. This skewed set is justified by the low number of fraudulent transactions.
* The dataset consists of numerical values from the 28 'Principal Component Analysis (PCA)' transformed features, namely V1 to V28. Furthermore, there is no metadata about the original features provided, so pre-analysis or feature study could not be done.
* There is no missing value in the dataset.

## Description
Credit Card Fraud Detection is a typical example of classification. Since we have highly imbalaced data, accuracy is not a good metric. Therefore, Precision and Recall are the best metric to use.

We can detect fraud using two ways, supervised and unsupervised learning.
In supervied learning various alogrithm such as lightgbm, xgboost are used to form a baseline model.
Once the baseline is formed, neural network are trained to see if we can get better precision and recall than baseline.
In unsupervised learning first I have to transform the data using UMAP, which is a dimensionality reduction techniques.
After that unsupervised algorithms are applied such as Isolation Forest and DBSCAN.


This dataset is taken from kaggle, it can be found [here](https://www.kaggle.com/mlg-ulb/creditcardfraud)  

The notebook is also available on kaggle:
* https://www.kaggle.com/rajgandhi/credit-card-fraud-detection


## Methods Used
* Data Visualization
* Supervised Learning
* Unsupervised Learning
* Sampling

## Technologies
* Python
* Jupyter Notebook
