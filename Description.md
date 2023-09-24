#Introduction to databases with SQLite

## Importing of Datasetes: 
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
- The one package that needed to be imported before running the needed commands was ```import sqlite3``` _(considering that the pandas package has been imported from previously)_
- Created the database by using ```conn = sqlite3.connect('___.db')``` as well as ```c = conn.cursor()```
- Then the table was created within the database through the ```c.execute``` command
- After confirming that the table has been created within the db and it returns no values since it is empty we proceed to the INSERT INTO SQL query
- We begin adding info in the created table within the database and then to view our table we can do it by using pandas read
- 
### Creating a table through the Automatic Table Creation:
- We have our loaded and corrected dataset from previously
- Then we can use ```df.to_sql``` command to load the dataset into our new table
- Lastly we can use the pandas command ```pd.read_sql``` to read the dataset through our new created table in our db
- **Committing changes and closing our dataset should be done sporadically throughout by using ```conn.commit()``` & ```conn.close()```**
