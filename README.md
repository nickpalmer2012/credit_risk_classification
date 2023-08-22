# credit_risk_classification
Module 20 Challenge
## Overview of the Analysis



The purpose of this analysis was to determine if one machine learning model performed better than another model in predicting if a customer is likely to default on a loan.  The variables used to determine if a customer will default on a loan were loan size, interest rate, borrower's annual income, debt to income ratio, number of accounts, derogatory marks, and total debt.  We used the loan status column as label data for the machine learning models and we used the columns mentioned previously as feature data. These had a binary format, so a customer received a "1" if they defaulted on thier loan or "0" if their loan is in good standing. The machine learning models were developed by taking the feature and label data and applying the "train_test_split" method to create training and testing data. We then created a Logistic Regression dataset with a random state of "1" to then "train" the test label and features created in the previous step. We then made predictions based on the test data by using the .predict method to generate prediction data. That prediction data was then fed into  a confusion matrix where we determined how the model performed based on the classification report. One model was generated with only the original data and the other was created using an oversampling method to aid in training and then compared. 
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * I believe this model predicts healthy loan candidates very well based on the "1.00" presicion score for healthy loan candidates.
  * The prediction performance on this model is good for this problem as you do not want to incorrectly identify creditworthy customers. The model is a little more unreliable for predicting high risk customers based on the .85 precision score it received.
  * The preditions for healthy loan candidates performed well on thier precision, recall, and f1 scores with accuracy scores in the 92 to 99 percentile.



* Machine Learning Model 2:
  *  I believe this model with the oversampled data performed very similarly to the model where we evaluated the original data. Recall seems to perform better with this model with respect to the "1" outcome, so there are less false negatives in this model.
  *  I think the oversampled model performs better than the model with the original data for predicting loan candidates, but the difference is marginal.

## Summary

The model that seems to perform the best is model 2 with the oversampling. This is due to its higher accuracy scores and f1 scores compared to the first model. I think it is important for each classification to perform well in the models as you do not want to incorrectly deny someone a loan if they are credit-worthy and you also do not want to incorrectly identify a credit-unworthy customer and give them a loan.

