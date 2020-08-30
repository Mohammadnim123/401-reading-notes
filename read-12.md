# Pandas Library

![p](https://miro.medium.com/max/481/1*cxfqR8NAj8HGal8CVOZ7hg.png)

>The Pandas library is one of the most preferred tools for data scientists to do data manipulation and analysis, next to matplotlib for data visualization and NumPy, the fundamental library for scientific computing in Python on which Pandas was built. 

>The fast, flexible, and expressive Pandas data structures are designed to make real-world data analysis significantly easier, but this might not be immediately the case for those who are just getting started with it. Exactly because there is so much functionality built into this package that the options are overwhelming.

**Importing Data**
**Use these commands to import data from a variety of different sources and format**

`pd.read_csv(filename) `| From a CSV file

`pd.read_table(filename) `| From a delimited text file (like TSV)

`pd.read_excel(filename) `| From an Excel file

`pd.read_sql(query, connection_object) `| Read from a SQL table/database

`pd.read_json(json_string) `| Read from a JSON formatted string, URL or file.

`pd.read_html(url) `| Parses an html URL, string or file and extracts tables to a list of dataframes

`pd.read_clipboard() `| Takes the contents of your clipboard and passes it to read_table()

`pd.DataFrame(dict) `| From a dict, keys for columns names, values for data as lists

**Exporting Data**
**Use these commands to export a DataFrame to CSV, .xlsx, SQL, or JSON.**

`df.to_csv(filename) `| Write to a CSV file

`df.to_excel(filename) `| Write to an Excel file

`df.to_sql(table_name, connection_object) `| Write to a SQL table

`df.to_json(filename) `| Write to a file in JSON format


**Join/Combine**
**Use these commands to combine multiple dataframes into a single one.**

`df1.append(df2) `| Add the rows in df1 to the end of df2 (columns should be identical)

`pd.concat([df1, df2],axis=1) `| Add the columns in df1 to the end of df2 (rows should be identical)

`df1.join(df2,on=col1,how='inner') `| SQL-style join the columns in df1 with the columns on df2 where the rows for col have identical values. 'how' can be one of 'left', 'right', 'outer', 'inner'

**Statistics**
**Use these commands to perform various statistical tests. (These can all be applied to a series as well.)**


`df.describe() `| Summary statistics for numerical columns

`df.mean() `| Returns the mean of all columns

`df.corr() `| Returns the correlation between columns in a DataFrame

`df.count() `| Returns the number of non-null values in each DataFrame column

`df.max() `| Returns the highest value in each column

`df.min() `| Returns the lowest value in each column

`df.median() `| Returns the median of each column

`df.std() `| Returns the standard deviation of each column