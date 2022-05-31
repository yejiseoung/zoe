---
title: "Credit Card Customers Churn Prediction"
date: 2019-12-23T20:56:42+06:00
type: portfolio
image: "images/projects/project-thumb-four_5.png"
category: ["Classification, Imbalanced, GBM, Model Deployment"]
project_images: ["images/projects/project-details-image-one.png", "images/projects/project-details-image-two.png"]
---

##### GO TO [GITHUB](https://github.com/zoeyejiseoung/CreditCard_Churn) 

##### Overview
`Customer Churn (customer attrition)` is the most challenging problem for businesses such as credit card and telecommunication companies. Using machine learning models to predict churn outcomes would help improve businesses and prevent companies from losing customers. 


In this project, I analyzed [credit card customers' dataset](https://www.kaggle.com/sakshigoyal7/credit-card-customers) and built machine learning (ML) models to predict those customers who would churn the service. 

`The roc-auc score of the final model is 0.993`. 


##### Machine Learning Model Pipeline
`Gradient Boosting model (GBM)` shows the best performance compared to 5 different algorithms including Logistic Regression, Support Vector Machine, KNeighbor, Random Forest (RF), AdaBoost (ADA).



##### Dealing with Imbalanced dataset and Tuned hyperparameters
Since the dataset is imbalanced (84% of Existing customers and 16% of attrited customers), I used `ADASYN` over-sampling method. 

Furthermore, using `Optuna` helped find the best hyper-parameters for 
GBM model. 

As a result, I got an improved GBM model showing 7% increased performance (0.993 roc-auc-score) compared to the baseline (0.916 roc-auc-score).


##### Deployment Model Production
I published GBM model API by using `Docker` and `Heroku`. 




