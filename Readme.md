# COURSERA/Getting and Cleaning Data - Course Project

This is the course project for the Getting and Cleaning Data Coursera course. The meaning of the variables and other descriptions can be found in the file `CodeBook.md`.

The R script, `run_analysis.R`, does the following:

1. Download the dataset if it does not already exist in the working directory

2. Load the activity and feature info

3. From features, select only those that reflect mean and standard deviation. Eliminate from those feature-names the extra characters, such as "()" or "-" such that the final names are to be only "Mean" or "Std".

3. Load the training and test datasets and keep only those columns which contain a mean or standard deviation
   
4. Load the activity and subject data for each dataset, and merges those columns with the dataset
   
5. Merges the two above-mentioned datasets

6. Converts the `activity` and `subject` columns into factors

7. Creates a tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

8. Save the clean data set to the file `tidy.txt`.
