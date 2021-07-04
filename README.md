# Credit Risk Analysis

## Objective
* The objective of this project is to analyze the different types of machine learning tools. The goal is to teach the machine to determine the credit risk of the applicants and provide a decision as to high risk or low risk.
* There are six different algorithms utilized: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.
* Each of these are explained and a final recommendation is provided. 

## Results
* This table provides a quick overview of the accuracy results of each of the models.

| Model       | RandomOverSampler   | SMOTE           | ClusterCentroids   | SMOTEENN            | BalancedRandomForestClassifier | EasyEnsembleClassifier |
| ----------- | ------------------- | --------------- | ------------------ | ------------------- | ------------------------------ | ---------------------- |
| BAS[^1]        | 0.6441163           | 0.6482720       || 0.6482720          | 0.5159904           | 0.7877673                      | 0.9254274              |
| Type        | Over Sampling       | Over Sampling   | Under Sampling     | Over/Under Sampling | Ensemble Learners              | Ensemble Learners      |
[^1]BAS == Balanced Accuracy Score