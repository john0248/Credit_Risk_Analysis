# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:

Module 17 gives us the chance to combine our skills in data preparation, statistical reasoning and machine learning.  Our goal is to understand and build a model that will assist in predicting credit risk.  

Credit risk can be seen as an unbalanced classification problem.  In general, there are more good loans compared to risky loans.   We were asked to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.  

Our credit card credit dataset comes from LendingClub, a peer-to-peer lending services company.  We will first oversample the data using the RandomOverSampler and SMOTE algorithms and under sample the data using the ClusterCentroids algorithm. After the combinatorial approach of over- and undersampling, we will compare two new machine learning models to reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results:

Please find the bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models below.

RandomOverSampler Model
*	Accuracy Score is 67.4%
*	Precision High Risk Score is 1%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 74%
*	Recall Low Risk Score is 61%

SMOTE Model
*	Accuracy Score is 66.2%
*	Precision High Risk Score is 1%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 63%
*	Recall Low Risk Score is 69%

ClusterCentroids Model
*	Accuracy Score is 66.2%
*	Precision High Risk Score is 1%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 69%
*	Recall Low Risk Score is 40%

SMOTEENN Model
*	Accuracy Score is 54.4%
*	Precision High Risk Score is 1%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 73%
*	Recall Low Risk Score is 59%

BalancedRandomForestClassifier Model
*	Accuracy Score is 78.9%
*	Precision High Risk Score is 3%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 70%
*	Recall Low Risk Score is 87%

EasyEnsembleClassifier Model
*	Accuracy Score is 93.2%
*	Precision High Risk Score is 9%
*	Precision Low Risk Score is 100%
*	Recall High Risk Score is 92%
*	Recall Low Risk Score is 94%

## Summary:

In summary, the results of these machine learning models show that the Balanced Random Forest Classifier and Easy Ensemble Classifier models had the highest scores, at 78.9% and 93.2% respectively. The recall score is an import metric since the goal of our analysis is to find a model that can best detect when a loan is high risk. When we compare the recall scores, we find that the Easy Ensemble Classifier had the highest score at 92%. The model recommended at this point is the Easy Ensemble Classifier model due to its recall high risk score and its good performance overall.
