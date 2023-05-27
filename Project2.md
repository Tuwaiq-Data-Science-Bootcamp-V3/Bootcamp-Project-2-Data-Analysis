# Crimes Analytics

Team members: Nourah Almuhaisen, Sarah Alyami and Lama Alshabani.

<img width="900" height="500" src="https://github.com/LamaAlshabani/Bootcamp-Project-2-Data-Analysis/blob/main/Burdick-TV-Crime.jpg.webp">

## Problem Statement

The problem is to analyze a crime dataset and gain insights into crime patterns, trends, and relationships within the data. By understanding the characteristics of reported crimes, we aim to identify key factors that can contribute to crime prevention and overall community safety.

## Objectives

1. Explore the distribution of crime occurrences by different dimensions such as time and crime subcategories.

2. Identify the most common types of crimes and their frequency of occurrence.

3. Analyze the relationship between reported time and other variables such as crime subcategories and clearance status.

4. Investigate any correlations or trends between specific types of crimes and their occurrence during different times of the day.

5. Visualize the crime data using various charts and graphs to facilitate a better understanding of the patterns and trends.

## Dataset

### Dataset Source:

We used The Crime DataSet from kaggle [Click here to access the dataset](https://www.kaggle.com/datasets/adoumtaiga/crime-data-set).

### Dataset Overview:

This dataset comprises around 481,000 crime reports from Seattle, WA, spanning approximately 10 years. It includes essential information for each crime offense, such as date and time details, crime categories and descriptions, police department information including sector, beat, and precinct, as well as the neighborhood name associated with each incident.

## Data Cleaning

1- During the data cleaning process, we performed several essential exploratory data analysis (EDA) steps to gain insights into the dataset and ensure its cleanliness and integrity. These steps included:

- Head: We used the `head()` function to inspect the initial rows of the dataset. 

- Shape: The `shape` attribute provided us with the dimensions of the dataset, indicating the number of rows and columns. 

- Info: By utilizing the `info()` function, we obtained a summary of the dataset's structure. 

- Describe: We employed the `describe()` function to generate descriptive statistics of the dataset. 

2. Handling Missing Values:

To address missing values in the dataset, we employed the following approach:

- Reported Time and Occurred Time Columns: 
We identified missing values in the Reported Time and Occurred Time columns by applying the `isna()` function. Since these columns are crucial for our analysis, we decided to drop the rows with missing values using the `dropna()` function. This ensures that we have complete and accurate time information for each crime report.

- Other Columns:
For the remaining columns, we tackled missing values by utilizing the `mode()` function. The `mode()` function allows us to determine the most frequent value in each respective column. We then filled the missing values in these specific columns with their respective mode values. This approach ensures that the missing values are replaced with meaningful and representative data points based on the prevailing values in the dataset.

3. For handling duplicated rows in the dataset, we employed the following steps:

- Duplicated Function: We utilized the `duplicated()` function to identify duplicate rows in the dataset. 

- Drop Duplicates: To eliminate the duplicated rows from the dataset, we employed the `drop_duplicates()` function. By default, this function keeps the first occurrence of each duplicated row and removes all subsequent duplicates.

4. To address the date format in the dataset, we performed the following steps:

- Reported Time and Occurrence Time Columns: We focused on the "Reported Time" and "Occurrence Time" columns, which contained time information.

- Reformatting with to_datetime(): We utilized the `to_datetime()` function from pandas to convert the values in these columns to datetime format. By specifying the `format='%H%M'` parameter, we instructed the function to interpret the values as hours and minutes in a 24-hour clock format.

- Resulting Format: The values in the "Reported Time" and "Occurrence Time" columns were successfully reformatted to the '%H%M' format. For example, a value like '1345' was transformed into '13:45' to represent 1:45 PM.

5. Finally, the cleaned dataset is saved in a new CSV file.

## The final ten insights

- What are the top 5 Crimes in the dataset?

- What are the most common type of CAR PROWL crime in the dataset?

- What are the most common type of HOMICIDE crime in the dataset?

- How does the number of reported crimes vary by day of the week?

- What is the distribution of crime occurrences throughout the day?

- What are the top 5 most common crimes subcategories occurence from 00.00 AM to 04.59 AM?

- How does the number of occurrences crimes vary by day of the week?

- What are the top 10 reported Narcotic crime ?

- How does the number of theft shoplifting incidents vary across different months?

- What are the different types of crimes associated with weapons and their respective proportions?
