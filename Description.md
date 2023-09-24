#Introduction to databases with SQLite

## Importing of Datasetes: imported packages 
- First imported through pandas the two datasets (1 csv, 1 json) of hospital records provided. ```import pandas as pd```
- Then after having the two datasets, some basic exploratory analysis was done for each
- Handling Missing Values:
   - The NaN values were replaced with the mean for the numerical columns
   - The NaN values were replaced with the mode for the categorical columns
   - As a last checking method for any missing values the missing values percentage was calculated to provide an overview of both whole datasets
- Then ```.describe``` was used to provide an analytical overview of the mean, std, min, max for each numerical column
- For the categorical columns the frequency counts were calculated through a loop command and a dictionary to store the data.
- These analysis steps were repeated for the second dataset imported (json file).

## SQLite Database Setup:

