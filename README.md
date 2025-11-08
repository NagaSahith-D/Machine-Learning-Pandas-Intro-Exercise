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

