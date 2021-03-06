# Creditcard-fraud-detection
 models trained to label anonymized credit card transactions as fraudulent or genuine. Dataset from Kaggle. 
In this project I build machine learning models to identify fraud in  credit card transactions. I also make several data visualizations to reveal patterns and structure in the data.

The dataset, hosted on Kaggle, includes credit card transactions made  by  cardholders. The data contains 7983 transactions that occurred over  of which 17 (0.21%) are fraudulent. Each transaction has 30 features, all of which are numerical. The features V1, V2, ..., V28 are the result of a PCA transformation. To protect confidentiality, background information on these features is not available. The Time feature contains the time elapsed since the first transaction, and the Amount feature contains the transaction amount. The response variable, Class, is 1 in the case of fraud, and 0 otherwise.
Project Introduction

 The approaches for the project are :

    Randomly split the dataset into train, validation, and test set.
    Do  feature engineering.
    Predict and evaluate with validation set.
    Train on  train set then predict and evaluate with validation set.
    Try other different models.
    Compare the difference between the predictions and choose the best model.
    Predict on test set to report final result.

Data Description

I was able to accurately identify fraudulent transactions using a LogisticRegression  model. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. Feature 'Class' is the target variable with value 1 in case of fraud and 0 otherwise.To improve a particular model, I optimized hyperparameters via a grid search with 3-fold cross-validation
