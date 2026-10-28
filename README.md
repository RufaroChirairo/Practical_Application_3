# Banking Model for Long Term Deposit Subscriptions 
Notebook: [link](https://github.com/RufaroChirairo/Practical_Application_3/blob/main/Practical_Assignment_3.ipynb)

## Business Problem
The business objective is to create a model that predicts whether a client will subscribe to a term deposit and identifies which characteristics influence the client's decision, in order to optimize the success of marketing campaigns. 

## Data Science Task
Since the output is binary task, this is a binary classification problem. 

## CRISP-DM Approach
The dataset contains information collected across 17 marketing campaigns, each using a different marketing technique. The objective is to improve campaign effectiveness by identifying clients who are more likely to subscribe to a term deposit while reducing unnecessary contacts.

Initial data exploration revealed no missing values, so no additional data cleaning was required. Data preprocessing involved one-hot encoding 10 categorical columns and scaling the 10 numerical columns. The dataset was then split, reserving 25% for model evaluation.

Four classification algorithms were implemented: Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree Classifier, and Support Vector Classifier (SVC). A baseline performance was established by dividing the yes observations in the target column by the total observations. Initial models were then trained to establish basic performance, followed by hyperparameter optimization using GridSearchCV with three-fold cross-validation and ROC-AUC scoring. ROC-AUC was selected to evaluate each model's ability to distinguish between clients who subscribed and those who did not across different classification thresholds

## Model Results
Basic Models:
Four classification models were evaluated before hyperparameter optimization. Logistic Regression achieved the highest test accuracy (91.51%), followed by SVC (91.37%). The Decision Tree achieved 100% training accuracy but only 89.04% test accuracy, suggesting overfitting.

Optimized Models:
GridSearchCV with three-fold cross-validation and ROC-AUC scoring was used to optimize model hyperparameters. Logistic Regression achieved the highest test ROC-AUC (94.23%), followed by SVC (93.94%), Decision Tree (93.36%), and KNN (91.17%

## Conclusion
Logistic Regression was the best-performing model, achieving the highest test ROC-AUC with relatively low training time. Further evaluation using precision, recall, and F1-score would help determine its effectiveness in identifying likely subscribers and reducing unnecessary marketing contacts# Practical_Application_3
