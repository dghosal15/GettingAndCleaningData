# Steps to re-produce the requirements of the Course project of Getting and Cleaning Data

## Step 1: Downloading and Unzipping the file
   * Download the file from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
   * Unzip the folder in the Current working directory
   * Rename the folder as "data"
   * We need to ensure that the folder "data" and the "run_analysis.R" script are both in the current working directory.
   
## Step 2: Using source() to run the R script  
   * Use **source("run_analysis.R")** command to run the script in R 
   
## Step 3: The output
   * After running the script in Step-3 above, you will find two output files are generated in the current working directory
      * merged_data.txt(7.9 mb) : This text file contains a data frame called cleanedData with 10299X68 dimension.
      * tidy_dataset.txt(220 kb): This text file contains a data frame called result with 180X68 dimension.
      
## Step 4: Checking the output
   * To check the output, you can use the data <- read.table("tidy_dataset.txt") command in R to read the file  
   * Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in      total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.

### Please see the codebook.md file to find details about all variables and summaries calculated.

Thank You
   
