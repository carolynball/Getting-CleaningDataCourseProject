##Course Project In Getting and Cleaning Data Codebook
##About the Project
This codebook provides detail regarding the course project for Getting and Cleaning Data.   The purpose of the project was to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. 

The data for the project can be found at: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

 It was necessary to create one R script called run_analysis.R that does the following:
1.	Merges the training and the test sets to create one data set.
2.	Extracts only the measurements on the mean and standard deviation for each measurement. 
3.	Uses descriptive activity names to name the activities in the data set
4.	Appropriately labels the data set with descriptive variable names. 
5.	Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

##The Tidy Data Set
For this project, a tidy data set called AveVariablebySubjectActivity was created. It summarizes the average of each variable measured and groups these measures by subject and activity label. The completed tidy data set should only contain the average of the features with the word “mean” or “std” (for standard deviation) features. 


##The description for the data set is below:
AverageVariablebySubjectActivity		Original Variable			Source Files
subject|					subject					subject_test.txt & subject_train.txt
activitylabel					Activitylabel				activity_labels.txt & Y_test.txt
"avg-tBodyAcc-mean-X"				"tBodyAcc-mean()-X"			X_test.txt & X_train.txt
"avg-tBodyAcc-mean-Y"				"tBodyAcc-mean()-Y"			X_test.txt & X_train.txt
"avg-tBodyAcc-mean-Z"				"tBodyAcc-mean()-Z"			X_test.txt & X_train.txt
"avg-tBodyAcc-std-X"				"tBodyAcc-std()-X"			X_test.txt & X_train.txt
"avg-tBodyAcc-std-Y"				"tBodyAcc-std()-Y"			X_test.txt & X_train.txt
"avg-tBodyAcc-std-Z"				"tBodyAcc-std()-Z"			X_test.txt & X_train.txt
"avg-tGravityAcc-mean-X"			"tGravityAcc-mean()-X"			X_test.txt & X_train.txt
"avg-tGravityAcc-mean-Y"			"tGravityAcc-mean()-Y"			X_test.txt & X_train.txt
"avg-tGravityAcc-mean-Z"			"tGravityAcc-mean()-Z"			X_test.txt & X_train.txt
"avg-tGravityAcc-std-X"				"tGravityAcc-std()-X"			X_test.txt & X_train.txt
"avg-tGravityAcc-std-Y"				"tGravityAcc-std()-Y"			X_test.txt & X_train.txt
"avg-tGravityAcc-std-Z"				"tGravityAcc-std()-Z"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-mean-X"			"tBodyAccJerk-mean()-X"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-mean-Y"			"tBodyAccJerk-mean()-Y"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-mean-Z"			"tBodyAccJerk-mean()-Z"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-std-X"			"tBodyAccJerk-std()-X"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-std-Y"			"tBodyAccJerk-std()-Y"			X_test.txt & X_train.txt
"avg-tBodyAccJerk-std-Z"			"tBodyAccJerk-std()-Z"			X_test.txt & X_train.txt
"avg-tBodyGyro-mean-X"				"tBodyGyro-mean()-X"			X_test.txt & X_train.txt
"avg-tBodyGyro-mean-Y"				"tBodyGyro-mean()-Y"			X_test.txt & X_train.txt
"avg-tBodyGyro-mean-Z"				"tBodyGyro-mean()-Z"			X_test.txt & X_train.txt
"avg-tBodyGyro-std-X"				"tBodyGyro-std()-X"			X_test.txt & X_train.txt
"avg-tBodyGyro-std-Y"				"tBodyGyro-std()-Y"			X_test.txt & X_train.txt
"avg-tBodyGyro-std-Z"				"tBodyGyro-std()-Z"			X_test.txt & X_train.txt
"avg-tBodyGyroJerk-mean-X"			"tBodyGyroJerk-mean()-X"		X_test.txt & X_train.txt
"avg-tBodyGyroJerk-mean-Y"			"tBodyGyroJerk-mean()-Y"		X_test.txt & X_train.txt
"avg-tBodyGyroJerk-mean-Z"			"tBodyGyroJerk-mean()-Z"		X_test.txt & X_train.txt
"avg-tBodyGyroJerk-std-X"			"tBodyGyroJerk-std()-X"			X_test.txt & X_train.txt
"avg-tBodyGyroJerk-std-Y"			"tBodyGyroJerk-std()-Y"			X_test.txt & X_train.txt
"avg-tBodyGyroJerk-std-Z"			"tBodyGyroJerk-std()-Z"			X_test.txt & X_train.txt
"avg-tBodyAccMag-mean"				"tBodyAccMag-mean()"			X_test.txt & X_train.txt
"avg-tBodyAccMag-std"				"tBodyAccMag-std()"			X_test.txt & X_train.txt
"avg-tGravityAccMag-mean"			"tGravityAccMag-mean()"			X_test.txt & X_train.txt
"avg-tGravityAccMag-std"			"tGravityAccMag-std()"			X_test.txt & X_train.txt
"avg-tBodyAccJerkMag-mean"			"tBodyAccJerkMag-mean()"		X_test.txt & X_train.txt
"avg-tBodyAccJerkMag-std"			"tBodyAccJerkMag-std()"			X_test.txt & X_train.txt
"avg-tBodyGyroMag-mean"				"tBodyGyroMag-mean()"			X_test.txt & X_train.txt
"avg-tBodyGyroMag-std"				"tBodyGyroMag-std()"			X_test.txt & X_train.txt
"avg-tBodyGyroJerkMag-mean"			"tBodyGyroJerkMag-mean()"		X_test.txt & X_train.txt
"avg-tBodyGyroJerkMag-std"			"tBodyGyroJerkMag-std()"		X_test.txt & X_train.txt
"avg-fBodyAcc-mean-X"				"fBodyAcc-mean()-X"			X_test.txt & X_train.txt
"avg-fBodyAcc-mean-Y"				"fBodyAcc-mean()-Y"			X_test.txt & X_train.txt
"avg-fBodyAcc-mean-Z"				"fBodyAcc-mean()-Z"			X_test.txt & X_train.txt
"avg-fBodyAcc-std-X"				"fBodyAcc-std()-X"			X_test.txt & X_train.txt
"avg-fBodyAcc-std-Y"				"fBodyAcc-std()-Y"			X_test.txt & X_train.txt
"avg-fBodyAcc-std-Z"				"fBodyAcc-std()-Z"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-mean-X"			"fBodyAccJerk-mean()-X"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-mean-Y"			"fBodyAccJerk-mean()-Y"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-mean-Z"			"fBodyAccJerk-mean()-Z"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-std-X"			"fBodyAccJerk-std()-X"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-std-Y"			"fBodyAccJerk-std()-Y"			X_test.txt & X_train.txt
"avg-fBodyAccJerk-std-Z"			"fBodyAccJerk-std()-Z"			X_test.txt & X_train.txt
"avg-fBodyGyro-mean-X"				"fBodyGyro-mean()-X"			X_test.txt & X_train.txt
"avg-fBodyGyro-mean-Y"				"fBodyGyro-mean()-Y"			X_test.txt & X_train.txt
"avg-fBodyGyro-mean-Z"				"fBodyGyro-mean()-Z"			X_test.txt & X_train.txt
"avg-fBodyGyro-std-X"				"fBodyGyro-std()-X"			X_test.txt & X_train.txt
"avg-fBodyGyro-std-Y"				"fBodyGyro-std()-Y"			X_test.txt & X_train.txt
"avg-fBodyGyro-std-Z"				"fBodyGyro-std()-Z"			X_test.txt & X_train.txt
"avg-fBodyAccMag-mean"				"fBodyAccMag-mean()"			X_test.txt & X_train.txt
"avg-fBodyAccMag-std"				"fBodyAccMag-std()"			X_test.txt & X_train.txt
"avg-fBodyBodyAccJerkMag-mean"			"fBodyBodyAccJerkMag-mean()"		X_test.txt & X_train.txt
"avg-fBodyBodyAccJerkMag-std"			"fBodyBodyAccJerkMag-std()"		X_test.txt & X_train.txt
"avg-fBodyBodyGyroMag-mean"			"fBodyBodyGyroMag-mean()"		X_test.txt & X_train.txt
"avg-fBodyBodyGyroMag-std"			"fBodyBodyGyroMag-std()"		X_test.txt & X_train.txt
"avg-fBodyBodyGyroJerkMag-mean"			"fBodyBodyGyroJerkMag-mean()"		X_test.txt & X_train.txt
"avg-fBodyBodyGyroJerkMag-std"			"fBodyBodyGyroJerkMag-std()"		X_test.txt & X_train.txt
"avg-angle(tBodyAccMeangravity)"		"angle(tBodyAccMean gravity)"		X_test.txt & X_train.txt
"avg-angle(tBodyAccJerkMean)gravityMean)"	"angle(tBodyAccJerkMean) gravityMean)"	X_test.txt & X_train.txt
"avg-angle(tBodyGyroMean,gravityMean)"		"angle(tBodyGyroMean, gravityMean)"	X_test.txt & X_train.txt
"avg-angle(tBodyGyroJerkMean,gravityMean)"	"angle(tBodyGyroJerkMean, gravityMean)"	X_test.txt & X_train.txt
"avg-angle(X,gravityMean)"			"angle(X, gravityMean)"			X_test.txt & X_train.txt
"avg-angle(Y,gravityMean)"			"angle(Y, gravityMean)"			X_test.txt & X_train.txt
"avg-angle(Z,gravityMean))"			"angle(Z, gravityMean)"			X_test.txt & X_train.txt


Dataset Summary
The following files were part of the source dataset:
•	README.txt
•	features_info.txt
•	features.txt
•	activity_labels.txt
•	X_train.txt
•	y_train.txt
•	X_test.txt
•	y_test.txt
•	subject_train.txt
•	total_acc_x_train.txt
•	total_acc_x_train.txt
•	total_acc_z_train.txt
•	body_acc_x_train.txt

The following is a list of the selected files that were used for the project:
•	features_info.txt
•	features.txt
•	activity_labels.txt
•	X_train.txt
•	y_train.txt
•	X_test.txt
•	y_test.txt
•	subject_train.txt
•	subject_train.txt
The subject_train.txt and subject_train.txt files were assumed to be the subject’s identifier. As it was not stated in the documentation, it was also assumed Subject 1 in one file was the same person as Subject 1 in the other file.
The y_train.txt and y_test.txt files were assumed to correspond to the activities that were being measured. There were 6 possible values in these files so it was assumed the number corresponded to the number and activity description in activity-labels.txt.
The number of rows in features.txt was the same as the number of columns in X_train.txt and X_test.txt. It was assumed the values in features.txt were the column names. It was also assumed they were in the same order.
The features_info.txt to understand the meaning of the variables.
Finally, the number of rows in X_train.txt, y_train.txt and subject_train.txt were equal and it was assumed they corresponded in order. The same was done for the test files.
##Project/Study Design
This section details the code used to complete the project
options (warn=-1)

library(dplyr)

Determine current working directory
getwd()

change wd if necessary
setwd("C:/Users/cball/Documents/R/UCI HAR Dataset")

read labels data into tables
activity_labels<-read.table("./activity_labels.txt")
features<-read.table("./features.txt")

##read test table data in as objects##
subject_test<-read.table("./test/subject_test.txt")
x_test<-read.table("./test/X_test.txt")
y_test<-read.table("./test/y_test.txt")

##read train table data in as objects##
subject_train<-read.table("./train/subject_train.txt")
x_train<-read.table("./train/X_train.txt")
y_train<-read.table("./train/y_train.txt")

##Merges training & test sets to create 1 data set for X, y & subject respectively
Merge tables into 3 respective entities.  x to x, y to y, and sub to
binding by rows
xreadings<-rbind(x_test,x_train)
subjectconsol<-rbind(subject_test, subject_train)
yactivity<-rbind(y_test, y_train)

dim(xreadings)
dim(subjectconsol)
dim(yactivity)

Merge consolidated training & test sets x, y and sub into 1 master via column bind
Mergeddata<-cbind(subjectconsol, yactivity, xreadings)

Add Column names to the merged and consolidated
Assume the first column is the subject, 2nd column "activity" as 6 variables
which correspond with 6 values in activity_labels.txt, and features were the
x variable train and test data
colnames(Mergeddata) <- c("subject", "activity","tBodyAcc-mean()-X",
                        "tBodyAcc-mean()-Y",
                        "tBodyAcc-mean()-Z",
                        "tBodyAcc-std()-X",
                        "tBodyAcc-std()-Y",
                        "tBodyAcc-std()-Z",
                        "tBodyAcc-mad()-X",
                        "tBodyAcc-mad()-Y",
                        "tBodyAcc-mad()-Z",
                        "tBodyAcc-max()-X",
                        "tBodyAcc-max()-Y",
                        "tBodyAcc-max()-Z",
                        "tBodyAcc-min()-X",
                        "tBodyAcc-min()-Y",
                        "tBodyAcc-min()-Z",
                        "tBodyAcc-sma()",
                        "tBodyAcc-energy()-X",
                        "tBodyAcc-energy()-Y",
                        "tBodyAcc-energy()-Z",
                        "tBodyAcc-iqr()-X",
                        "tBodyAcc-iqr()-Y",
                        "tBodyAcc-iqr()-Z",
                        "tBodyAcc-entropy()-X",
                        "tBodyAcc-entropy()-Y",
                        "tBodyAcc-entropy()-Z",
                        "tBodyAcc-arCoeff()-X,1",
                        "tBodyAcc-arCoeff()-X,2",
                        "tBodyAcc-arCoeff()-X,3",
                        "tBodyAcc-arCoeff()-X,4",
                        "tBodyAcc-arCoeff()-Y,1",
                        "tBodyAcc-arCoeff()-Y,2",
                        "tBodyAcc-arCoeff()-Y,3",
                        "tBodyAcc-arCoeff()-Y,4",
                        "tBodyAcc-arCoeff()-Z,1",
                        "tBodyAcc-arCoeff()-Z,2",
                        "tBodyAcc-arCoeff()-Z,3",
                        "tBodyAcc-arCoeff()-Z,4",
                        "tBodyAcc-correlation()-X,Y",
                        "tBodyAcc-correlation()-X,Z",
                        "tBodyAcc-correlation()-Y,Z",
                        "tGravityAcc-mean()-X",
                        "tGravityAcc-mean()-Y",
                        "tGravityAcc-mean()-Z",
                        "tGravityAcc-std()-X",
                        "tGravityAcc-std()-Y",
                        "tGravityAcc-std()-Z",
                        "tGravityAcc-mad()-X",
                        "tGravityAcc-mad()-Y",
                        "tGravityAcc-mad()-Z",
                        "tGravityAcc-max()-X",
                        "tGravityAcc-max()-Y",
                        "tGravityAcc-max()-Z",
                        "tGravityAcc-min()-X",
                        "tGravityAcc-min()-Y",
                        "tGravityAcc-min()-Z",
                        "tGravityAcc-sma()",
                        "tGravityAcc-energy()-X",
                        "tGravityAcc-energy()-Y",
                        "tGravityAcc-energy()-Z",
                        "tGravityAcc-iqr()-X",
                        "tGravityAcc-iqr()-Y",
                        "tGravityAcc-iqr()-Z",
                        "tGravityAcc-entropy()-X",
                        "tGravityAcc-entropy()-Y",
                        "tGravityAcc-entropy()-Z",
                        "tGravityAcc-arCoeff()-X,1",
                        "tGravityAcc-arCoeff()-X,2",
                        "tGravityAcc-arCoeff()-X,3",
                        "tGravityAcc-arCoeff()-X,4",
                        "tGravityAcc-arCoeff()-Y,1",
                        "tGravityAcc-arCoeff()-Y,2",
                        "tGravityAcc-arCoeff()-Y,3",
                        "tGravityAcc-arCoeff()-Y,4",
                        "tGravityAcc-arCoeff()-Z,1",
                        "tGravityAcc-arCoeff()-Z,2",
                        "tGravityAcc-arCoeff()-Z,3",
                        "tGravityAcc-arCoeff()-Z,4",
                        "tGravityAcc-correlation()-X,Y",
                        "tGravityAcc-correlation()-X,Z",
                        "tGravityAcc-correlation()-Y,Z",
                        "tBodyAccJerk-mean()-X",
                        "tBodyAccJerk-mean()-Y",
                        "tBodyAccJerk-mean()-Z",
                        "tBodyAccJerk-std()-X",
                        "tBodyAccJerk-std()-Y",
                        "tBodyAccJerk-std()-Z",
                        "tBodyAccJerk-mad()-X",
                        "tBodyAccJerk-mad()-Y",
                        "tBodyAccJerk-mad()-Z",
                        "tBodyAccJerk-max()-X",
                        "tBodyAccJerk-max()-Y",
                        "tBodyAccJerk-max()-Z",
                        "tBodyAccJerk-min()-X",
                        "tBodyAccJerk-min()-Y",
                        "tBodyAccJerk-min()-Z",
                        "tBodyAccJerk-sma()",
                        "tBodyAccJerk-energy()-X",
                        "tBodyAccJerk-energy()-Y",
                        "tBodyAccJerk-energy()-Z",
                        "tBodyAccJerk-iqr()-X",
                        "tBodyAccJerk-iqr()-Y",
                        "tBodyAccJerk-iqr()-Z",
                        "tBodyAccJerk-entropy()-X",
                        "tBodyAccJerk-entropy()-Y",
                        "tBodyAccJerk-entropy()-Z",
                        "tBodyAccJerk-arCoeff()-X,1",
                        "tBodyAccJerk-arCoeff()-X,2",
                        "tBodyAccJerk-arCoeff()-X,3",
                        "tBodyAccJerk-arCoeff()-X,4",
                        "tBodyAccJerk-arCoeff()-Y,1",
                        "tBodyAccJerk-arCoeff()-Y,2",
                        "tBodyAccJerk-arCoeff()-Y,3",
                        "tBodyAccJerk-arCoeff()-Y,4",
                        "tBodyAccJerk-arCoeff()-Z,1",
                        "tBodyAccJerk-arCoeff()-Z,2",
                        "tBodyAccJerk-arCoeff()-Z,3",
                        "tBodyAccJerk-arCoeff()-Z,4",
                        "tBodyAccJerk-correlation()-X,Y",
                        "tBodyAccJerk-correlation()-X,Z",
                        "tBodyAccJerk-correlation()-Y,Z",
                        "tBodyGyro-mean()-X",
                        "tBodyGyro-mean()-Y",
                        "tBodyGyro-mean()-Z",
                        "tBodyGyro-std()-X",
                        "tBodyGyro-std()-Y",
                        "tBodyGyro-std()-Z",
                        "tBodyGyro-mad()-X",
                        "tBodyGyro-mad()-Y",
                        "tBodyGyro-mad()-Z",
                        "tBodyGyro-max()-X",
                        "tBodyGyro-max()-Y",
                        "tBodyGyro-max()-Z",
                        "tBodyGyro-min()-X",
                        "tBodyGyro-min()-Y",
                        "tBodyGyro-min()-Z",
                        "tBodyGyro-sma()",
                        "tBodyGyro-energy()-X",
                        "tBodyGyro-energy()-Y",
                        "tBodyGyro-energy()-Z",
                        "tBodyGyro-iqr()-X",
                        "tBodyGyro-iqr()-Y",
                        "tBodyGyro-iqr()-Z",
                        "tBodyGyro-entropy()-X",
                        "tBodyGyro-entropy()-Y",
                        "tBodyGyro-entropy()-Z",
                        "tBodyGyro-arCoeff()-X,1",
                        "tBodyGyro-arCoeff()-X,2",
                        "tBodyGyro-arCoeff()-X,3",
                        "tBodyGyro-arCoeff()-X,4",
                        "tBodyGyro-arCoeff()-Y,1",
                        "tBodyGyro-arCoeff()-Y,2",
                        "tBodyGyro-arCoeff()-Y,3",
                        "tBodyGyro-arCoeff()-Y,4",
                        "tBodyGyro-arCoeff()-Z,1",
                        "tBodyGyro-arCoeff()-Z,2",
                        "tBodyGyro-arCoeff()-Z,3",
                        "tBodyGyro-arCoeff()-Z,4",
                        "tBodyGyro-correlation()-X,Y",
                        "tBodyGyro-correlation()-X,Z",
                        "tBodyGyro-correlation()-Y,Z",
                        "tBodyGyroJerk-mean()-X",
                        "tBodyGyroJerk-mean()-Y",
                        "tBodyGyroJerk-mean()-Z",
                        "tBodyGyroJerk-std()-X",
                        "tBodyGyroJerk-std()-Y",
                        "tBodyGyroJerk-std()-Z",
                        "tBodyGyroJerk-mad()-X",
                        "tBodyGyroJerk-mad()-Y",
                        "tBodyGyroJerk-mad()-Z",
                        "tBodyGyroJerk-max()-X",
                        "tBodyGyroJerk-max()-Y",
                        "tBodyGyroJerk-max()-Z",
                        "tBodyGyroJerk-min()-X",
                        "tBodyGyroJerk-min()-Y",
                        "tBodyGyroJerk-min()-Z",
                        "tBodyGyroJerk-sma()",
                        "tBodyGyroJerk-energy()-X",
                        "tBodyGyroJerk-energy()-Y",
                        "tBodyGyroJerk-energy()-Z",
                        "tBodyGyroJerk-iqr()-X",
                        "tBodyGyroJerk-iqr()-Y",
                        "tBodyGyroJerk-iqr()-Z",
                        "tBodyGyroJerk-entropy()-X",
                        "tBodyGyroJerk-entropy()-Y",
                        "tBodyGyroJerk-entropy()-Z",
                        "tBodyGyroJerk-arCoeff()-X,1",
                        "tBodyGyroJerk-arCoeff()-X,2",
                        "tBodyGyroJerk-arCoeff()-X,3",
                        "tBodyGyroJerk-arCoeff()-X,4",
                        "tBodyGyroJerk-arCoeff()-Y,1",
                        "tBodyGyroJerk-arCoeff()-Y,2",
                        "tBodyGyroJerk-arCoeff()-Y,3",
                        "tBodyGyroJerk-arCoeff()-Y,4",
                        "tBodyGyroJerk-arCoeff()-Z,1",
                        "tBodyGyroJerk-arCoeff()-Z,2",
                        "tBodyGyroJerk-arCoeff()-Z,3",
                        "tBodyGyroJerk-arCoeff()-Z,4",
                        "tBodyGyroJerk-correlation()-X,Y",
                        "tBodyGyroJerk-correlation()-X,Z",
                        "tBodyGyroJerk-correlation()-Y,Z",
                        "tBodyAccMag-mean()",
                        "tBodyAccMag-std()",
                        "tBodyAccMag-mad()",
                        "tBodyAccMag-max()",
                        "tBodyAccMag-min()",
                        "tBodyAccMag-sma()",
                        "tBodyAccMag-energy()",
                        "tBodyAccMag-iqr()",
                        "tBodyAccMag-entropy()",
                        "tBodyAccMag-arCoeff()1",
                        "tBodyAccMag-arCoeff()2",
                        "tBodyAccMag-arCoeff()3",
                        "tBodyAccMag-arCoeff()4",
                        "tGravityAccMag-mean()",
                        "tGravityAccMag-std()",
                        "tGravityAccMag-mad()",
                        "tGravityAccMag-max()",
                        "tGravityAccMag-min()",
                        "tGravityAccMag-sma()",
                        "tGravityAccMag-energy()",
                        "tGravityAccMag-iqr()",
                        "tGravityAccMag-entropy()",
                        "tGravityAccMag-arCoeff()1",
                        "tGravityAccMag-arCoeff()2",
                        "tGravityAccMag-arCoeff()3",
                        "tGravityAccMag-arCoeff()4",
                        "tBodyAccJerkMag-mean()",
                        "tBodyAccJerkMag-std()",
                        "tBodyAccJerkMag-mad()",
                        "tBodyAccJerkMag-max()",
                        "tBodyAccJerkMag-min()",
                        "tBodyAccJerkMag-sma()",
                        "tBodyAccJerkMag-energy()",
                        "tBodyAccJerkMag-iqr()",
                        "tBodyAccJerkMag-entropy()",
                        "tBodyAccJerkMag-arCoeff()1",
                        "tBodyAccJerkMag-arCoeff()2",
                        "tBodyAccJerkMag-arCoeff()3",
                        "tBodyAccJerkMag-arCoeff()4",
                        "tBodyGyroMag-mean()",
                        "tBodyGyroMag-std()",
                        "tBodyGyroMag-mad()",
                        "tBodyGyroMag-max()",
                        "tBodyGyroMag-min()",
                        "tBodyGyroMag-sma()",
                        "tBodyGyroMag-energy()",
                        "tBodyGyroMag-iqr()",
                        "tBodyGyroMag-entropy()",
                        "tBodyGyroMag-arCoeff()1",
                        "tBodyGyroMag-arCoeff()2",
                        "tBodyGyroMag-arCoeff()3",
                        "tBodyGyroMag-arCoeff()4",
                        "tBodyGyroJerkMag-mean()",
                        "tBodyGyroJerkMag-std()",
                        "tBodyGyroJerkMag-mad()",
                        "tBodyGyroJerkMag-max()",
                        "tBodyGyroJerkMag-min()",
                        "tBodyGyroJerkMag-sma()",
                        "tBodyGyroJerkMag-energy()",
                        "tBodyGyroJerkMag-iqr()",
                        "tBodyGyroJerkMag-entropy()",
                        "tBodyGyroJerkMag-arCoeff()1",
                        "tBodyGyroJerkMag-arCoeff()2",
                        "tBodyGyroJerkMag-arCoeff()3",
                        "tBodyGyroJerkMag-arCoeff()4",
                        "fBodyAcc-mean()-X",
                        "fBodyAcc-mean()-Y",
                        "fBodyAcc-mean()-Z",
                        "fBodyAcc-std()-X",
                        "fBodyAcc-std()-Y",
                        "fBodyAcc-std()-Z",
                        "fBodyAcc-mad()-X",
                        "fBodyAcc-mad()-Y",
                        "fBodyAcc-mad()-Z",
                        "fBodyAcc-max()-X",
                        "fBodyAcc-max()-Y",
                        "fBodyAcc-max()-Z",
                        "fBodyAcc-min()-X",
                        "fBodyAcc-min()-Y",
                        "fBodyAcc-min()-Z",
                        "fBodyAcc-sma()",
                        "fBodyAcc-energy()-X",
                        "fBodyAcc-energy()-Y",
                        "fBodyAcc-energy()-Z",
                        "fBodyAcc-iqr()-X",
                        "fBodyAcc-iqr()-Y",
                        "fBodyAcc-iqr()-Z",
                        "fBodyAcc-entropy()-X",
                        "fBodyAcc-entropy()-Y",
                        "fBodyAcc-entropy()-Z",
                        "fBodyAcc-maxInds-X",
                        "fBodyAcc-maxInds-Y",
                        "fBodyAcc-maxInds-Z",
                        "fBodyAcc-meanFreq()-X",
                        "fBodyAcc-meanFreq()-Y",
                        "fBodyAcc-meanFreq()-Z",
                        "fBodyAcc-skewness()-X",
                        "fBodyAcc-kurtosis()-X",
                        "fBodyAcc-skewness()-Y",
                        "fBodyAcc-kurtosis()-Y",
                        "fBodyAcc-skewness()-Z",
                        "fBodyAcc-kurtosis()-Z",
                        "fBodyAcc-bandsEnergy()-1,8",
                        "fBodyAcc-bandsEnergy()-9,16",
                        "fBodyAcc-bandsEnergy()-17,24",
                        "fBodyAcc-bandsEnergy()-25,32",
                        "fBodyAcc-bandsEnergy()-33,40",
                        "fBodyAcc-bandsEnergy()-41,48",
                        "fBodyAcc-bandsEnergy()-49,56",
                        "fBodyAcc-bandsEnergy()-57,64",
                        "fBodyAcc-bandsEnergy()-1,16",
                        "fBodyAcc-bandsEnergy()-17,32",
                        "fBodyAcc-bandsEnergy()-33,48",
                        "fBodyAcc-bandsEnergy()-49,64",
                        "fBodyAcc-bandsEnergy()-1,24",
                        "fBodyAcc-bandsEnergy()-25,48",
                        "fBodyAcc-bandsEnergy()-1,8",
                        "fBodyAcc-bandsEnergy()-9,16",
                        "fBodyAcc-bandsEnergy()-17,24",
                        "fBodyAcc-bandsEnergy()-25,32",
                        "fBodyAcc-bandsEnergy()-33,40",
                        "fBodyAcc-bandsEnergy()-41,48",
                        "fBodyAcc-bandsEnergy()-49,56",
                        "fBodyAcc-bandsEnergy()-57,64",
                        "fBodyAcc-bandsEnergy()-1,16",
                        "fBodyAcc-bandsEnergy()-17,32",
                        "fBodyAcc-bandsEnergy()-33,48",
                        "fBodyAcc-bandsEnergy()-49,64",
                        "fBodyAcc-bandsEnergy()-1,24",
                        "fBodyAcc-bandsEnergy()-25,48",
                        "fBodyAcc-bandsEnergy()-1,8",
                        "fBodyAcc-bandsEnergy()-9,16",
                        "fBodyAcc-bandsEnergy()-17,24",
                        "fBodyAcc-bandsEnergy()-25,32",
                        "fBodyAcc-bandsEnergy()-33,40",
                        "fBodyAcc-bandsEnergy()-41,48",
                        "fBodyAcc-bandsEnergy()-49,56",
                        "fBodyAcc-bandsEnergy()-57,64",
                        "fBodyAcc-bandsEnergy()-1,16",
                        "fBodyAcc-bandsEnergy()-17,32",
                        "fBodyAcc-bandsEnergy()-33,48",
                        "fBodyAcc-bandsEnergy()-49,64",
                        "fBodyAcc-bandsEnergy()-1,24",
                        "fBodyAcc-bandsEnergy()-25,48",
                        "fBodyAccJerk-mean()-X",
                        "fBodyAccJerk-mean()-Y",
                        "fBodyAccJerk-mean()-Z",
                        "fBodyAccJerk-std()-X",
                        "fBodyAccJerk-std()-Y",
                        "fBodyAccJerk-std()-Z",
                        "fBodyAccJerk-mad()-X",
                        "fBodyAccJerk-mad()-Y",
                        "fBodyAccJerk-mad()-Z",
                        "fBodyAccJerk-max()-X",
                        "fBodyAccJerk-max()-Y",
                        "fBodyAccJerk-max()-Z",
                        "fBodyAccJerk-min()-X",
                        "fBodyAccJerk-min()-Y",
                        "fBodyAccJerk-min()-Z",
                        "fBodyAccJerk-sma()",
                        "fBodyAccJerk-energy()-X",
                        "fBodyAccJerk-energy()-Y",
                        "fBodyAccJerk-energy()-Z",
                        "fBodyAccJerk-iqr()-X",
                        "fBodyAccJerk-iqr()-Y",
                        "fBodyAccJerk-iqr()-Z",
                        "fBodyAccJerk-entropy()-X",
                        "fBodyAccJerk-entropy()-Y",
                        "fBodyAccJerk-entropy()-Z",
                        "fBodyAccJerk-maxInds-X",
                        "fBodyAccJerk-maxInds-Y",
                        "fBodyAccJerk-maxInds-Z",
                        "fBodyAccJerk-meanFreq()-X",
                        "fBodyAccJerk-meanFreq()-Y",
                        "fBodyAccJerk-meanFreq()-Z",
                        "fBodyAccJerk-skewness()-X",
                        "fBodyAccJerk-kurtosis()-X",
                        "fBodyAccJerk-skewness()-Y",
                        "fBodyAccJerk-kurtosis()-Y",
                        "fBodyAccJerk-skewness()-Z",
                        "fBodyAccJerk-kurtosis()-Z",
                        "fBodyAccJerk-bandsEnergy()-1,8",
                        "fBodyAccJerk-bandsEnergy()-9,16",
                        "fBodyAccJerk-bandsEnergy()-17,24",
                        "fBodyAccJerk-bandsEnergy()-25,32",
                        "fBodyAccJerk-bandsEnergy()-33,40",
                        "fBodyAccJerk-bandsEnergy()-41,48",
                        "fBodyAccJerk-bandsEnergy()-49,56",
                        "fBodyAccJerk-bandsEnergy()-57,64",
                        "fBodyAccJerk-bandsEnergy()-1,16",
                        "fBodyAccJerk-bandsEnergy()-17,32",
                        "fBodyAccJerk-bandsEnergy()-33,48",
                        "fBodyAccJerk-bandsEnergy()-49,64",
                        "fBodyAccJerk-bandsEnergy()-1,24",
                        "fBodyAccJerk-bandsEnergy()-25,48",
                        "fBodyAccJerk-bandsEnergy()-1,8",
                        "fBodyAccJerk-bandsEnergy()-9,16",
                        "fBodyAccJerk-bandsEnergy()-17,24",
                        "fBodyAccJerk-bandsEnergy()-25,32",
                        "fBodyAccJerk-bandsEnergy()-33,40",
                        "fBodyAccJerk-bandsEnergy()-41,48",
                        "fBodyAccJerk-bandsEnergy()-49,56",
                        "fBodyAccJerk-bandsEnergy()-57,64",
                        "fBodyAccJerk-bandsEnergy()-1,16",
                        "fBodyAccJerk-bandsEnergy()-17,32",
                        "fBodyAccJerk-bandsEnergy()-33,48",
                        "fBodyAccJerk-bandsEnergy()-49,64",
                        "fBodyAccJerk-bandsEnergy()-1,24",
                        "fBodyAccJerk-bandsEnergy()-25,48",
                        "fBodyAccJerk-bandsEnergy()-1,8",
                        "fBodyAccJerk-bandsEnergy()-9,16",
                        "fBodyAccJerk-bandsEnergy()-17,24",
                        "fBodyAccJerk-bandsEnergy()-25,32",
                        "fBodyAccJerk-bandsEnergy()-33,40",
                        "fBodyAccJerk-bandsEnergy()-41,48",
                        "fBodyAccJerk-bandsEnergy()-49,56",
                        "fBodyAccJerk-bandsEnergy()-57,64",
                        "fBodyAccJerk-bandsEnergy()-1,16",
                        "fBodyAccJerk-bandsEnergy()-17,32",
                        "fBodyAccJerk-bandsEnergy()-33,48",
                        "fBodyAccJerk-bandsEnergy()-49,64",
                        "fBodyAccJerk-bandsEnergy()-1,24",
                        "fBodyAccJerk-bandsEnergy()-25,48",
                        "fBodyGyro-mean()-X",
                        "fBodyGyro-mean()-Y",
                        "fBodyGyro-mean()-Z",
                        "fBodyGyro-std()-X",
                        "fBodyGyro-std()-Y",
                        "fBodyGyro-std()-Z",
                        "fBodyGyro-mad()-X",
                        "fBodyGyro-mad()-Y",
                        "fBodyGyro-mad()-Z",
                        "fBodyGyro-max()-X",
                        "fBodyGyro-max()-Y",
                        "fBodyGyro-max()-Z",
                        "fBodyGyro-min()-X",
                        "fBodyGyro-min()-Y",
                        "fBodyGyro-min()-Z",
                        "fBodyGyro-sma()",
                        "fBodyGyro-energy()-X",
                        "fBodyGyro-energy()-Y",
                        "fBodyGyro-energy()-Z",
                        "fBodyGyro-iqr()-X",
                        "fBodyGyro-iqr()-Y",
                        "fBodyGyro-iqr()-Z",
                        "fBodyGyro-entropy()-X",
                        "fBodyGyro-entropy()-Y",
                        "fBodyGyro-entropy()-Z",
                        "fBodyGyro-maxInds-X",
                        "fBodyGyro-maxInds-Y",
                        "fBodyGyro-maxInds-Z",
                        "fBodyGyro-meanFreq()-X",
                        "fBodyGyro-meanFreq()-Y",
                        "fBodyGyro-meanFreq()-Z",
                        "fBodyGyro-skewness()-X",
                        "fBodyGyro-kurtosis()-X",
                        "fBodyGyro-skewness()-Y",
                        "fBodyGyro-kurtosis()-Y",
                        "fBodyGyro-skewness()-Z",
                        "fBodyGyro-kurtosis()-Z",
                        "fBodyGyro-bandsEnergy()-1,8",
                        "fBodyGyro-bandsEnergy()-9,16",
                        "fBodyGyro-bandsEnergy()-17,24",
                        "fBodyGyro-bandsEnergy()-25,32",
                        "fBodyGyro-bandsEnergy()-33,40",
                        "fBodyGyro-bandsEnergy()-41,48",
                        "fBodyGyro-bandsEnergy()-49,56",
                        "fBodyGyro-bandsEnergy()-57,64",
                        "fBodyGyro-bandsEnergy()-1,16",
                        "fBodyGyro-bandsEnergy()-17,32",
                        "fBodyGyro-bandsEnergy()-33,48",
                        "fBodyGyro-bandsEnergy()-49,64",
                        "fBodyGyro-bandsEnergy()-1,24",
                        "fBodyGyro-bandsEnergy()-25,48",
                        "fBodyGyro-bandsEnergy()-1,8",
                        "fBodyGyro-bandsEnergy()-9,16",
                        "fBodyGyro-bandsEnergy()-17,24",
                        "fBodyGyro-bandsEnergy()-25,32",
                        "fBodyGyro-bandsEnergy()-33,40",
                        "fBodyGyro-bandsEnergy()-41,48",
                        "fBodyGyro-bandsEnergy()-49,56",
                        "fBodyGyro-bandsEnergy()-57,64",
                        "fBodyGyro-bandsEnergy()-1,16",
                        "fBodyGyro-bandsEnergy()-17,32",
                        "fBodyGyro-bandsEnergy()-33,48",
                        "fBodyGyro-bandsEnergy()-49,64",
                        "fBodyGyro-bandsEnergy()-1,24",
                        "fBodyGyro-bandsEnergy()-25,48",
                        "fBodyGyro-bandsEnergy()-1,8",
                        "fBodyGyro-bandsEnergy()-9,16",
                        "fBodyGyro-bandsEnergy()-17,24",
                        "fBodyGyro-bandsEnergy()-25,32",
                        "fBodyGyro-bandsEnergy()-33,40",
                        "fBodyGyro-bandsEnergy()-41,48",
                        "fBodyGyro-bandsEnergy()-49,56",
                        "fBodyGyro-bandsEnergy()-57,64",
                        "fBodyGyro-bandsEnergy()-1,16",
                        "fBodyGyro-bandsEnergy()-17,32",
                        "fBodyGyro-bandsEnergy()-33,48",
                        "fBodyGyro-bandsEnergy()-49,64",
                        "fBodyGyro-bandsEnergy()-1,24",
                        "fBodyGyro-bandsEnergy()-25,48",
                        "fBodyAccMag-mean()",
                        "fBodyAccMag-std()",
                        "fBodyAccMag-mad()",
                        "fBodyAccMag-max()",
                        "fBodyAccMag-min()",
                        "fBodyAccMag-sma()",
                        "fBodyAccMag-energy()",
                        "fBodyAccMag-iqr()",
                        "fBodyAccMag-entropy()",
                        "fBodyAccMag-maxInds",
                        "fBodyAccMag-meanFreq()",
                        "fBodyAccMag-skewness()",
                        "fBodyAccMag-kurtosis()",
                        "fBodyBodyAccJerkMag-mean()",
                        "fBodyBodyAccJerkMag-std()",
                        "fBodyBodyAccJerkMag-mad()",
                        "fBodyBodyAccJerkMag-max()",
                        "fBodyBodyAccJerkMag-min()",
                        "fBodyBodyAccJerkMag-sma()",
                        "fBodyBodyAccJerkMag-energy()",
                        "fBodyBodyAccJerkMag-iqr()",
                        "fBodyBodyAccJerkMag-entropy()",
                        "fBodyBodyAccJerkMag-maxInds",
                        "fBodyBodyAccJerkMag-meanFreq()",
                        "fBodyBodyAccJerkMag-skewness()",
                        "fBodyBodyAccJerkMag-kurtosis()",
                        "fBodyBodyGyroMag-mean()",
                        "fBodyBodyGyroMag-std()",
                        "fBodyBodyGyroMag-mad()",
                        "fBodyBodyGyroMag-max()",
                        "fBodyBodyGyroMag-min()",
                        "fBodyBodyGyroMag-sma()",
                        "fBodyBodyGyroMag-energy()",
                        "fBodyBodyGyroMag-iqr()",
                        "fBodyBodyGyroMag-entropy()",
                        "fBodyBodyGyroMag-maxInds",
                        "fBodyBodyGyroMag-meanFreq()",
                        "fBodyBodyGyroMag-skewness()",
                        "fBodyBodyGyroMag-kurtosis()",
                        "fBodyBodyGyroJerkMag-mean()",
                        "fBodyBodyGyroJerkMag-std()",
                        "fBodyBodyGyroJerkMag-mad()",
                        "fBodyBodyGyroJerkMag-max()",
                        "fBodyBodyGyroJerkMag-min()",
                        "fBodyBodyGyroJerkMag-sma()",
                        "fBodyBodyGyroJerkMag-energy()",
                        "fBodyBodyGyroJerkMag-iqr()",
                        "fBodyBodyGyroJerkMag-entropy()",
                        "fBodyBodyGyroJerkMag-maxInds",
                        "fBodyBodyGyroJerkMag-meanFreq()",
                        "fBodyBodyGyroJerkMag-skewness()",
                        "fBodyBodyGyroJerkMag-kurtosis()",
                        "angle(tBodyAccMean,gravity)",
                        "angle(tBodyAccJerkMean),gravityMean)",
                        "angle(tBodyGyroMean,gravityMean)",
                        "angle(tBodyGyroJerkMean,gravityMean)",
                        "angle(X,gravityMean)",
                        "angle(Y,gravityMean)",
                        "angle(Z,gravityMean)")

Per course instructions #2, extracts only the measurements that include
the mean and standard deviation for each measurement into new table Mergeddata2
Mergeddata2<-Mergeddata[,c("subject", "activity","tBodyAcc-mean()-X",
             "tBodyAcc-mean()-Y",
             "tBodyAcc-mean()-Z",
             "tBodyAcc-std()-X",
             "tBodyAcc-std()-Y",
             "tBodyAcc-std()-Z",
             "tGravityAcc-mean()-X",
             "tGravityAcc-mean()-Y",
             "tGravityAcc-mean()-Z",
             "tGravityAcc-std()-X",
             "tGravityAcc-std()-Y",
             "tGravityAcc-std()-Z",
             "tBodyAccJerk-mean()-X",
             "tBodyAccJerk-mean()-Y",
             "tBodyAccJerk-mean()-Z",
             "tBodyAccJerk-std()-X",
             "tBodyAccJerk-std()-Y",
             "tBodyAccJerk-std()-Z",
             "tBodyGyro-mean()-X",
             "tBodyGyro-mean()-Y",
             "tBodyGyro-mean()-Z",
             "tBodyGyro-std()-X",
             "tBodyGyro-std()-Y",
             "tBodyGyro-std()-Z",
             "tBodyGyroJerk-mean()-X",
             "tBodyGyroJerk-mean()-Y",
             "tBodyGyroJerk-mean()-Z",
             "tBodyGyroJerk-std()-X",
             "tBodyGyroJerk-std()-Y",
             "tBodyGyroJerk-std()-Z",
           "tBodyAccMag-mean()",
             "tBodyAccMag-std()",
             "tGravityAccMag-mean()",
             "tGravityAccMag-std()",
               "tBodyAccJerkMag-mean()",
             "tBodyAccJerkMag-std()",
             "tBodyGyroMag-mean()",
             "tBodyGyroMag-std()",
             "tBodyGyroJerkMag-mean()",
             "tBodyGyroJerkMag-std()",
             "fBodyAcc-mean()-X",
             "fBodyAcc-mean()-Y",
             "fBodyAcc-mean()-Z",
             "fBodyAcc-std()-X",
             "fBodyAcc-std()-Y",
             "fBodyAcc-std()-Z",
             "fBodyAccJerk-mean()-X",
             "fBodyAccJerk-mean()-Y",
             "fBodyAccJerk-mean()-Z",
             "fBodyAccJerk-std()-X",
             "fBodyAccJerk-std()-Y",
             "fBodyAccJerk-std()-Z",
             "fBodyGyro-mean()-X",
             "fBodyGyro-mean()-Y",
             "fBodyGyro-mean()-Z",
             "fBodyGyro-std()-X",
             "fBodyGyro-std()-Y",
             "fBodyGyro-std()-Z",
             "fBodyAccMag-mean()",
             "fBodyAccMag-std()",
             "fBodyBodyAccJerkMag-mean()",
             "fBodyBodyAccJerkMag-std()",
             "fBodyBodyGyroMag-mean()",
            "fBodyBodyGyroMag-std()",
             "fBodyBodyGyroJerkMag-mean()",
             "fBodyBodyGyroJerkMag-std()",
             "angle(tBodyAccMean,gravity)",
             "angle(tBodyAccJerkMean),gravityMean)",
             "angle(tBodyGyroMean,gravityMean)",
             "angle(tBodyGyroJerkMean,gravityMean)",
             "angle(X,gravityMean)",
             "angle(Y,gravityMean)",
             "angle(Z,gravityMean)")]

Add correct activity labels to the consolidated table. Merge activity labels by linking activity (numeric value) and activity label.
Mergeddata3<-merge(Mergeddata2, activity_labels, by.x="activity", by.y = "V1")

Add the column name for activity labels
colnames(Mergeddata3)[colnames(Mergeddata3)=="V2"]<-"activitylabel"

Check for NA values
any(is.na(Mergeddata3))


##Creates an independent tidy data set w/the average of each variable for each activity & each subject
AveVariablebySubjectActivity<-Mergeddata3%.%
      group_by(subject,activitylabel)%.%
      summarise("avg-tBodyAcc-mean-X"=mean(Mergeddata3$"tBodyAcc-mean()-X"),
                "avg-tBodyAcc-mean-Y"=mean(Mergeddata3$"tBodyAcc-mean()-Y"),
                "avg-tBodyAcc-mean-Z"=mean(Mergeddata3$"tBodyAcc-mean()-Z"),
                "avg-tBodyAcc-std-X"=mean(Mergeddata3$"tBodyAcc-std()-X"),
                "avg-tBodyAcc-std-Y"=mean(Mergeddata3$"tBodyAcc-std()-Y"),
                "avg-tBodyAcc-std-Z"=mean(Mergeddata3$"tBodyAcc-std()-Z"),
                "avg-tGravityAcc-mean-X"=mean(Mergeddata3$"tGravityAcc-mean()-X"),
                "avg-tGravityAcc-mean-Y"=mean(Mergeddata3$"tGravityAcc-mean()-Y"),
                "avg-tGravityAcc-mean-Z"=mean(Mergeddata3$"tGravityAcc-mean()-Z"),
                "avg-tGravityAcc-std-X"=mean(Mergeddata3$"tGravityAcc-std()-X"),
                "avg-tGravityAcc-std-Y"=mean(Mergeddata3$"tGravityAcc-std()-Y"),
                "avg-tGravityAcc-std-Z"=mean(Mergeddata3$"tGravityAcc-std()-Z"),
                "avg-tBodyAccJerk-mean-X"=mean(Mergeddata3$"tBodyAccJerk-mean()-X"),
                "avg-tBodyAccJerk-mean-Y"=mean(Mergeddata3$"tBodyAccJerk-mean()-Y"),
                "avg-tBodyAccJerk-mean-Z"=mean(Mergeddata3$"tBodyAccJerk-mean()-Z"),
                "avg-tBodyAccJerk-std-X"=mean(Mergeddata3$"tBodyAccJerk-std()-X"),
                "avg-tBodyAccJerk-std-Y"=mean(Mergeddata3$"tBodyAccJerk-std()-Y"),
                "avg-tBodyAccJerk-std-Z"=mean(Mergeddata3$"tBodyAccJerk-std()-Z"),
                "avg-tBodyGyro-mean-X"=mean(Mergeddata3$"tBodyGyro-mean()-X"),
                "avg-tBodyGyro-mean-Y"=mean(Mergeddata3$"tBodyGyro-mean()-Y"),
                "avg-tBodyGyro-mean-Z"=mean(Mergeddata3$"tBodyGyro-mean()-Z"),
                "avg-tBodyGyro-std-X"=mean(Mergeddata3$"tBodyGyro-std()-X"),
                "avg-tBodyGyro-std-Y"=mean(Mergeddata3$"tBodyGyro-std()-Y"),
                "avg-tBodyGyro-std-Z"=mean(Mergeddata3$"tBodyGyro-std()-Z"),
                "avg-tBodyGyroJerk-mean-X"=mean(Mergeddata3$"tBodyGyroJerk-mean()-X"),
                "avg-tBodyGyroJerk-mean-Y"=mean(Mergeddata3$"tBodyGyroJerk-mean()-Y"),
                "avg-tBodyGyroJerk-mean-Z"=mean(Mergeddata3$"tBodyGyroJerk-mean()-Z"),
                "avg-tBodyGyroJerk-std-X"=mean(Mergeddata3$"tBodyGyroJerk-std()-X"),
                "avg-tBodyGyroJerk-std-Y"=mean(Mergeddata3$"tBodyGyroJerk-std()-Y"),
                "avg-tBodyGyroJerk-std-Z"=mean(Mergeddata3$"tBodyGyroJerk-std()-Z"),
                "avg-tBodyAccMag-mean"=mean(Mergeddata3$"tBodyAccMag-mean()"),
                "avg-tBodyAccMag-std"=mean(Mergeddata3$"tBodyAccMag-std()"),
                "avg-tGravityAccMag-mean"=mean(Mergeddata3$"tGravityAccMag-mean()"),
                "avg-tGravityAccMag-std"=mean(Mergeddata3$"tGravityAccMag-std()"),
                "avg-tBodyAccJerkMag-mean"=mean(Mergeddata3$"tBodyAccJerkMag-mean()"),
                "avg-tBodyAccJerkMag-std"=mean(Mergeddata3$"tBodyAccJerkMag-std()"),
                "avg-tBodyGyroMag-mean"=mean(Mergeddata3$"tBodyGyroMag-mean()"),
                "avg-tBodyGyroMag-std"=mean(Mergeddata3$"tBodyGyroMag-std()"),
                "avg-tBodyGyroJerkMag-mean"=mean(Mergeddata3$"tBodyGyroJerkMag-mean()"),
                "avg-tBodyGyroJerkMag-std"=mean(Mergeddata3$"tBodyGyroJerkMag-std()"),
                "avg-fBodyAcc-mean-X"=mean(Mergeddata3$"fBodyAcc-mean()-X"),
                "avg-fBodyAcc-mean-Y"=mean(Mergeddata3$"fBodyAcc-mean()-Y"),
                "avg-fBodyAcc-mean-Z"=mean(Mergeddata3$"fBodyAcc-mean()-Z"),
                "avg-fBodyAcc-std-X"=mean(Mergeddata3$"fBodyAcc-std()-X"),
                "avg-fBodyAcc-std-Y"=mean(Mergeddata3$"fBodyAcc-std()-Y"),
                "avg-fBodyAcc-std-Z"=mean(Mergeddata3$"fBodyAcc-std()-Z"),
                "avg-fBodyAccJerk-mean-X"=mean(Mergeddata3$"fBodyAccJerk-mean()-X"),
                "avg-fBodyAccJerk-mean-Y"=mean(Mergeddata3$"fBodyAccJerk-mean()-Y"),
                "avg-fBodyAccJerk-mean-Z"=mean(Mergeddata3$"fBodyAccJerk-mean()-Z"),
                "avg-fBodyAccJerk-std-X"=mean(Mergeddata3$"fBodyAccJerk-std()-X"),
                "avg-fBodyAccJerk-std-Y"=mean(Mergeddata3$"fBodyAccJerk-std()-Y"),
                "avg-fBodyAccJerk-std-Z"=mean(Mergeddata3$"fBodyAccJerk-std()-Z"),
                "avg-fBodyGyro-mean-X"=mean(Mergeddata3$"fBodyGyro-mean()-X"),
                "avg-fBodyGyro-mean-Y"=mean(Mergeddata3$"fBodyGyro-mean()-Y"),
                "avg-fBodyGyro-mean-Z"=mean(Mergeddata3$"fBodyGyro-mean()-Z"),
                "avg-fBodyGyro-std-X"=mean(Mergeddata3$"fBodyGyro-std()-X"),
                "avg-fBodyGyro-std-Y"=mean(Mergeddata3$"fBodyGyro-std()-Y"),
                "avg-fBodyGyro-std-Z"=mean(Mergeddata3$"fBodyGyro-std()-Z"),
                "avg-fBodyAccMag-mean"=mean(Mergeddata3$"fBodyAccMag-mean()"),
                "avg-fBodyAccMag-std"=mean(Mergeddata3$"fBodyAccMag-std()"),
                "avg-fBodyBodyAccJerkMag-mean"=mean(Mergeddata3$"fBodyBodyAccJerkMag-mean()"),
                "avg-fBodyBodyAccJerkMag-std"=mean(Mergeddata3$"fBodyBodyAccJerkMag-std()"),
                "avg-fBodyBodyGyroMag-mean"=mean(Mergeddata3$"fBodyBodyGyroMag-mean()"),
                "avg-fBodyBodyGyroMag-std"=mean(Mergeddata3$"fBodyBodyGyroMag-std()"),
                "avg-fBodyBodyGyroJerkMag-mean"=mean(Mergeddata3$"fBodyBodyGyroJerkMag-mean()"),
                "avg-fBodyBodyGyroJerkMag-std"=mean(Mergeddata3$"fBodyBodyGyroJerkMag-std()"),
                "avg-angle(tBodyAccMeangravity)"=mean(Mergeddata3$"angle(tBodyAccMeangravity)"),
                "avg-angle(tBodyAccJerkMean)gravityMean)"=mean(Mergeddata3$"angle(tBodyAccJerkMean)gravityMean)"),
                "avg-angle(tBodyGyroMean,gravityMean)"=mean(Mergeddata3$"angle(tBodyGyroMean,gravityMean)"),
                "avg-angle(tBodyGyroJerkMean,gravityMean)"=mean(Mergeddata3$"angle(tBodyGyroJerkMean,gravityMean)"),
                "avg-angle(X,gravityMean)"=mean(Mergeddata3$"angle(X,gravityMean)"),
                "avg-angle(Y,gravityMean)"=mean(Mergeddata3$"angle(Y,gravityMean)"),
                "avg-angle(Z,gravityMean)"=mean(Mergeddata3$"angle(Z,gravityMean)")
      )

Take a look at/review the layout & data
head(AveVariablebySubjectActivity)
            
Save the table from prior step "AveVariablebySubjectActivity" to a text file for upload to Coursera
write.table(x=AveVariablebySubjectActivity, file="./TidyData.txt", sep="\t")


##About the Study
Data for this project comes from the following study:
One of the most exciting areas in all of data science right now is wearable computing.. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 
Data for the project was gathered from

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
Experiment
The dataset was built from a recording of 30 subjects performing various activities of daily life.  The subjects carried a waist-mounted smartphone with embedded inertial sensors to obtain/record data surrounding these activities.  The data was labeled:  Human Activity Recognition data.
Data Set Characteristics: Multivariate, time-series
Number of Instances: 10,299
Number of Attributes: 561
Date of Recordings (donated): 12-10-2012
Associated Tasts: Classification, Clustering
Missing Values: N/A
Number of Web Hits: 94,658

##Data Set Information:
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. 

Attribute Information:
For each record in the dataset it is provided: 
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration. 
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

##Selected Variables
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 
Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 
Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 
These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.
tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

The set of variables that were estimated from these signals are: 
mean(): Mean value
std(): Standard deviation
mad(): Median absolute deviation 
max(): Largest value in array
min(): Smallest value in array
sma(): Signal magnitude area
energy(): Energy measure. Sum of the squares divided by the number of values. 
iqr(): Interquartile range 
entropy(): Signal entropy
arCoeff(): Autorregresion coefficients with Burg order equal to 4
correlation(): correlation coefficient between two signals
maxInds(): index of the frequency component with largest magnitude
meanFreq(): Weighted average of the frequency components to obtain a mean frequency
skewness(): skewness of the frequency domain signal 
kurtosis(): kurtosis of the frequency domain signal 
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
angle(): Angle between to vectors.
Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:
gravityMean
tBodyAccMean
tBodyAccJerkMean
tBodyGyroMean
tBodyGyroJerkMean
The complete list of variables of each feature vector is available in 'features.txt'Activity Labels
1.	WALKING
2.	WALKING_UPSTAIRS
3.	WALKING_DOWNSTAIRS
4.	SITTING
5.	STANDING
6.	LAYING
