# Introduction

This project show how apply al concepts learned in this course of Gettin And Cleaning, therefor this repository contains just one R script to merge and tidy data collected from an experiment 
that was collecting data from the accelerometers Samsung Galaxy S smartphones, the script's name is run_analisis.R

# Data source provided for this project was download from this web site

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

# Steps carried out to complete this project were:

1. Clone this repository
2. change the working directory to getting-cleaning-data-project/ folder
3. Download the data source zip file
4. Unzip the source zip file: `unzip getdata-projectfiles-UCI\ HAR\ Dataset.zip`
5. Run run_analysis.R

Corresponding commands are:

git clone https://github.com/juanguanoluisa/Proyecto
cd getting-cleaning-data-project
wget https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
unzip getdata-projectfiles-UCI\ HAR\ Dataset.zip
R run_analysis.R


# Output

run_analysis.R generates 2 files:
* tidy_data.txt: a space-delimited value file that contains mean and standard deviation for each measurements from the train and test data,
* average_data.txt: a space-delimited value file that contains tidy data set with the average of each variable for each activity and each subject

I used default params for write.table() so space-delimited, with column names, ... To read those files, use:


read.table('tidy_data.txt')
read.table('average_data')
