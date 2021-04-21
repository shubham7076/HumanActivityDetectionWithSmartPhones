# HumanActivityDetectionWithSmartPhones
CMPE 255 Data Mining Project

Team-8<br><br>
Subhash Polisetti 015286063<br>
Kanak Kshirsagar 015264106<br>
Shreshta Balmuri 015442960<br>
Priyanka Cornelius 015217254<br>
Shubham Singla 014807221<br>

# Human Activity Recognition

## Introduction

This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying from the smartphone dataset.
This dataset is collected from 30 persons (referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.

By using the sensors (Gyroscope and accelerometer) in a smartphone, they have captured '3-axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations.

We will try to implement some classical machine learning algorithms and observe our model performance using F-1 Scores of different algorithms.

## Problem Framework
Smartphone dataset with data points consisting each corresponding to one of the six activities.
Dataset is built from below 17 signals:
o	tBodyAcc-XYZ
o	tGravityAcc-XYZ
o	tBodyAccJerk-XYZ
o	tBodyGyro-XYZ
o	tBodyGyroJerk-XYZ
o	tBodyAccMag
o	tGravityAccMag
o	tBodyAccJerkMag
o	tBodyGyroMag
o	tBodyGyroJerkMag
o	fBodyAcc-XYZ
o	fBodyAccJerk-XYZ
o	fBodyGyro-XYZ
o	fBodyAccMag
o	fBodyAccJerkMag
o	fBodyGyroMag
o	fBodyGyroJerkMag

We can estimate some set of variables from the above signals. Ie. We will estimate the following properties on each and every signal that we recorded so far.
o	mean(): Mean value
o	std(): Standard deviation
o	mad(): Median absolute deviation
o	max(): Largest value in array
o	min(): Smallest value in array
o	sma(): Signal magnitude area
o	energy(): Energy measure. Sum of the squares divided by the number of values.
o	iqr(): Interquartile range
o	entropy(): Signal entropy
o	arCoeff(): Autoregression coefficients with Burg order equal to 4
o	correlation(): correlation coefficient between two signals
o	maxInds(): index of the frequency component with largest magnitude
o	meanFreq(): Weighted average of the frequency components to obtain a mean frequency
o	skewness(): skewness of the frequency domain signal
o	kurtosis(): kurtosis of the frequency domain signal

## Problem Statement

1.Performing Exploratory data analysis (EDA) differentiating the six activities into static and Dynamic Activities using visualization techniques.
2.Plotting Distribution plots for the Static and Dynamic activities using the Magnitude of the acceleration of the activities.
3.Dimensionality reduction required for the high dimensional dataset using t-distributed Stochastic Neighbor Embedding (t-SNE) for different perplexities each for a good number of iterations.
4.Trying to implement classical Linear SVC with GridSearch machine learning algorithm, to observe the model accuracy for performance and evaluating the confusion matrix.
5.Comparing seven classical ML classifiers by calculating the accuracy as F1-Score for each ML classifier.
6.Setting up a Stacking classifier using each of the previous classifiers as an estimator and evaluating the F-1 Score for training and test dataset.
7.Trying to reduce the number of features for important features from the dataset and then evaluating the accuracy for training and test dataset.
