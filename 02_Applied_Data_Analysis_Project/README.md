# **Advanced Applied Data Analysis Project**

## **Author**
Ophélie Rutschmann 
Project submitted in March 2026.

## **Introduction**
The goal of this project is to showcase skills in applied data analysis by exploring a dataset, preparing it for in-depth analysis and drawing meaningful insights from it. The dataset for this project is collected from the Open Food repo, a community-driven open database for barcoded food products. This dataset contains the ingredients and nutritional facts of approximately 385k food products, from several countries worldwide.

## **Methodology**
This project is separated into several units. Each unit is contained in a single jupyter lab notebook (with the exception of units B and C that are combined in the same notebook. All of the notebooks can be found in this repository.

### **Unit A: An overview of the dataset**
In this first unit, the goal is to gain some general information about the dataset before starting the exploration journey in the other subjects. 

### **Unit B: Data Cleaning**
The goal of this unit is to get familiar with the strengths and weaknesses of the data set and prepare it for in-depth analysis. 
In this unit, I performed several data cleaning steps mainly focusing on removing duplicated rows and filling in missing values. Several strategies will be used to adress the missing values.

### **Unit C: Preliminary Exploratory Data Analysis (EDA)**
The goal of this unit is to explore the variables in our data in more detail. This will allow us to gain a better understanding of the limitations and inconsistencies in our data set. Once we have explored the data, will perform additional cleaning steps to adress inconsistencies and errors in our data, and remove extreme values. At the end of the unit, we will save the cleaned data as a new pickle file and make sure to use this cleaned data for further analysis later on. 

### **Unit D: Text Data**
The goal of this unit is to demonstrate essential data analysis skills related to text data. We will tokenize items in the ingredients_en column into individual ingredients and answer several questions related to the ingredients. 

### **Unit E. EDA: Time-series data**
Another data type that requires specific methods and skills for analysis is time-series data. Although the Open Food database is not a time-series database, it contains several columns with dates and times, allowing for a simple investigation. The goal of this unit is to work with the created_at column that stores the date and time at which products were added to the Open Food database and create two visualizations of the data to understand it better. 

### **Unit F: correlation analysis**
The goal of this unit is to try out different statistical tests on our data set. We will quantify the linear relationship between the energy_per_hundred and the per_hundred columns by computing their correlation, and reveal the true nature of the relationship between some of these variables using visualizations. 
Finally, we will test the independence of two categorical variables statistically. We will test if the energy level in a product is associated with the country in which the product is produced.

### **Unit G: Advanced EDA**
The goal of this unit is to perform a couple of advance data analysis steps to answer the following questions:
- What is the total number of samples by country ? Countries with very small sample size should be dropped from this analysis
- Count the number of organic and non-organic products in each country. Is there a country with a higher percentage of organic products ?
- Compare the distributions of the macronutrients between organic and non-organic products in each country.

## **Table of content**
### **Unit A**
1) Importing the data
2) Exploration of data types
3) Creating columns for each data type
4) Creating columns based on the type of information they hold

### **Unit B**
0. Importing the Data  
1. Checking and Removing Duplicated Rows  
2. Checking for Missing Values  
   - a) Assessing the Percentage of Missing Values  
   - b) Visualizing Missing Values Using the `missingno` Library  
   - c) Visualizing Missing Values Using Bar Plots and Violin Plots  
3. Addressing Missing Values  
   - a) Removing Empty Rows / Columns  
   - b) Filling in Missing Values Using the Most Frequent Value in the Column  
   - c) Filling Missing Values Using Related Columns  
   - d) Filling Missing Values Using Common Knowledge  
   - e) Filling Missing Text Values by Indicating the Field Is Missing  
   - f) Removing Columns That Still Contain > 95% Missing Values  
   
### **Unit C**
1. Data Visualization
    - a) Visualizing the categorical variables
    - b) isualizing the numerical variables
2. Cleaning the data
    - a) Removing improbable values and errors
        - Addressing wrong values in the per_hundred column
        - Addressing inconsistencies and errors using related columns
    - b) Removing outliers

3. Saving the data

### **Unit D**
1) Data exploration
2) Data cleaning
3) Tokenization
4) Identifying the longest and shortest ingredient lists
5) Identifying the most frequent products

### **Unit E**
1) Plotting the total number of items created each month at each hour. 
2) Plotting the evolution of the total number of items over time.

### **Unit F**
1) Correlation analysis
    - a) Computing the correlations
    - b) Visualizing the correlations
2) Independence testing
    - a) Data exploration and cleaning
    - b) Statistical testing

### **Unit G**
1) What is the total number of samples per country?
2) What is the percentage of organic products for each country?
3) Comparision in the distribution of macronutrients between organic and non organic products.