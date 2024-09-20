# python-data-manipulation

The sample_data_for_assignment.json file contains 2 keys namely cols and data. Write a
program to load this data to MySQL (should be installed locally) table (table_name:
json_to_sql_table) under a database. After loading the data do the following -

1. unload the data from MySQL to pandas dataframe
2. write a program to display all data under their respective column name as a pandas dataframe
3. write a program to change all email address to have the format - abc@gmail.com (note the ending should be gmail.com
4. 4. The values for "postalZip" doesn't have same type of data (some are string, some are int, some are alpha numeric). Write a program to convert all values to int. In case of alpha numeric remove the letters and keep only the numbers and convert it to int.
5. write a separate function which take input data as values under the column name "phone" and processes it to return equivalent ASCII char of the value taken 2 at a time from left to right. Considering the value should be in between 65 to 99. If two-digit number is less than 65 replace it with O (O for Orange)
6. For example -
example1 : (816) 530-4269 should be converted to 8165304269 and taking two digit at a time, finding the ASCII equivalent char
81 - Q
65 - A
30 - O
42 - O
69 - E
So the function should return QAOOE for the input (816) 530-4269 or 8165304269 and replace
it in the dataframe.
example2 : 1-811-920-9732 should be converted to 18119209732 and taking two digit at a time from left to right, finding the ASCII equivalent char
18 - O
11 - O
92 - \
09 - O
73 – I
Ignore the last digit 2 as it is single.
So the function should return OO\OI for the input 1-811-920-9732 or 18119209732 and replace it in the dataframe.

At last rename the column "phone" to "coded_phone_number" in the dataframe
