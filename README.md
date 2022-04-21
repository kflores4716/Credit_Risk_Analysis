# Credit_Risk_Analysis

## Overview

In this analysis, we created 6 machine learning models, each with a goal of predicting credit risk. We built our models using the `imbalanced-learn` and `scikit-learn` libraries in `Jupyter notebook`. Once our models were built, trained, and tested, we evaluated their performances to determine whether we should or should not recommend using them to predict credit risk.

## Results

Here are the results from all 6 of our machine learning models. The results will include each model's balanced accuracy score, a confusion matrix, and a classification report that will display their precision and recall scores.

#### Random Over Sampling

![Random Over Sampling](https://user-images.githubusercontent.com/94764735/164114325-655fd09f-a980-49e1-a097-d724aa970cb5.png)

- The Balanced Accuracy Score here is about 63.67%.
- The high_risk precision score is 1% with a recall score of 62%.
- The low_risk precision score is 100% with a recall score of 65%.

#### SMOTE

![SMOTE](https://user-images.githubusercontent.com/94764735/164114331-c9df1dcb-1b96-4f28-9c0d-8ac0bb116d5c.png)

- The Balanced Accuracy Score is about 64.54%.
- The high_risk precision score is 1% with a recall score of 63%.
- The low_risk precision score is 100% with a recall score of 66%.

#### Cluster Centroids

![Cluster Centroids](https://user-images.githubusercontent.com/94764735/164114342-f71219e8-195b-42a0-a872-3723ffeca943.png)

- The Balanced Accuracy Score is about 51.03%.
- The high_risk precision score is 1% with a recall score of 59%.
- The low_risk precision score is 100% with a recall score of 43%.

#### SMOTEENN

![SMOTEENN](https://user-images.githubusercontent.com/94764735/164114351-beb14a44-c149-4d1b-8e05-cac7e44b2279.png)

- The Balanced Accuracy Score is about 63.76%.
- The high_risk precision score is 1% with a recall score of 70%.
- The low_risk precision score is 100% with a recall score of 57%.

#### Balanced Random Forest Classifier

![Balanced Random Forest](https://user-images.githubusercontent.com/94764735/164114357-2dad562b-9753-4f03-887e-f378b9b61841.png)

- The Balanced Accuracy Score is about 78.78%.
- The high_risk precision score is 4% with a recall score of 67%.
- The low_risk precision score is 100% with a recall score of 91%.

#### Easy Ensemble Classifier

![Easy Ensemble Classifier](https://user-images.githubusercontent.com/94764735/164114370-15984df0-971f-460d-a96b-13f49851c607.png)

- The Balanced Accuracy Score is about 92.54%.
- The high_risk precision score is 7% with a recall score of 91%.
- The low_risk precision score is 100% with a recall score of 94%.


## Summary


All models in this analysis had a pretty large disparity between f1 scores when predicting high_risk versus low_risk borrowers. The high-risk f1 scores are much lower than the low-risk ones, meaning that there's a larger discrepancy between precision and recall for high-risk compared to low-risk. 

Looking at the precision and recall scores for each model, it is apparent that all models are lacking in precision when it comes to high_risk borrowers. The largest high-risk precision score is only 7%, while on the other hand, the low-risk precision scores for ALL models is at 100%. Although there is a whole lot of room for improvement when it comes to precision as a whole, it is better for a lending institution to predict low-risk borrowers with higher accuracy than high-risk borrowers. They do not want to be lending to high-risk borrowers thinking that they're low-risk. However, these models' inability to predict high-risk borrowers does mean that the lender would be losing out on additional lending opportunities that would be favorable to them. Even if they use the `Easy Ensemble Classifier` model that has the highest high-risk precision (7%), they would be losing out on the other 93% of these supposed "high-risk" borrowers who (in reality) are low-risk. That being said, this `Easy Ensemble Classifier` model does have a balanced accuracy score of about 93%. 

In conclusion, while it is unfortunate that we will lose out on some low-risk lending opportunities, we would still recommend that we use the `Easy Ensemble Classifier` model. It's accuracy score is over 10% higher than the next closest model (`Balanced Random Forest Classifier` at 79%), and you would be hard-pressed to find a model that can make predictions with 100% accuracy across the board. Of course, there is always room for improvement, so if there are other predictive models out there that are potentially more accurate, they should certainly be factored in to this analysis. 
