#Introduction to databases with SQLite

## Importing of Datasetes: imported packages 
- First imported through pandas the two datasets of hospital records provided. ```import pandas as pd```
- Then after having the two datasets, some basic exploratory analysis was done for each:
  - Handling Missing Values
   - The NaN values were replaced with the mean for the numerical columns
   - The NaN values were replaced with the mode for the categorical columns
