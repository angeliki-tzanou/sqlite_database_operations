#Introduction to databases with SQLite

## Importing of Datasetes: imported packages 
- First imported through pandas the two datasets of hospital records provided. ```import pandas as pd```
- Then after having the two datasets, some basic exploratory analysis was done for each
- Handling Missing Values:
   - The NaN values were replaced with the mean for the numerical columns
   - The NaN values were replaced with the mode for the categorical columns
- Then ```.describe``` was used to provide an analytical overview of the mean, std, min, max for each numerical column
- For the categorical columns the frequency counts were calculated
- These analysis steps were repeated for the second dataset imported of the json file.
