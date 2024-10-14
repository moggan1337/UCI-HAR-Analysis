# UCI-HAR-Analysis

## Human Activity Recognition Using Smartphones - Data Cleaning Project
"Getting and Cleaning Data" Course Project.

## Files
README.md: This documentation explains the project and how to use the scripts.
CodeBook.md: Describes the variables, data, and processes used for cleaning up the data.
run_analysis.R: A script that cleans the data and creates one single tidy dataset.
tidy_data.txt: The output resulting from the R script, containing the tidy dataset following proper naming conventions.

## Running the Analysis
Download the run_analysis.R script to your R working directory.
Run this script in R or RStudio.
The script reads the dataset, downloads it, cleans up surplus items, and creates a tidy dataset. You'll find the tidy_data.txt file in your working directory.

## Dependencies
The script requires the dplyr and tidyr libraries. If not already installed, it will try to install them.
