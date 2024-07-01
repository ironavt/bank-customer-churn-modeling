## Introduction

This research is carried out as part of an independent project on the topic "Supervised Learning." The goal of the project is to develop practical skills in using various machine learning models, tuning model hyperparameters, analysing model quality using metrics, and studying the impact of class imbalance on learning outcomes. The project uses data available at the following link: https://www.kaggle.com/datasets/barelydedicated/bank-customer-churn-modeling. This data is generated.

## Problem Statement

Clients have started leaving "Beta-Bank." Every month. Not many, but noticeably. Bank marketers have calculated that retaining existing customers is cheaper than attracting new ones. It is necessary to predict whether a client will leave the bank in the near future or not. You are provided with historical data on client behaviour and contract terminations with the bank. Build a model with the highest possible F1-score. To successfully complete the project, the metric needs to reach 0.59. Check the F1-score on the test sample independently. Additionally, measure AUC-ROC and compare its value with the F1-score.

## Actions Taken
* Exploratory Data Analysis (EDA) and filling in missing values
* * Identified class imbalance of the target variable
* Preparation of features for training
* Training decision tree and logistic regression models without considering class imbalance
* Addressing class imbalance of the target variable
* * Using the `class_weight` parameter
* * Using the upsampling method
* Training random forest, logistic regression, and decision tree models on balanced data
* Comparing metrics of the obtained models and selecting the best one

## Results Obtained
* The best value of the target metric was shown by the random forest model trained on upsampled data
* It was demonstrated that the AUC-ROC metric is less sensitive to class imbalance
* An increase in recall and F1-score was demonstrated after addressing class imbalance
* After upsampling, the decision tree model became prone to overfitting - a consequence of the increase in the number of identical data points