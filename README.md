# Credit Risk Analysis

## Objective
* The objective of this project is to analyze the different types of machine learning tools to determine the credit risk of the applicants and provide a decision as to high risk or low risk.
* There are six different algorithms utilized: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.
* Each of these are explained and a final recommendation is provided. 

## Results
* This table provides a quick overview of the accuracy results of each of the algorithms.

| Model                          | Balanced Accuracy Score   | F1 Score   | Type                | 
| -----------                    | -------------------       | --------   | ---------------     | 
| RandomOverSampler              | 0.6441747                 | 0.80       | Over Sampling       |
| SMOTE                          | 0.6482720                 | 0.78       | Over Sampling       |  
| ClusterCentroids               | 0.6482720                 | 0.60       | Under Sampling      |
| SMOTEENN                       | 0.5103601                 | 0.70       | Over/Under Sampling |
| BalancedRandomForestClassifier | 0.7877673                 | 0.95       | Ensemble Learners   |
| EasyEnsembleClassifier         | 0.9254274                 | 0.97       | Ensemble Learners   |

* From the list above, it is clear to see that the Easy Ensemble Classifier has the highest Accuracy and F1 scores.

* A total of 68470 Low Risk and 347 High Risk data points were utilized in this analysis (total 68,817). These were broken into X and y training and testing groups. The percentage breakdown is the same for all models (75/25 split). 

### RandomOverSampler



(((((((((((((((((((  WRITE A DESCRIPTON ABOUT THE ONE THAT HAS THE BEST ACCURACY. FOCUS ON GIVING DEFINITIONS AND SUPPORT WHY THE
RESULT IS SO MUCH BETTER THAN THE OTHERS.))))))))))))))))))))))))