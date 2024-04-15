# Pymaceuticals_Inc_Challenge
Module 5 Challenge- applying what I've learned about Matplotlib to a real-world situation and dataset.


**Background:**
I have just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, I have been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked me with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked me for a top-level summary of the study results.


**Instructions:**
This assignment is broken down into the following tasks:

- Prepare the data.

- Generate summary statistics.

- Create bar charts and pie charts.

- Calculate quartiles, find outliers, and create a box plot.

- Create a line plot and a scatter plot.

- Calculate correlation and regression.

- Submit your final analysis.

**Prepare the Data**- 

a) Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

b) Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

c) Display the updated number of unique mice IDs.

**Generate Summary Statistics**- 

a) Create a DataFrame of summary statistics. 
  
  Your summary statistics should include:

  a. A row for each drug regimen. These regimen names should be contained in the index column.
 
  b. A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.
    
b) Create Bar Charts and Pie Charts to show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

  a. Create the first bar chart with the Pandas DataFrame.plot() method.
 
  b. Create the second bar chart with Matplotlib's pyplot methods.

c) Generate two pie charts to show the distribution of female versus male mice in the study.

  a. Create the first pie chart with the Pandas DataFrame.plot() method.

  b. Create the second pie chart with Matplotlib's pyplot methods.

d) Calculate Quartiles, Find Outliers, and Create a Box Plot
  Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 
  Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

  a. Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
 
  b. Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
 
  c. Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. 

  d. Append the resulting final tumor volumes for each drug to the empty list.

  e. Determine outliers by using the upper and lower bounds, and then print the results.

e) Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group.
  Highlight any potential outliers in the plot by changing their color and style.

  a. Create a Line Plot and a Scatter Plot
 
  b. Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

  c. Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

f) Calculate Correlation and Regression
 
  a. Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
 
  b. Plot the linear regression model on top of the previous scatter plot.
