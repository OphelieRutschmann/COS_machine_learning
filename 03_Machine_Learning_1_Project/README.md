# **House Price Prediction using Multiple Linear Regressions and the Ames Housing Data Set (In Progress)**

## **Author**
Ophélie Rutschmann

## **Introduction**
This project uses a house price dataset compiled and published by Dean De Cock, which contains 2,930 observations across 82 features. The original data, sourced directly from the Ames Assessor’s Office, was collected for tax assessment purposes.

The primary goal of this project is to develop and evaluate Linear Regression Models that can accurately predict house prices based on the available features. During this project, I will go through all the main steps of a data science project i.e. **preparing the data**, **exploring the data (EDA)** and **modeling**. In the modeling part, I will use a training set that consists of 2430 ones entries to fit and evaluate different models and use them to make predictions for a test set consisting of 500 entries.

## **Methods**

This project is separated into several jupyter notebooks that each contain an important section of the data analysis and modeling pipeline. 

#### **Section 1: Exploratory data analysis and data cleaning**
The objective of this section is to gain a better understanding of the dataset through exploratory data analysis and visualizations. By examining the distributions and patterns within the data, I want to identify potential issues such as missing or inconsistent values, errors, and outliers. Once the issues have been identified, I will clean the data using different methodologies. 

#### **Section 2: Feature engineering**
The goal of this section is to enhance the dataset by creating new features and transforming existing ones to improve the predictive power of the model. There are several strategies that I will follow during this section, with the goal to capture additional information from the raw data.

#### **Section 3: Feature encoding**
The goal of this section is to encode the categorical features in our data set. I will encode both nominal features (where we don't need to order the categories) and ordinal features (where we will define how to order the categories).

#### **Section 4: Data Splitting**


## **Table of content**

#### **Section 1: Exploratory data analysis and data cleaning**
1. **Preliminary EDA and data cleaning**
    - 1.1 Preliminary data set exploration
    - 1.2 Removing duplicated rows
    - 1.3 Removing empty rows / columns
2. **Exploratory data analysis**
    - 2.1 Continuous variables
        - a) Identifying missing values
        - b) Identifying values with the wrong data type
        - c) Identifying and removing incorrect values
        - d) Removing features with low correlation to sale price
        - e) Removing possible colinear features
    - 2.2 Discrete variables
        - a) Identifying missing values
        - b) Identifying values with the wrong data type
        - c) Identifying and removing incorrect values
        - d) Removing features with low correlation to sale price
        - e) Removing possible colinear features
    - 2.3 Nominal variables
        - a) Identifying missing values
        - b) Removing features with low impact on sale price    
    - 2.3 Ordinal variables
        - a) Identifying missing values
        - b) Removing features with low impact on sale price
3. **Sale Price distribution**
    - 3.1 Plotting the distribution
    - 3.2 Identifying outliers
4. **Outlier Removal**
    - 4.1 Identifying outliers for the continuous variables
    - 4.2 Identifying rare/extreme values for the discrete variables
    - 4.3 Identifying rare values for the nominal variables
    - 4.4 Identifying rare values for the ordinal variables
    - 4.5 Filtering the training data set
5. **Summary**
6. **Saving the cleaned data**

#### **Section 2: Feature Engineering**
1. **Creating indicator variables**
    - 1.1 Selecting the variables
    - 1.2 Indicator variables for variables we wish to replace
    - 1.3 Indicator variables for variables we do not wish to replace
2. **Creating summary variables**
    - 2.1 Investigating "Porch" features
    - 2.2 Investigating "Bathrooms" features
3. **Creating polynomial variables**
    - 3.1 Selecting the variables
    - 3.2 Creating polynomial features for Gr Liv Area
4. **Saving the data sets**

#### **Section 3: Feature Encoding**
1. **Encoding the nominal features**
    - 1.1 Boolean Encoding for the "Central Air* feature
    - 1.2 One hot encoding for the other nominal features
    - 1.3 Reindexing the test data frame
2. **Encoding the ordinal features**
    - 2.1 Encoding the "Quality" features
    - 2.2 Encoding the "Quantity" features
    - 2.3 Encoding the "Lot Shape" feature
    - 2.4 Encoding the "Bsmt Exposure" feature
    - 2.5 Encoding the "BsmtFin Type" features
    - 2.6 Encoding the "Electrical" feature
    - 2.7 Encoding the "Functional" feature
    - 2.8 Encoding the "Garage Finish" feature
    - 2.9 Encoding the "Paved Drive" feature
3. **Saving the data sets**


## **Academic Integrity and Learning Statement**

By submitting my work, I confirm that:

- The code, analysis, and documentation in this notebook are my own work and reflect my own understanding.
- I am prepared to explain all code and analysis included in this submission.

If I used assistance (e.g., AI tools, tutors, or other resources), I have:

- Clearly documented where and how external tools or resources were used in my solution.
- Included a copy of the interaction (e.g., AI conversation or tutoring notes) in an appendix.

I acknowledge that:

- I may be asked to explain any part of my code or analysis during evaluation.
- Misrepresenting assisted work as my own constitutes academic dishonesty and undermines my learning.