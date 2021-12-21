# Pandas - Find Excel Date Errors

## INTRO
Often with spreadsheets, you'll have incorrectly filled in date columns - empty strings, strings and integers or invalid dates. 

This tool shows how Python and Pandas can be used to take a set of data from excel or a csv file and create a new column saing if the data is valid is True or False.

The scipt then filters the data and creates a new file of all rows with invalid date information.

## GETTING STARTED
The first file generates a 2000 row dataset containing string columns and a date column with an employee start date using Numpy and Pandas. 

Some of the date columns in the file are overriden by strings, empty strings and integers.

The second file is the tool that opens the first file, finds all NaN data, finds all integers and strings and creates a new column called 'Valid Start Date' with True or False for the 'Date Started' column.

A new file containing the row numbers of the date errors is created and can be sent to a team member for correcton.

## SKILLS COVERED
Packages and methods
- Numpy
- Pandas
- pd.read_csv(), pd.read_excel(), pd.to_csv(), pd.to_excel()
- pd.dtypes
- datetime()
- pd.fillna()
- np.random.randint()
- pd.to_datetime()
- df.apply()

General
- filtering data in Pandas
- creating new columns by filtering data in other columns
- populating columns with list
- checking data types in pandas
- replacing NaN values
- deleteing rows in pandas

