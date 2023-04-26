# long-term-occupational-prediction

This is a Python code that reads a CSV file named "Long-Term_Occupational_Employment_Projections.csv" and performs data cleaning and preprocessing operations on the data.

First, it imports the required libraries such as Pandas, NumPy, Matplotlib, and Seaborn.

Then, it accesses the CSV file and converts it into a Pandas dataframe. It also prints the shape of the dataframe, the first 10 rows, and information about the dataframe such as column names, data types, and non-null values.

Next, it checks for the number of null values in each column using the isna() and isnull() functions and calculates the percentage of missing values per column and the percentage of total missing values. It also sets the maximum number of columns to display in the output to 18 and drops the first row of the dataframe, which contains the total record.

After that, it fills the missing values in the "Job Training" column by replacing the NaN and None values with "No Training". It also fills the missing values in the "Entry Level Education" column by replacing the NaN values with "No information available".

Then, it calculates the median values of non-zero hourly and annual wages records for each SOC level (1 to 4) and replaces all the missing or zero hourly and annual wages values with these median values.

Finally, it fills the missing values in the "Work Experience" column based on the SOC level.
