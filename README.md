### Machine Learning
Machine Learning (ML) is a subset of Artificial Intelligence that enables computers to learn patterns from data and make predictions or decisions without being explicitly programmed.

ML workflows involve:
• Data Manipulation & Analysis: Handling raw data using tools like Pandas and NumPy.

• Data Visualization: Visualizing relationships using Matplotlib, and plotting using different plot types.

• Modelling & Evaluation: 	Applying algorithms via Scikit-learn to make predictions and measure performance.

• Deployment: Integrating the model into real-world applications.

• Notebooks: Jupyter Notebooks

•	Jupyter Notebooks provide an interactive environment for writing and running Python code, visualizing results, and documenting experiments in one place.)
### Data Manipulation & Analysis: Pandas
1. What are pandas?

•	Pandas builds on NumPy to provide powerful data structures i.e., Series and DataFrames, designed for analyzing structured data.

•	Ideal for Loading and cleaning data from CSV, Excel, JSON, etc.

•	Exploratory data analysis (EDA) using filtering, grouping, and aggregation

•	Handling missing values and reshaping datasets.

•	Merging and joining data from multiple sources.
### For this exercise ive used a car-sales data set which is in csv format, then done data manipulation and analysis by using Pandas library.
 ## Datasets
-	car-sales-DataFrame-exported.csv
-	car-sales-missing-data.csv
-	car-sales.csv
### Operations I Performed (Pandas Exercises)
•	I imported the pandas library.  
•	I created a Series containing three different colours.  
•	I viewed the Series of different colours.  
•	I created a Series containing three different car types and viewed it.  
•	I combined the Series of cars and colours into a single DataFrame.  
•	I imported the dataset **"car-sales.csv"** and converted it into a DataFrame.  
•	I exported the created DataFrame to a new `.csv` file.  
•	I identified the different data types of each column in the car sales DataFrame.  
•	I described the numerical columns in the DataFrame using the `.describe()` method.  
•	I gathered detailed information about the DataFrame using `.info()`.  
•	I created a Series of different numbers and calculated their mean.  
•	I created another Series of different numbers and calculated their sum.  
•	I listed all the column names of the car sales DataFrame.  
•	I found the total number of rows in the DataFrame using `len()`.  
•	I displayed the first 5 rows of the car sales DataFrame.  
•	I displayed the first 7 rows of the car sales DataFrame.  
•	I displayed the last 5 rows of the car sales DataFrame.  
•	I used `.loc` to select the row at index 3 of the car sales DataFrame.  
•	I used `.iloc` to select the row at position 3 of the DataFrame.  
•	I selected the `"Odometer (KM)"` column from the DataFrame.  
•	I calculated the mean of the `"Odometer (KM)"` column.  
•	I filtered and displayed the rows where the odometer reading was over 100,000 kilometers.  
•	I created a crosstab of the `"Make"` and `"Doors"` columns.  
•	I grouped the DataFrame by the `"Make"` column and found the average values for each group.  
•	I imported **Matplotlib** and created a plot of the Odometer column using `%matplotlib inline`.  
•	I created a histogram of the Odometer column using `.hist()`.  
•	I attempted to plot the Price column using `.plot()`.  
•	I removed punctuation symbols from the `"Price"` column.  
•	I verified the changes to the `"Price"` column.  
•	I removed the two extra zeros at the end of the values in the `"Price"` column.  
•	I checked the updates made to the `"Price"` column.  
•	I changed the data type of the `"Price"` column to integers.  
•	I converted all text in the `"Make"` column to lowercase.  
•	I made the lowercase transformation of the `"Make"` column permanent.  
•	I reviewed the car sales DataFrame to confirm all changes.  
•	I imported another DataFrame containing missing data from **"car-sales-missing-data.csv"**.  
•	I reviewed the newly imported DataFrame.  
•	I filled the missing values in the `"Odometer"` column with the column’s mean value, updating it inplace.  
•	I viewed the updated DataFrame to verify the changes.  
•	I removed the remaining missing data inplace.  
•	I confirmed that all missing values had been removed by viewing the DataFrame again.  
•	I created a new `"Seats"` column, assigning every row a value of 5.  
•	I created another column named `"Engine Size"` containing random values between 1.3 and 4.5.  
•	I ensured that the list of values matched the number of rows in the DataFrame.  
•	I created a new column representing the price of a car per kilometer, then viewed the updated DataFrame.  
•	I removed this last column using the `.drop()` method.  
•	I shuffled the rows of the DataFrame using `.sample()` with the `frac=1` parameter.  
•	I saved the shuffled version of the DataFrame to a new variable.  
•	I reset the indexes of the shuffled DataFrame.  
•	I converted the Odometer values from kilometers to miles using a Lambda function, then viewed the DataFrame.  
•	Finally, I changed the column title from `"Odometer (KM)"` to represent miles instead of kilometers.
### Key Syntax and Concepts Used (df = DataFrame)
• `import pandas as pd`  
  (Imported the pandas library and gave it the common alias `pd`).
  
• `df = pd.read_csv("car-sales.csv")
  (Loaded the CSV file named *car-sales.csv* into a DataFrame called `df`).
  
• `df.head()`  
  (Displayed the first five rows of the DataFrame).
  
• `df.info()`  
  (Showed summary information — number of rows, column names, data types, and memory usage).
  
• `df.describe()`  
  (Provided statistical details like mean, min, max, and standard deviation for numeric columns).
  
• `df.shape`  
  (Returned the dimensions of the DataFrame as `(rows, columns)`).
  
• `df.columns`  
  (Displayed a list of all column names in the DataFrame).
  
• `df["Make"]`  
  (Selected a single column named *Make*).
  
• `df[["Make", "Price"]]`  
  (Selected multiple columns — *Make* and *Price*).
  
• `df.loc[0]`  
  (Accessed the row with index label 0 using label-based indexing).
  
• `df.iloc[0:5]`  
  (Accessed the first five rows using position-based indexing).
  
• `df[df["Price"] > 20000]`  
  (Filtered rows where the *Price* column had values greater than 20,000).
### What Ive Learned:
•	Got an idea about Data Anlalysis and manipulation libraries and frameworks. 

•	Learned how to import/export a .csv file and creating a series/DataFrame for the gathered data.

•	I loaded and explored the car_sales.csv dataset (and the missing-data variant) with read_csv, info, and describe to understand schema and quality.

•	I created and worked with Series and DataFrames, selecting data using loc/iloc and filtering rows to answer specific questions.

•	I cleaned missing values using dropna/fillna, and engineered columns (e.g., simple arithmetic/transformations) to make the data more informative.

•	I summarized insights with groupby + agg and produced quick checks using DataFrame.plot() for distributions and relationships.

•	Finally, I exported results with to_csv to keep my processed data reproducible and ready for follow-up analysis.

• Through these exercises, I learned how to work with **pandas DataFrames and Series**, clean and manipulate data, and perform exploratory data analysis.

• These operations strengthened my understanding of how **pandas** can be used for preparing and transforming datasets before building **machine learning models**.


