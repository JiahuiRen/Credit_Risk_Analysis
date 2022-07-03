## Credit_Risk_Analysis

# What You're Creating

This new assignment consists of three technical analysis deliverables and a written report. You will submit the following:
Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

# Overview of the analysis

Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

# Results

Naive Random Oversampling
<img width="760" alt="image" src="https://user-images.githubusercontent.com/6320035/177061391-3184e591-9fb4-437c-b66b-88ceca193be0.png">

SMOTE Oversampling
<img width="747" alt="image" src="https://user-images.githubusercontent.com/6320035/177061409-f04acbca-6538-4be7-9c28-4cb8b0079d64.png">

Undersampling
<img width="731" alt="image" src="https://user-images.githubusercontent.com/6320035/177061424-32f910d2-a685-4cab-a9ce-266f7a7cd423.png">

Combination (Over and Under) Sampling
<img width="745" alt="image" src="https://user-images.githubusercontent.com/6320035/177061439-dd2b2374-4ef8-438f-a05d-95b6206fa611.png">

# Summary
All the models used for credit risk analysis show weak accuracy in judging whether credit risk is high or not.  The integration model has greatly improved the sensitivity of high-risk credit in particular. Due to poor accuracy, many low-risk credit is still wrongly detected as high risk, which will punish the bank's credit strategy and infer its income by missing these business opportunities.  
For these reasons, I do not recommend that banks use any of these models to predict credit risk. 
