# Credit Risk Analysis

## Objective
* The objective of this project is to analyze the different types of machine learning tools to determine the credit risk of the applicants and provide a decision as to high risk or low risk.
* There are six different algorithms utilized: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.
* Each of these are explained and a final recommendation is provided. 

## Results Summary
* This table provides a quick overview of the accuracy results of each of the algorithms.

| Model                          | Balanced Accuracy Score   | F1 Score   | Imbalanced Accuracy Score   | Type                | 
| -----------                    | -------------------       | --------   | -------------------         | ---------------     | 
| RandomOverSampler              | 0.6441747                 | 0.80       | 0.42                        | Over Sampling       |
| SMOTE                          | 0.6482720                 | 0.78       | 0.42                        | Over Sampling       |  
| ClusterCentroids               | 0.6482720                 | 0.60       | 0.25                        | Under Sampling      |
| SMOTEENN                       | 0.5103601                 | 0.70       | 0.38                        | Over/Under Sampling |
| BalancedRandomForestClassifier | 0.7877673                 | 0.95       | 0.62                        | Ensemble Learners   |
| EasyEnsembleClassifier         | 0.9254274                 | 0.97       | 0.86                        | Ensemble Learners   |

* From the list above, it is clear to see that the Easy Ensemble Classifier has the highest Accuracy and F1 scores.

* The F1 Score is highlighted here because it is the harmonic mean of the imbalanced data. It takes into consideration the Precision (TP/[TP+FP]) and Sensitivity (TP/[TP+FN]) and provides a summary statistic for evaluation. 

* A total of 68,470 Low Risk and 347 High Risk data points were utilized in this analysis (total 68,817). These were broken into X and y training and testing groups. The percentage breakdown is the same for all models (75/25 split). 

### RandomOverSampler

* The RandomOverSampler (ROS) utilized the process of correcting the imbalance by adding additional data points to the smaller (minority) class. This is done by randomly duplicating points already in the minority class.

* The Confusion Matrix and Classification Report are show below for your review.

![Confusion Matrix ROS](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/ROSconfusionMatrix.png)
![Classification Report ROS](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/ROSclassReport.png)


### SMOTE
he synthetic minority oversampling technique (SMOTE) is another oversampling approach to deal with unbalanced datasets. In SMOTE, like random oversampling, the size of the minority is increased. The key difference between the two lies in how the minority class is increased in size. As we have seen, in random oversampling, instances from the minority class are randomly selected and added to the minority class. In SMOTE, by contrast, new instances are interpolated





