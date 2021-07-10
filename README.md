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
	* Confusion Matrix ROS
![Confusion Matrix ROS](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/ROSconfusionMatrix.png)

	* Classification Report ROS
![Classification Report ROS](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/ROSclassReport.png)

### SMOTE - Synthetic Minority Oversampling Technique
* SMOTE is another way to work with unbalanced data. It is similar to ROS because the minority group is increased. The difference between them is that SMOTE interpolates the data added to the minority class.
* The Confusion Matrix and Classification Report are show below for your review.
	* Confusion Matrix SMOTE
![Confusion Matrix SMOTE](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/SMOTEconfusionMatrix.png)

	* Classification Report SMOTE
![Classification Report SMOTE](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/SMOTEclassReport.png)

### Cluster Centroids
* Cluster Centroids is an under sampling method. Instead of adding data to the minority, it randomly reduces the majority data set to match the quantity of data points in the minority group.
* The Confusion Matrix and Classification Report are show below for your review.
	* Confusion Matrix Cluster Centroids
![Confusion Matrix Cluster Centroids](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/CCconfusionMatrix.png)

	* Classification Report Cluster Centroids
![Classification Report Cluster Centroids](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/CCclassReport.png)

### SMOTEENN - SMOTE and Edited Nearest Neighbors (ENN)
* SMOTEEN uses over and under sampling methods to analyze the data. SMOTE was described above. ENN removes outliers and helps to reduce the amount of overlapping data.
* The Confusion Matrix and Classification Report are show below for your review.
	* Confusion Matrix SMOTEENN
![Confusion Matrix SMOTEENN](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/SMOTEENNconfusionMatrix.png)

	* Classification Report SMOTEENN
![Classification Report SMOTEENN](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/SMOTEENNclassReport.png)

### Balanced Random Forest Classifier 
* The Balanced Random Forest Classifier utilizes [decision trees](https://towardsdatascience.com/decision-trees-in-machine-learning-641b9c4e8052) and balanced bootstrap samples.
* The combination of various methods is called an [ensemble](https://towardsdatascience.com/ensemble-methods-in-machine-learning-what-are-they-and-why-use-them-68ec3f9fef5f).
* The Confusion Matrix and Classification Report are show below for your review.
	* Confusion Matrix Balanced Random Forest Classifier
![Confusion Matrix Balanced Random Forest Classifier](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/FORESTconfusionMatrix.png)

	* Classification Report Balanced Random Forest Classifier
![Classification Report Balanced Random Forest Classifier](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/FORESTclassReport.png)


### Easy Ensemble AdaBoost Classifier 
* The [Easy Ensemble AdaBoost Classifier](http://restanalytics.com/2020-03-29-Machine-Learning-With-Imbalanced-Target-Class-Datasets/) utilizes [Adaptive Boosting](https://machinelearningmastery.com/boosting-and-adaboost-for-machine-learning/) which helps boost the accuracy of weak decision trees.
* The Confusion Matrix and Classification Report are show below for your review.
	* Confusion Matrix Easy Ensemble AdaBoost Classifier
![Confusion Matrix Easy Ensemble AdaBoost Classifier](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/EASYconfusionMatrix.png)

	* Classification Report Easy Ensemble AdaBoost Classifier
![Classification Report Easy Ensemble AdaBoost Classifier](https://github.com/summerstime/Credit_Risk_Analysis/blob/main/Images/EASYclassReport.png)

## Summary
* In summary, the Easy Ensemble AdaBoost Classifier shows much more accuracy in the determination of the credit risk of applicants.


