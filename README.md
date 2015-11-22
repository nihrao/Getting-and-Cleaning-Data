# Getting and Cleaning Data (Tidy.txt) for run_analysis.R

##Summary
This file provides an initial insight into the data files analyzed and the tidy data set produced as a part of the course project.


##Files used
Here is a list of the files used from the UCI HAR Dataset :
1. X_train.txt
2. y_train.txt
3. subject_train.txt
4. X_test.txt
5. y_test.txt
6. subject_test.txt
7. activity_labels.txt
8. features.txt

For convenience purposes, I have placed these files in a single folder which can be accessed using the syntax "dir/file_name.txt"

The features (561 of them) are unlabeled and can be found in the x_test.txt. The activity labels are in the y_test.txt file. The test subjects are in the subject_test.txt file.

##run_analysis.R
* The script merges the test and training data sets. Once the merge is complete, lables are added to only those columns that house either a mean or standard deviation data.
* The final data set, i.e. the tidy data set will be containing the means of all the columns per test subject and per activity. This tidy dataset will be written to a tab-delimited file called tidy.txt, which can also be found in this repository.
