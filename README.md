# Bank customer classification

## Main goal
Developing ML model predicting bank' customer inclination to open a deposit

### Tasks 
1) EDA;
2) Feature preprocessing;
3) Feature selection;
4) Data scaling;
5) Fitting Models (LogisticRegression, DecisionTree, RandomForrest); Hyperparameter optimization; Scores evaluation

## Data set feature description
### Customer details:
- age;
- job;
- marital (relationship status);
- education (level of education);
- default (has got an expired credit);
- housing (has got a housing loan);
- loan (has got a personal loan);
- balance.

### Features related to the last contact:
- contact (contact type with a customer);
- month (month of the last contact);
- day (day of the last contact);
- duration (contact duration, seconds).

### Other features:
- campaign (quantity of contacts with a client durint the current campaign);
- pdays (quantity of days missed since the last marketing campaign till the contact in the current campaign);
- previous (quantity of contacts till the current campaign)
- poutcome (the result of the previous campaign).

### Target:
- deposit. Defines if a customer agrees to open a credit in a bank.


## Summary
    * Following classifiers were tested and compaired during the investigation: LogisticRegression, DecisionTree, RandomForest, GradientBoosting, Stacking
    * DecisionTree, RandomForest, GradientBoosting models provided comparable scores after hyperparameters optimization  
    * The best scores obtained with StackingClassifier after threshold optimizing: f1-score=0.83, accuracy=0.83

## Tools used
pandas==2.0.1
numpy==1.23.5
matplotlib==3.6.3
optuna==3.3.0
seaborn==0.12.2
scikit-learn==1.3.0
