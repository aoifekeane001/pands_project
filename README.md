# Programming & Scripting Project
### Author: Aoife Keane

## Table of Contents
1. Project Name
2. Project Description
3. Project Scope
4. Objectives
5. Assumptions
6. Approach
7. Initial Data Research & Summary
8. Python Program ('analysis.py') & Summary
9. References

## Project Name 
Fisher Iris data set analysis

## Project Description
Purpose of this project is to research the Fishers Iris data set and write documentation and code (in Python) to investigate it, demonstrating learnings from ATU Programming & Scripting course modules 

## Project Scope
### In Scope
Data: 
* Fishers Iris data set (https://www.kaggle.com/datasets/uciml/iris) 

Project Requirements: 
* Python Program ('analyis.py)
1. Outputs a summary of each variable to a single text file 
2. Saves a histogram of each variable to png file 
3. Outputs a scatter plot of each pair of variables 
4. Performs any other appropriate analysis 

### Out of Scope
Data: 
* Any other data set not listed in scope of this document

Project Requirements: 
* Any requirement not listed in scope of this document

## Objectives
* Research & analyse the Fishers Iris data set online and interpret the data in your own words using course learnings to extract the data
* Use learnings from ATU Programming & Scripting course to successfully write a python program called 'analysis.py'

## Assumptions
* Correct data set used for the project
* Measuring system is accurate and precise

## Approach 
Process Steps to analyse the data in order to meet project requirements:
* Data Collection 
* Data Preparation 
* Data Exploration /Data Visualisation 
* Results Interpretation

Types of data analysis in orde to meet project requirements:
* Descriptive Analysis
* Data Reprocessing
* Data Visualisation

Use Python libraries:
* NumPy: supports n-dimensional arrays and provides numerical computing tools - useful for Linear algebra and Fourier transform
* Pandas: to handle missing data, manipulate the data, perform mathematical operations
* Matplotlib: to add data visualisation (e.g. graphs, charts, histograms, plots)

## Initial Data Research & Summary
* Fisher's Iris data set was introduced by the British statistician and biologist Ronald Fisher in 1936
* Data set was used in R.A. Fisher's classic 1936 paper, The Use of Multiple Measurements in Taxonomic Problems, and can also be found on the UCI Machine Learning Repository
* It is a well-known and commonly used data set in the field of machine learning & statistics and pattern recognition techniques
* The data set consists of 150 samples, with 50 samples of each of the three Iris species
* The data set consists of measurements of four features of the three different species of Iris flowers: setosa, versicolor, and virginica 
* It includes three iris species with 50 samples each as well as some properties about each flower
* One flower species is linearly separable from the other two, but the other two are not linearly separable from each other
* The four features / variables measured for each sample are - Sepal length, Sepal Width, Petal Length, Petal Width
* Key objective of the Fisher's Iris data set is to distinguish between the three different species of iris flowers based on the measurement features

## Python Program ('analysis.py') & Summary
### Python program 'analysis.py'
###  Data Analysis Process Steps for Python Program:
#### Data Collection
Collect the data set by doing the following steps:

Import the libraries: 
* import pandas as pd
* import seaborn as sns
* import matplotlib.pyplot as plt

Import Fisher's Iris data set (CSV) file: 
* Download data set from Kaggle (https://www.kaggle.com/datasets/uciml/iris) 
* Save to local Downloads folder on C drive
* Import the data set to Jupyter notebook as follows:
* iris_data=pd.read_csv ('Iris.csv')

#### Data Preparation
Remove any unwanted and redundant values, convert to the right format, and make it ready for analysis by doing the following:

* Display the first few rows of the data set: 
* iris_data.head()

Check for missing values: 
* iris_data.isnull().sum()

Get descriptive stats:
* iris_data.describe()

#### Data Exploration & Data Visualisation
Explore data using various data visualization techniques to find unseen trends from the data by doing the following steps & meet project requirements 1-3:

* Requirement 1: Outputs a summary of each variable to a single text file

Summary of data set: 
* iris_data.info()


* Requirement 2: Saves a histogram of each variable to png file 





* Requirement 3: Outputs a scatter plot of each pair of variables 

Plot the distribution of the features: 
* sns.histplot(data=iris_data, x='sepal_length', kde=True)

Scatter plot for relationship between two features: 
* sns.scatterplot(data=iris_data, x='sepal_length', y='petal_length', hue='species')plt.show()

Identify outliers with a Boxplot: 
* sns.boxplot(data=iris_data)plt.show()

#### Results Interpretation & Summary
Derive meaningful results and check if the output is in line with your expected results.

* Requirement 4: Performs any other appropriate analysis



## References
* UCI Machine Learning ‘Iris Species’ https://www.kaggle.com/datasets/uciml/iris
* Make a README https://www.makeareadme.com/ 
* Data Analytics with Python: Use Case Demo https://www.simplilearn.com/tutorials/data-analytics-tutorial/data-analytics-with-python
* Python.Org 'The Python Standard Library' (https://docs.python.org/3/library/index.html)
* Plotting Histogram in Python using Matplotlib https://www.geeksforgeeks.org/plotting-histogram-in-python-using-matplotlib/
