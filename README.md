# Credit_Risk_Analysis

## Overview

In this analysis, we created 6 machine learning models, each with a goal of predicting credit risk. We built our models using the `imbalanced-learn` and `scikit-learn` libraries in `Jupyter notebook`. Once our models were built, trained, and tested, we evaluated their performances to determine whether we should or should not recommend using them to predict credit risk.

## Results

Here are the results from all 6 of our machine learning models. The results will include each model's balanced accuracy score, a confusion matrix, and a classification report that will display their precision and recall scores.

#### Random Over Sampling

![Random Over Sampling](https://user-images.githubusercontent.com/94764735/164114325-655fd09f-a980-49e1-a097-d724aa970cb5.png)

- The Balanced Accuracy Score here is about 63.67%.
- The high_risk precision score is 1% with a recall score of 62%.

#### SMOTE

![SMOTE](https://user-images.githubusercontent.com/94764735/164114331-c9df1dcb-1b96-4f28-9c0d-8ac0bb116d5c.png)

- The Balanced Accuracy Score is about 64.54%.
- The high_risk precision score is 1% with a recall score of 63%.

#### Cluster Centroids

![Cluster Centroids](https://user-images.githubusercontent.com/94764735/164114342-f71219e8-195b-42a0-a872-3723ffeca943.png)

- The Balanced Accuracy Score is about 51.03%.
- The high_risk precision score is 1% with a recall score of 59%.

#### SMOTEENN

![SMOTEENN](https://user-images.githubusercontent.com/94764735/164114351-beb14a44-c149-4d1b-8e05-cac7e44b2279.png)

- The Balanced Accuracy Score is about 63.76%.
- The high_risk precision score is 1% with a recall score of 70%.

#### Balanced Random Forest Classifier

![Balanced Random Forest](https://user-images.githubusercontent.com/94764735/164114357-2dad562b-9753-4f03-887e-f378b9b61841.png)

- The Balanced Accuracy Score is about 78.78%.
- The high_risk precision score is 4% with a recall score of 67%.

#### Easy Ensemble Classifier

![Easy Ensemble Classifier](https://user-images.githubusercontent.com/94764735/164114370-15984df0-971f-460d-a96b-13f49851c607.png)

- The Balanced Accuracy Score is about 92.54%.
- The high_risk precision score is 7% with a recall score of 91%.
