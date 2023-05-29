# Read: Class 12
# Pandas

**Reading Questions :**
1. The purpose of Pandas is to simplify and accelerate the data analysis and manipulation process. 
  It offers a wide range of functionalities that allow you to clean, transform, explore, and analyze data efficiently.
 
 **some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?**
 * Data Import/Export: Pandas provides functions to read data from various file formats such as CSV, Excel, SQL databases, and more. This allows you to easily load data into a DataFrame for further analysis.
 * Data Inspection: You can use functions like head(), tail(), info(), and describe() to get a quick overview of the data. These functions help you understand the structure of the data, check for missing values, and get summary statistics.
 * Data Selection and Filtering: Pandas allows you to select specific columns or rows from a DataFrame using indexing and slicing operations. You can also filter data based on conditions, such as selecting rows where a certain column meets a specific criteria. These operations enable you to focus on relevant subsets of the data for further analysis.
 * Data Manipulation: Pandas provides numerous functions for manipulating data. You can create new columns, rename columns, drop columns or rows, sort data, perform arithmetic operations between columns, and more. These operations help transform and reshape the data to suit your analysis needs.
 * Missing Data Handling: Pandas offers tools for identifying and handling missing data. You can detect missing values, drop rows or columns with missing values, or fill missing values with appropriate values, such as the mean or median. These operations ensure that missing data does not hinder your analysis.
 * Grouping and Aggregating: Pandas allows you to group data based on one or more columns and apply aggregate functions like sum, mean, count, etc. This is particularly useful for generating insights from categorical variables or performing calculations on subsets of data.
 * Data Merging and Joining: With Pandas, you can combine multiple DataFrames based on common columns using functions like merge() and join(). This helps in combining related data from different sources into a single DataFrame for comprehensive analysis.
 * Data Visualization: Pandas integrates with popular data visualization libraries like Matplotlib and Seaborn, enabling you to easily create visualizations such as line plots, bar charts, histograms, scatter plots, and more. Data visualization aids in understanding patterns, trends, and relationships within the data.
 
2. The primary data structures in Pandas are the Series and DataFrame
  
**Series:**

* A Series is a one-dimensional labeled array that can hold any data type.
* It is similar to a column in a spreadsheet or a single column of data in a database.
* Each element in a Series has a unique label called an index.
* Series is useful for handling data that can be represented as a single column or a single feature.
Use cases: Time series data, sensor readings, financial data, representing a single variable.

**DataFrame:**

* A DataFrame is a two-dimensional labeled data structure that can hold data of different types in columns.
* It is similar to a table in a relational database or a spreadsheet with rows and columns.
* DataFrame allows for easy indexing, selection, and manipulation of data.
* It provides a powerful way to handle structured data with multiple variables and observations.
Use cases: Structured data with multiple variables, data cleaning, data exploration, data analysis, merging and joining datasets.

3. 
* Import the Pandas library:
```python
import pandas as pd
```
* Choose the file format and locate the dataset file on your system.
* Use the appropriate Pandas function to read the dataset file and create a DataFrame. 
*  some common file formats and the corresponding Pandas functions to read them:
  * df = pd.read_csv('data.csv')
  * df = pd.read_excel('data.xlsx', sheet_name='Sheet1')
  * df = pd.read_json('data.json')


## Things I want to know more about
panda library








## Bookmark

df = pd.DataFrame(data, columns=['col1', 'col2', ...])

/////////////

df = pd.read_csv('data.csv')
df = pd.read_excel('data.xlsx', sheet_name='Sheet1')

///////////

df.head()       # View the first few rows
df.tail()       # View the last few rows
df.info()       # Summary information about the DataFrame
df.describe()   # Statistical summary of the data

//////////////

df.head()       # View the first few rows
df.tail()       # View the last few rows
df.info()       # Summary information about the DataFrame
df.describe()   # Statistical summary of the data

///////////////

df['col']                   # Select a single column
df[['col1', 'col2']]        # Select multiple columns
df.loc[row_label]           # Select rows by label
df.iloc[row_index]          # Select rows by index
df[df['col'] > 5]           # Filter rows based on a condition

/////////////////

df['new_col'] = df['col1'] + df['col2']     # Create a new column
df.drop('col', axis=1, inplace=True)        # Drop a column
df.rename(columns={'old_col': 'new_col'}, inplace=True)  # Rename a column
df.sort_values('col', ascending=False, inplace=True)    # Sort the DataFrame

/////////////////

df.isnull()                 # Check for missing values
df.dropna()                 # Drop rows with missing values
df.fillna(value)            # Fill missing values with a specified value

//////////////////

df.groupby('col').mean()     # Group by a column and calculate mean
df.groupby(['col1', 'col2']).sum()   # Group by multiple columns and calculate sum

/////////////////

merged_df = pd.merge(df1, df2, on='col')    # Merge two DataFrames based on a column

////////////////

df.plot()                   # Plot the data
df.plot(kind='bar')         # Plot a bar chart
df.plot(kind='hist')        # Plot a histogram






