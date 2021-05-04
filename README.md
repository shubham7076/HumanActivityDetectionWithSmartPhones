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

![alt text](https://imgur.com/WTKA3de)


## Features
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



## Goal

1.Performing Exploratory data analysis (EDA) differentiating the six activities(Target Variable) <br>
 1.1 Sitting <br>
 1.2 Walking <br>
 1.3.Walking_upstairs <br>
 1.4 Walking_downstairs <br>
 1.5 Lying <br>
 1.6 Standing <br>
 into static and Dynamic Activities using visualization techniques.<br>
<br>
<br>
2. Activity Exploration <br>
    2.1 Are The Activities Separable? <br>
    2.2 How Good Are The Activities Separable? <br>
<br>
<br>
3. Dimensionality Reduction
   3.2 Which Perplexity value performs best with TSNE? <br>
   3.1 Which Sensor Is More Important For Classifying Participants By Walking Style? <br>
<br>
<br>
5. which classifier performs best for the activity detection? <br>
   5.1 Finding the best estimator with Gridsearch <br>
