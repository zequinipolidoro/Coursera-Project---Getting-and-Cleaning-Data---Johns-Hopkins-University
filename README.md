# Coursera-Project---Getting-and-Cleaning-Data---Johns-Hopkins-University
This project is designed to collect, work with and cleaning data sets in R.
Licence: CC0 1.0

## Project Structure
* `data/`: Raw data and metadata, from Human Activity Recognition database, was downloaded as a .zip folder at  
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip. Other details are present at: https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones.
* `R/`: R file presents the used R scripts and respective outputs.

## Requirements & Installation
Required package: dplyr. 
R version and IDE used to run this code: 4.5.1/R Studio.

```R
# Open your R console and run:
install.packages("dplyr")
library(dplyr)
```

## How to Run the Analysis
1. Clone the repository.
2. Open the ProjectCoursera.rmd file in RStudio.
3. Run the chunk codes in this file (changing lines containing file paths as necessary).

# Expected Outputs
* Merged and ordered training and testing datasets
* Summary of means and SDs for each variable as a new dataframe.
* Tidy table with calculated variables' means and SDs for each subject and for each activity.
* A .txt file to be exported presenting this tidy table.
