# Pandas - Find Excel Date Errors

## INTRO
Often with spreadsheets, you'll have incorrectly filled in date columns - empty strings, strings and integers or invalid dates. 

This tool shows how Python and Pandas can be used to take a set of data from excel or a csv file and create a new column saing if the data is valid is True or False.

The scipt then filters the data and creates a new file of all rows with invalid date information.

## GETTING STARTED
### 1-generate-employee-data.ipynb
- Run this file first.
- This creates a 2000 row employee data file with names and date started.
- Numpy is used to generate employee names and random dates into the date started column.
- It inserts random errors such as wrong data types and empty strings into the date started column.
- It saves the data file to be used in file 2...

### 2-create-invalid-dates-report.ipynb
- It opens the file generated above.
- Empty strings are converted to 'NaN' values, so an action in this file is to convert all 'NaN' values to a string (Assessing if a string or int is a date type is easier than with 'NaN' types.)
- It creates a new column called 'Valid Start Date' and asesses all fields from the 'Date Started' column and inserts a boolean into the new 'Valid Start Date' declaring if the date is valid.
- A new file is created highlighting the row numbers which have dates that need fixing.

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

