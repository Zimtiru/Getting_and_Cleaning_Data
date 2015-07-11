<h4> Getting and Cleaning Data course project</h4>

Downlad the data for the project from  https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

setwd("/Users/anteneh/Documents/COURSERA/Gettingandcleaningdata/Project_trial/data/UCI HAR Dataset")

filedownloaded <- "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"

download.file(filedownloaded,destfile="Dataset.zip",method="curl")

unzip(zipfile="Dataset.zip")

This is the course project for the Getting and Cleaning Data Coursera course. The R script, run_analysis.R, does the following:

-Download the dataset in the working directory
-Unzip the dataset in the working directory
-Load the activity and feature info
-Loads both the training and test datasets, keeping those columns which reflect a mean or standard deviation only.
-Loads the activity and subject data for each dataset and merges those columns with the dataset
-Merges these datasets
-Converts the activity and subject columns into factors
-Creates a tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

Finally we get the tidydata.txt
