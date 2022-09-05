# Module-17-Challenge  Credit_Risk_Analysis
# Overview of Project #
The purpose of this Project is to create a supervised machine learning model that could accurately predict credit risk by using the credit card dataset from LendingClub, a peer-to-peer lending services company.Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.
Different techniques are used to train and evaluate models with unbalanced classes.

The analysis consisted of the following:
1. Resampling Models to Predict Credit Risk.
2. SMOTEENN Algorithm to Predict Credit Risk.
3. Ensemble Classifiers to Predict Credit Risk.

# Resources #
Software: Jupyter Notebook <br>
Libraries: numpy, pandas, matplotlib, scipy, scikit-learn,imbalanced-learn<br>
Data Sources: LoanStats_2019Q1.csv

# Results #
## Credit Risk Resampling Techniques ##
### Naive Random Oversampling ###
- Balanced Accuracy: 0.65%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 62%
- Recall Low Risk: 68% <br>

![Naive Random Oversampling](/Image/Naive_Random_Oversampling.png)

### SMOTE Oversampling ###
- Balanced Accuracy: 0.62%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 59%
- Recall Low Risk: 66% <br>

![SMOTE_Oversampling](/Image/SMOTE_Oversampling.png)

### Undersampling ###
- Balanced Accuracy: 0.65%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 68%
- Recall Low Risk: 62% <br>

![Undersampling](/Image/Undersampling.png)

### Combination (Over and Under) Sampling ###
- Balanced Accuracy: 0.65%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 68%
- Recall Low Risk: 62% <br>

![Combination (Over and Under) Sampling](/Image/Combination_(Over_and_Under)_Sampling.png)

## Ensemble Classifiers to Predict Credit Risk ##
### Balanced Random Forest Classifier ###
- Balanced Accuracy: 0.78.7%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 67%
- Recall Low Risk: 91% <br>

![Naive Random Oversampling](/Image/Balanced_Random_Forest_Classifier.png)

### Easy Ensemble AdaBoost Classifier ###
- Balanced Accuracy: 0.92.5%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 91%
- Recall Low Risk: 94% <br>

![Easy_Ensemble_AdaBoost_Classifier](/Image/Easy_Ensemble_AdaBoost_Classifier.png)

# Summary #
From our analysis, we were able to conclude that the following:
1. This analysis is trying to find the best model that can detect if a loan is high risk or not. Becasue of that, we need to find a model that lets the least amount of high risk loans pass through undetected.
2. When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model.
3. The Easy Ensemble AdaBoost Classifier is the best model for the Credit_Risk_Analysis with 93% Accuracy Score.
4. The most weakest model in predicting the credit card risk is undersampling method which shows the lowest f1 score.


