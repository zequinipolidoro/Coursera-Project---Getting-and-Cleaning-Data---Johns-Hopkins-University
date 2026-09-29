# Code Book
This document describes the original data and variables from the Human Activity Recognition database as well as the transformations to get clean datasets.  

## Raw Data
* 561 variables in original files related to accelerometer and gyroscope signals. 
* ID subjects from 1 to 30.
* 6 different activity levels (walking, walking downstairs, walking upstairs, sitting, standing, laying) presented as numerical factors.
* Training and testing datasets splitted in different .txt files.

## Transformations 
* Reading the list of variable names present in .txt file and getting them into a chr vector.
* Merging of the training dataset (three files) by cbind and renaming the variable names considering the chr vector.
* Merging of the testing dataset (three files) by cbind and renaming the variable names considering the chr vector.
* Combining the merged training and testing datasets by rbind.
* Cleaning of duplicated variable columns in the merged dataset.
* Sorting of this merged dataset based on the order of Subject IDs.
* Converting the numerical factors in the Activity column to character factors
(walking, walking downstairs, walking upstairs, sitting, standing, laying).
* Getting a new dataframe combining the 66 columns representing the means and SDs for each variable as well as the Subject ID and activity.
* Getting a new dataframe presenting the average values of these 66 columns grouped by Subject and Activity levels (30*6 = 180 combinations/rows).
* Getting a .txt tidy table of the previous dataframe.
