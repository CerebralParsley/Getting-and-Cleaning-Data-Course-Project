# Getting-and-Cleaning-Data-Course-Project

This repository was created as a course requirement for the Module 3 Getting and Cleaning Data.

* First, download and unzip the data file into your R working directory.
* Second, download the R source code into your R working directory.
* Finally, execute R source code to generate tidy data file.

## Data description

The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects.
The variable in data Y indicates activity type the subjects performed during recording.

## Code explanation

The code combined training dataset and test dataset, and extracted partial variables to create another
dataset with the averages of each variable for each activity.

## New dataset

The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the
dataset is an average of each activity type for all subjects.

## The code written was based on the instruction of this assigment:

Read training and test dataset into R environment. Read variable names into R 
environment. Read subject index into R environment.

1. Merges the training and the test sets to create one data set. Use command rbind 
to combine training and test set
2. Extracts only the measurements on the mean and standard deviation for each
measurement. Use grep command to get column indexes for variable name contains 
"mean()" or "std()"
3. Uses descriptive activity names to name the activities in the data se. 
Convert activit labels to characters and add a new column as a factor
4. Appropriately labels the data set with descriptive variable names. Give
the selected descriptive names to variable columns
5. From the dataset in step 4, creates a second, independent tidy dataset with the
average of each variable for each activity and each subject. Use
pipeline command to create a new tidy dataset with command group_by and
summmarize_each in dplyr package
