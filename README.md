# Data-Cleaning-FIFA21-Dataset
This is a raw and messy dataset. Data Cleaning and Transformation has been performed on this data using Python.
The following questions have been answered:

1. Do the height and weight columns have appropriate data types?
Ans: It is observed that the height and weight columns are not of the appropriate type. They are of object data type. They have been converted into float64 and int64 data types respectively. The height has been converted into centimetres for a more straightforward conversion.

2. Is it possible to separate the joined and loan date end columns into datetime format?
Ans: It is possible to directly do the same using pandas.to_datetime(fifa21.Joined) and the same for the loan date end column.

3. Is it possible to clean and transform the value, wage and release clause columns into integers?
Ans: It is possible, by using if-else statements inside for loops to remove the currency symbols and replace the 'M' and 'K' with their respective integer multiples.

4. How should one remove the newline characters from the Hits column?
Ans: It is possible by using the .replace() method inside a for loop.

5. Should one separate the Team & Contract column into separate team and contract columns?
Ans: It is advisable to separate the Team & Contract column into separate columns such as Team Name, Start Year, End Year, On Loan, Free, etc. to be a more usable and clean form of data.

6. Should one remove the stars in the performance columns?
Ans: Removing unnecessary information such as the star symbol and converting the data directly into numeric types for higher accessibility is good.
