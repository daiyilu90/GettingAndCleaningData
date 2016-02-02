data source:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

following files are useing in run_analysis.R to complete this project

Y_test.txt: activity info for testing data
Y_train.txt: activity info for training data
subject_test.txt: subject info for testing data
subject_train.txt: subject info for training data
X_test.txt: features info for testing data
X_train.txt: features info for trianing data
features.txt: features names file
activity_labels.txt: activity label file

run_analysis.R Process:

#1 download file
#2 unzip the file
#3 save upzip file and get the list of files 
#4 read all required files (see list above)
#5 adding column names to all files
#6 column combine activity, subject and features files and row combine test and train files
#7 Only keep measurements on the mean and standard deviation by searching "mean" or "sd" in the column names.
#8 merge the activity labels file to repalce activity with activity descriptions. 
#9 sorting and reorder column  by subject, activity description
#10 Remove redudant symbols in variable names and make them readable 
#11 export table to cleandata.txt
#12 calculate the average of each variables on each activity and subject. Export to tidydata.txt

final output files:
cleandata.txt combined several pieces datasets with files: subject, activity, and measurements on the mean and standard deviation for each measurement. All variables names are descriptive and appropriately labeled. 
tidydata.txt is independent tidy data set with the average of each variable for each activity and each subject.