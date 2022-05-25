# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to use a logistic regression model to compare two versions of a dataset. The data being analyzed is of historical lending activities from a peer-to-peer lending service company. The ultimate goal is to determine the creditworthiness of borrowers using the given dataset. Some of the variables that were used in the regression modeling include 'y' for the 'loan status' and 'X' for features. Other variables that were used include those for training data ('X_train' and 'y_train') and those for testing data ('X_test' and 'y_test'). The different stages of the machine learning process include creating a logistic regression model with the original dataset. The data is then fit to the model followed by a testing of the model. This test is what generates a prediction. Thereafter, given the small number of high-risk loans (label=1), the training data was resampled to address the data imbalance and then run through another LogisticRegression model. This data, as was the case for Model 1, was fit to the model and then re-tested. The test generates predictions which are then compared to the predictions/analytics of Model 1.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Accuracy = 0.9520479254722232
  * Precision = 0.85
  * Recall scores = 0.91



* Machine Learning Model 2:
  * Accuracy = 0.9936781215845847
  * Precision = 0.84
  * Recall scores = 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

In terms of performance, Model 1 seems to perform the best since it has a precision score of 0.85. However, Model 2 has a precision of 0.84 which is marginally less than that of Model 1. Thus, for all intents and purposes, both models perform similarly. However, the more important metrics are Accuracy and Recall Scores. For that reason, Model 2 is the better model overall. It has higher accuracy and recall scores which demonstrate that the Model 2 was correct more often than Model 1.
