#Code Book for Getting and Cleaning Data Course Project (run_analysis.R)

##Source
The UCI HAR data set can be accessed at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
The .zip file needs to be extracted in order to access all the required files.
Please note : All the files located in the 'Internal Signals' folder were ignored for this course project

##Brief Summary of data
30 volunteers performed 6 different activities while wearing a smartphone. The smartphone captured various data about their movements. The goal of this project is to create a tidy data set that contains data merged from test and train data files.

Here is a list of the files used in this course project:
1. X_train.txt 2. y_train.txt 3. subject_train.txt 4. X_test.txt 5. y_test.txt 6. subject_test.txt 7. activity_labels.txt 8. features.txt

##Steps involved in script
* Read the files from all the .txt files mentioned above
* Make substitutions in the features data set to facilitate the easy identification of columns housing mean and standard deviation data
* Combine the testing and training data sets
* Using grep(), identify the columns we want from the features data set
* Subset the columns we want from the features data set
* Subset these columns from the combined data set of training and testing data sets in order to remove unnecessary columns
* Add the activity and subject columns to the merged data set
* Aggregate this data set and write it to a file called "tidy.txt"
