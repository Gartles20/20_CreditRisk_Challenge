# Module 12 Report Template

## Overview of the Analysis

In this challenge I trained 4 different machine learning models to predict the danger of someone defaulting on their loan. I had information about loan size, interest rate, borrower income, debt to income ratio,num of accounts, derogatory marks, total debt, and loan status. After scaling the data using a standard scaler, I split the data into a train set with about 75% of the data and a test set with the remaining 25%. Then, I defined a helper function to simplify the process of training a model. This takes in the train and test set as well as a machine learning model and outputs the classification report, confusion matrix, and ROC Curve. 

## Results


* Logistic Model:
    * Accuracy 0.99, high precision and recall for safe loans but slightly lower for unsafe, 0.87 precision and 0.98 recall
* Nearest Neighbors Model:
    * Accuracy 0.99, high precision and recall for safe loans but slightly lower for unsafe, 0.86 precision and 0.99 recall
* Random Forest Model:
    * Accuracy 0.99, high precision and recall for safe loans but much lower for unsafe,   0.87 precision and 0.88 recall
* LightGB Model:
    * Accuracy 0.99, high precision and recall for safe loans but slightly lower for unsafe, 0.86 precision and 0.99 recall

## Summary

The best model for this data depends on the needs/goals of the user. If explainability is important then the best is the Logistic because it did almost as well as the best models but is very explainable. Otherwise, the LightGBM or Nearest Neighbor model would be best as they have a slightly lower risk of false negatives and do not compromise on accuracy. 
