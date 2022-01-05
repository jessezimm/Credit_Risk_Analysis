# Credit Risk Analysis

# Overview 
The purpose of this analysis is to predict if an applicant with default on a loan. Applicants we believe to be high risk are separated from the majority of applicants who are low risk. We are concerned with high risk applicants, and therefore, the following conclusions will reflect that. 

# Results
## Accuracy Score
The accuracy score ranges from 0.51 to 0.93. The minimium accuracy score comes from the Cluster Centroids model while the maximum score comes from both the Balanced Random Forest Classifier and Easy Ensemble AdaBoost models. The latter models are much better at predicts high and low risk applicants than the other models.

## Precision
The precision for high risk applicants is extremely low for all models ranging from 0.01 to 0.05. The classification of high risk applicants is not reliable.

## Recall
The recall for high risk applicants ranges between 0.59 and 0.70 with the highest recall being for the SMOTEENN model. The higher the recall the better the model is at classifying all positive, in this case high risk, samples (applicants).

## F1 Score
The F1 score for high risk applicants ranges from 0.02 to 0.08 with the highest F1 score being for the Balanced Forest Random Classifier and Easy Ensemble AdaBoost Classifier models. The F1 score is the weighted average of precision and recall, and thus the higher the better.

## Support
For all models, the support highlights that low risk applicants heavily outnumber high risk applicants. 

# Models
## Naive Random Oversampling

Accuracy Score: 0.62

![image](https://user-images.githubusercontent.com/88340176/148154903-00c0b312-c4ea-4c89-b6e1-dd57d8b8fe72.png)


## SMOTE Oversampling

Accuracy Score: 0.65

![image](https://user-images.githubusercontent.com/88340176/148154984-f96af832-e2dc-46ec-8d37-d8d22c3c4766.png)

## Cluster Centroids  Undersampling

Accuracy Score: 0.51

![image](https://user-images.githubusercontent.com/88340176/148155018-1df35edf-57bb-47d9-8a2d-453c92f59728.png)

## SMOTEENN Combination (Over and Under) Sampling

Accuracy Score: 0.64

![image](https://user-images.githubusercontent.com/88340176/148155071-b90d6015-cdec-46b7-9453-719bc9790937.png)

## Balanced Random Forest Classifier

Accuracy Score: 0.93

![image](https://user-images.githubusercontent.com/88340176/148155197-28e14511-2cdf-4c38-8ff0-2c38fe68332d.png)

## Easy Ensemble AdaBoost Classifier

Accuracy Score: 0.93

![image](https://user-images.githubusercontent.com/88340176/148155271-cc0b337b-20b3-417d-843a-ce9eac6b6986.png)

# Summary 
With the limited number of high risk applicants and the results discussed above, all models struggle to classify high risk applicants. I would recomend the Easy Ensemble AdaBoost Classifier model because it has the highest accuracy and F1 scores of all the models. Additionally, after each model is trained, another model is trained by evaluating the errors of the first model. This process is easy to understand for new users of neural networks. 
