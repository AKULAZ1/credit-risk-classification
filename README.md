# credit-risk-classification

## Overview of the Analysis

The objective of this analysis was to use historical data to train models to predict the creditworthiness of a lending services company's clients. The borrowers' income and number of accounts were compared against certain characteristics of their loans to determine the creditworthiness of each borrower. Two models were developed to identify the most accurate one- one with the original data and one with resampled data to balance the two classes and reduce the dominance of the healthy loan group. For further clarification, the original data resulted in two groups- 0 (healthy loan) with 75036 members and 1 (high-risk) with 2500; however, when resampled, both groups had 56,271. 

For each model, the data was split into training and testing sets. The former were used to fit to the LogisticRegression model and the latter were used to make predictions to later determine the accuracy of the models when acting as a parameter in elements that test machine learning model accuracy i.e. the balance_accuracy_score, the confusion matrix, and the classification report. These elements succintly revealed the accuracy of each model, and allowed me to clearly see any tangible improvements between the two model. 

## Results

* Machine Learning Model 1:
  * Accuracy: 0.972
  * Precision: 0- 1; 1- 0.87
  * Recall: 0- 1; 1- 0.95



* Machine Learning Model 2:
  * Accuracy: 0.994
  * Precision: 0- 1; 1- 0.87
  * Recall: 0- 1; 1- 0.99

## Summary

Although given the metrics mentioned above, the second model is slightly more accurate than the first; I believe the first model performs better when considering the risks of a lending services company. The second model had a significanlty high number of false positives, which poses a great risk that mistakenly approved borrowers might default on their loans and threaten the financial position of the company. That being said, the first model also returned a significant number of false positives and false negatives. Therefore, I do think, given more scope and time, the company ought to continue to train the model to acheive greater accuracy and reduce their risk.

## Sources
The code in cell 13 to fit the original data to the ROS model was sourced from machinelearningmastery.com, which can be found [here](https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/).
