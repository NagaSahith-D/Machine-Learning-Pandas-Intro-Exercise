Machine Learning (ML) is a subset of Artificial Intelligence that enables computers to learn patterns from data and make predictions or decisions without being explicitly programmed.
ML workflows involve:
Data Manipulation & Analysis:	 Handling raw data using tools like Pandas and NumPy.

Data Visualization: 		Visualizing relationships using Matplotlib, and plotting using different plot types.

Modelling & Evaluation: 	Applying algorithms via Scikit-learn to make predictions and measure performance

Deployment: 			Integrating the model into real-world applications.

Notebooks: 			Jupyter Notebooks
•	Jupyter Notebooks provide an interactive environment for writing and running Python code, visualizing results, and documenting experiments in one place.)

Data Manipulation & Analysis: Pandas
1. What are pandas?

•	Pandas builds on NumPy to provide powerful data structures i.e., Series and DataFrames, designed for analyzing structured data.

•	Ideal for Loading and cleaning data from CSV, Excel, JSON, etc.

•	Exploratory data analysis (EDA) using filtering, grouping, and aggregation

•	Handling missing values and reshaping datasets

•	Merging and joining data from multiple sources

## For this exercise ive used a car-sales data set which is in csv format, then done data manipulation and analysis by using Pandas library.
 ## Datasets
-	car-sales-DataFrame-exported.csv
-	car-sales-missing-data.csv
-	car-sales.csv
## Key Syntax and concepts used (df = DataFrame)
•	import pandas as pd      				##imports panda library

•	df = pd.read_csv("car-sales.csv")      		## read CSV file

•	df.head()                            			## preview top 5 rows

•	df.info()                              			## column info

•	df.describe()                          			## summary statistics

•	df.shape                               			## displays rows, columns shape

•	df.columns    					## list column names

•	df["Make"]                             			## select one column (Series)

•	df[["Make", "Price"]]                  			## select multiple columns

•	df.loc[0]                            				## select row by label/index

•	df.iloc[0:5]                           			## select first 5 rows (position)

•	df[df["Price"] > 20000]                			## boolean filtering

•	df[df["Colour"].isin(["Red", "Blue"])] 		## filter using a list


    ## What Ive Learned:
    
•	Got an idea about Data Anlalysis and manipulation libraries and frameworks. 

•	Learned how to import/export a .csv file and creating a series/DataFrame for the gathered data.

•	I loaded and explored the car_sales.csv dataset (and the missing-data variant) with read_csv, info, and describe to understand schema and quality.

•	I created and worked with Series and DataFrames, selecting data using loc/iloc and filtering rows to answer specific questions.

•	I cleaned missing values using dropna/fillna, and engineered columns (e.g., simple arithmetic/transformations) to make the data more informative.

•	I summarized insights with groupby + agg and produced quick checks using DataFrame.plot() for distributions and relationships.

•	Finally, I exported results with to_csv to keep my processed data reproducible and ready for follow-up analysis.

Steps Followed for this exercise:

# Import pandas
# Create a series of three different colours
# View the series of different colours
# Create a series of three different car types and view it
# Combine the Series of cars and colours into a DataFrame
# Import "car-sales.csv" and turn it into a DataFrame
# Export the DataFrame you created to a .csv file
# Find the different datatypes of the car data DataFrame
# Describe your current car sales DataFrame using describe()
# Get information about your DataFrame using info()
# Create a Series of different numbers and find the mean of them
# Create a Series of different numbers and find the sum of them
# List out all the column names of the car sales DataFrame
# Find the length of the car sales DataFrame
# Show the first 5 rows of the car sales DataFrame
# Show the first 7 rows of the car sales DataFrame
# Show the bottom 5 rows of the car sales DataFrame
# Use .loc to select the row at index 3 of the car sales DataFrame
# Use .iloc to select the row at position 3 of the car sales DataFrame
# Select the "Odometer (KM)" column from the car sales DataFrame
# Find the mean of the "Odometer (KM)" column in the car sales DataFrame
# Select the rows with over 100,000 kilometers on the Odometer
# Create a crosstab of the Make and Doors columns
# Group columns of the car sales DataFrame by the Make column and find the average
# Import Matplotlib and create a plot of the Odometer column
# Don't forget to use %matplotlib inline
# Create a histogram of the Odometer column using hist()
# Try to plot the Price column using plot()
# Remove the punctuation from price column
# Check the changes to the price column
# Remove the two extra zeros at the end of the price column
# Check the changes to the Price column
# Change the datatype of the Price column to integers
# Lower the strings of the Make column
# Make lowering the case of the Make column permanent
# Check the car sales DataFrame
# Import the car sales DataFrame with missing data ("../data/car-sales-missing-data.csv")
# Check out the new DataFrame
# Fill the Odometer column missing values with the mean of the column inplace
# View the car sales missing DataFrame and verify the changes
# Remove the rest of the missing data inplace
# Verify the missing values are removed by viewing the DataFrame
# Create a "Seats" column where every row has a value of 5
# Create a column called "Engine Size" with random values between 1.3 and 4.5
# Remember: If you're doing it from a Python list, the list has to be the same length
# as the DataFrame
# Create a column which represents the price of a car per kilometer
# Then view the DataFrame
# Remove the last column you added using .drop()
# Shuffle the DataFrame using sample() with the frac parameter set to 1
# Save the the shuffled DataFrame to a new variable
# Reset the indexes of the shuffled DataFrame
# Change the Odometer values from kilometers to miles using a Lambda function
# Then view the DataFrame
# Change the title of the Odometer (KM) to represent miles instead of kilometers.


