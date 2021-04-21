# HumanActivityDetectionWithSmartPhones
CMPE 255 Data Mining Project<br>

Team-8<br><br>
Subhash Polisetti 015286063<br>
Kanak Kshirsagar 015264106<br>
Shreshta Balmuri 015442960<br>
Priyanka Cornelius 015217254<br>
Shubham Singla 014807221<br>

# Human Activity Recognition

## Introduction

This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying from the smartphone dataset.
This dataset is collected from 30 persons (referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.<br><br>

By using the sensors (Gyroscope and accelerometer) in a smartphone, they have captured '3-axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations.<br><br>

We will try to implement some classical machine learning algorithms and observe our model performance using F-1 Scores of different algorithms.<br><br>

## Problem Framework
Smartphone dataset with data points consisting each corresponding to one of the six activities.<br>
Dataset is built from below 17 signals:<br>
o	tBodyAcc-XYZ<br>
o	tGravityAcc-XYZ<br>
o	tBodyAccJerk-XYZ<br>
o	tBodyGyro-XYZ<br>
o	tBodyGyroJerk-XYZ<br>
o	tBodyAccMag<br>
o	tGravityAccMag<br>
o	tBodyAccJerkMag<br>
o	tBodyGyroMag<br>
o	tBodyGyroJerkMag<br>
o	fBodyAcc-XYZ<br>
o	fBodyAccJerk-XYZ<br>
o	fBodyGyro-XYZ<br>
o	fBodyAccMag<br>
o	fBodyAccJerkMag<br>
o	fBodyGyroMag<br>
o	fBodyGyroJerkMag<br>

We can estimate some set of variables from the above signals. Ie. We will estimate the following properties on each and every signal that we recorded so far.<br>
o	mean(): Mean value<br>
o	std(): Standard deviation<br>
o	mad(): Median absolute deviation<br>
o	max(): Largest value in array<br>
o	min(): Smallest value in array<br>
o	sma(): Signal magnitude area<br>
o	energy(): Energy measure. Sum of the squares divided by the number of values.<br>
o	iqr(): Interquartile range<br>
o	entropy(): Signal entropy<br>
o	arCoeff(): Autoregression coefficients with Burg order equal to 4<br>
o	correlation(): correlation coefficient between two signals<br>
o	maxInds(): index of the frequency component with largest magnitude<br>
o	meanFreq(): Weighted average of the frequency components to obtain a mean frequency<br>
o	skewness(): skewness of the frequency domain signal<br>
o	kurtosis(): kurtosis of the frequency domain signal<br>

## Problem Statement

1.Performing Exploratory data analysis (EDA) differentiating the six activities > Target Variables <br>
 1.1 Sitting <br>
 1.2 Walking <br>
 1.3.Walking_upstairs <br>
 1.4 Walking_downstairs <br>
 1.5 Lying <br>
 1.6 Standing <br>
 into static and Dynamic Activities using visualization techniques.<br>
3.Plotting Distribution plots for the Static and Dynamic activities using the Magnitude of the acceleration of the activities.<br>
4.Dimensionality reduction required for the high dimensional dataset using t-distributed Stochastic Neighbor Embedding (t-SNE) for different perplexities each for a good number of iterations.<br>
5.Trying to implement classical Linear SVC with GridSearch machine learning algorithm, to observe the model accuracy for performance and evaluating the confusion matrix.<br>
6.Comparing seven classical ML classifiers by calculating the accuracy as F1-Score for each ML classifier.<br>
7.Setting up a Stacking classifier using each of the previous classifiers as an estimator and evaluating the F-1 Score for training and test dataset.<br>
8.Trying to reduce the number of features for important features from the dataset and then evaluating the accuracy for training and test dataset.<br>
