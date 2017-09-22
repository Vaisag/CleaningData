# Variable Details, data clean up and other transformations
* train - table which has X_train file's data;
* test  - table which has X_test file's data;
* trainLabel - table which has y_train file's data;
* testLabel - table which has y_test file's data;
* activity - table which has activity_labels file's data;
* subjectTrain - table which has subject_train file's data;
* subjectTest - table which has subject_test file's data;
* mergedSubject - merged table which has the all the rows and columns from subjectTrain and subjectTest
* mergedData - merged table which has the all the rows and columns from train and test
* activityNameTrain - All activity numbers in trainLabel are assigned with the activity names
* activityNameTest - All activity numbers in testLabel are assigned with the activity names
* mergedLabel - merged table which has both activityNameTrain and activityNameTest
* columnNames - table which has features file's data;
* mergedMean - mean columns data from the mergedData dataset
* mergedStd - std columns data from the mergedData dataset
* mergedMeanColNums - used as intermediate variable to get the column numbers with mean in it
* mergedStdColNums - used as intermediate variable to get the column numbers with std in it
* mergedMeanColNames - column names which has mean in it
* mergedStdColNames - column names which has std in it
* allMergedData - a merged Dataset which has all the data in the mergedSubject, mergedLabel and mergedData datasets
* tidyDfBoth - tidy dataset which has means for each variable for each subject and each activity




# Functions
* ActivityFun - assigns activity names to the activity numbers in the file
* nameFun - asssigns column names for the mean and std 
