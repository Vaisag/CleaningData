# CleaningData
Body Movement Analysis 

The objective of the function run_analysis is to fulfill the following five things
* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Algorithm

* Reads the train and test datasets and merges the data on to mergedData variable
* Reads the label details to get the activity numbers which the subjects performed, match it with the activity_labels using ActivityFun function and merge them on to mergedLabel
* Takes the data from the columns which has 'mean' and 'std' present in it and save it to mergedMean and mergedStd respectively
* Takes the numbers of columns which has 'mean' and 'std' in it and save it in mergedMeanColNums and mergedStdColNums respectively 
* Assigns column names to this mergedMean and mergedStd tables to mergedMeanColNames and mergedStdColNames respectively using the nameFun function
* Merges all the data from the mergedSubject, mergedLabel and mergedData into allMergedData
* Creates a new dataset tidyDfBoth using the aggregate function to get the average of each variable for each activity and each subject

# How to Run the script

* Download the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
* Set the downloaded path as working directory
* Source the code and run the function by calling run_analysis()
