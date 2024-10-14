## Code Book
This document lays out the variables, data, and steps utilized for cleaning and processing the Human Activity Recognition Using Smartphones dataset.

## Data Source
The source of the data is the UCI Machine Learning Repository, and the link is http://https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones

## Dataset Description
The dataset consists of thirty participants whose ages ranged between 19 and 48. Each individual performed six activities: WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, and LAYING. In place of a traditional wearable device, participants were each given a smartphone, Samsung Galaxy S II, which they wore on their waist. The smartphone had a built-in accelerometer and gyroscope hardware that recorded 3-axial linear acceleration and 3-axial angular velocity. The data was kept at a consistent record of 50hz.

## Variables
The final clean data features of the data include: – subject: an identifier of the participant (1-30) – activity: performed task from the following WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, and LAYING – Features: This is a set of 66 variables obtained by averaging the mean and standard measurements of each subject and activity. The mean and standard deviation are extracted from the beginning 561 feature vector and account for both time and frequency domain signals obtained by the accelerometer and gyroscope.

## Data Transformation
The following are the data transformation steps taken to tidy up and structure the data:

Joined the training and test data to form a single data frame.
Filtered the data to remove the extremely high and low measurements to attain only the mean and standard deviation.
Assigned descriptive names to the activity variables for clear data comprehension.
Renamed all variables with descriptive variable names.
Finally, we generated a new tidy dataset with the average of each variable for subject and activity.
Cleaning Process
The cleaning steps taken include the following:

Load training and test data. Load feature names. Load activity names.
Merge the training and the test datasets.
Assign column names to the resultant dataset.
Extract only the measurements of the mean and standard deviation.
Label the activity variables with the separate activity labels.
Renaming the above columns to more understandable variables. E.g., the letter “t” was replaced with “Time” and “Acc” with “Accelerometer.”
Create a new tidy dataset, which comprises the average of each variable for the activity and subject.
Save the dataset as tidy_data.txt.
