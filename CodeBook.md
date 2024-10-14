# Code Book

This document explains the variables, data, and steps taken to clean and process the Human Activity Recognition Using Smartphones dataset.

## Data Source

The data was sourced from the UCI Machine Learning Repository:
http://https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones

## Dataset Overview

The dataset was collected through experiments involving 30 volunteers, aged between 19 and 48.
Each participant completed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING and LAYING) while carrying a smartphone (Samsung Galaxy S II) on their waist. 
The phone's accelerometer and gyroscope recorded 3-axis linear acceleration and angular velocity data at a consistent 50hz frequency.

## Variables

The cleaned dataset contains the following key variables:
-`subject`: A unique identifier for each volunteer (1-30)
-`activity`: The specific activity performed (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING and LAYING).
Features: 66 variables representing the mean and standard deviation measurements for each subject and activity. 
These features capture both time-domain and frequency domain signals from the accelerometer and gyroscope.

## Data Transformations

The following transformations were applied to clean and organize the data:
1. Combined the training and test sets into one unified dataset.
2. Filtered the data to include only the mean and standard deviation measurements.
3. Replaced activity codes with descriptive names for easier understanding.
4. Labeled all variables using clear and descriptive names.
5. Created a new tidy dataset that averaged each variable by activity and subject.

## Data Cleaning Process

1. Loaded training, test data, feature names and activity labels.
2. Merged the training and test sets.
3. Assigned proper column names to the merged dataset.
4. Extracted only the mean and standard deviation measurements.
5. Substituted activity IDs with their descriptive names.
6. Renamed columns to more intuitive labels (e.g, 't' became 'Time', 'Acc' became 'Accelerometer').
7. Generated a tidy dataset with the average of each variable for every activity and subject.
8. Saved the tidy dataset as 'tidy_data.txt'.
