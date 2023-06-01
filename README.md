## Overview of the Analysis

* The purpose of this analysis was to develop machine learning models to predict loan approval based on various financial features. The dataset provided included information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status (0 indicating not approved, 1 indicating approved). Loan status was the variable used to predict and train the model.
* The analysis involved two machine learning models:
  * Machine Learning Model 1: Logistic Regression Model trained on the original data.
  * Machine Learning Model 2: Logistic Regression Model trained on resampled training data
* The machine learning process followed these stages:
  * Data Preparation: The dataset was preprocessed, ensuring the data was in the appropriate format and handling any missing values or outliers.
  * Feature Selection: Relevant features were selected to train the models.
  * Model Training: Logistic Regression models were trained using the selected features and the original data in Model 1 and resampled training data in Model 2.
  * Model Evaluation: The trained models were evaluated using metrics such as balanced accuracy, precision, recall, and the confusion matrix.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.9520479254722232 this indicates a high level of overall accuracy in predicting both loan approval and rejection.
  * Precision : for not approved loans: 1.00, the Model 1 correctly predicts 100% of the loans that are not approved. And has a precision of 0.85 for predicting loan     approvals. This indicates that out of all the loan applications predicted as approved, approximately 85% are actually approved.
  * Recall: for not approved loans: 0.99, this means that it correctly identifies 99% of the loans that are not approved.
Recall for approved loans: 0.91. This indicates that out of all the actual loan approvals, approximately 91% are correctly identified by the model.

* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.9936781215845847, indicating a very high level of overall accuracy in predicting both loan approval and rejection.
  * Precision : for not approved loans: 1.00, the Model 2 correctly predicts 100% of the loans that are not approved.
Precision for class 1 (approved loans): 0.84, the Model 2 has a precision of 0.84 for predicting loan approvals. This means that out of all the loan applications predicted as approved, approximately 84% are actually approved.
  * Recall: for not approved loans: 0.99, this means that it correctly identifies 99% of the loans that are not approved.
Recall for approved loans: 0.99, this indicates that out of all the actual loan approvals, approximately 99% are correctly identified by the model.

## Summary

Comparing the results of the two machine learning models, we can see that Model 2 (trained on resampled training data) outperformed Model 1 (trained on the original data) in terms of balanced accuracy, precision, and recall. 
In Model 2, the balanced accuracy score improved significantly to 0.9937, indicating a high level of accuracy in predicting both loan approval and rejection. The precision for predicting class 1 (approved) improved from 0.85 to 0.84, and the recall increased from 0.91 to 0.99. This means that Model 2 is better at identifying true positives (actual loan approvals) while maintaining a high accuracy overall.
Considering the problem of predicting loan approval, it is crucial to have a high recall for class 1 (approved) loans to avoid rejecting potentially deserving loan applications. In this context, Model 2 performs better by achieving a higher recall score, making it the recommended model to use for predicting loan approval.

It is worth noting that the choice of the best model depends on the specific problem and the associated costs or consequences of false positives and false negatives. However, based on the provided results and the assumption that correctly approving loans is more important, Model 2 is the preferable option.
