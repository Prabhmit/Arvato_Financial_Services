# Bertelsmann/Arvato Project

# 1. Table of Contents

1. Installations and package requirement
2. Project Motivation
3. Project Components and File Descriptions
4. Instructions
5. Licensing, Authors and Acknowledgments

# 2. Installations and package requirement

The code is in Python 3.7.6. The Python libraries applied are numpy, pandas, scipy, matplotlib, seaborn and sklearn. 

# 3. Project Motivation

Bertelsmann/Arvato is a mail-order sales company in Germany. The motivation is to  analyze demographics data for its customers comparing it against demographics information for the general population. To achieve this, unsupervised learning techniques were used to perform customer segmentation, identifying the parts of the population that best describe the core customer base of the company. Then, on a separate dataset, Supervised learing is used to build a model to predict which individuals are most likely to convert into becoming customers for the company. 
The goal of of the project is to build a model that can acquire new clients efficiently for Bertelsmann/Arvato.

# 4. Project Components and File Descriptions

The datasets are Udacity_AZDIAS_052018.csv and Udacity_CUSTOMERS_052018.csv. Arvato Project workbook.ipynb is a Jupyter notebook which includes the relevant Python code for this excercise. 
Modularised_code.ipynb is a Jupyter notebook that contains modularised code for the entire project. 

There are four data files associated with this project:

Udacity_AZDIAS_052018.csv: Demographics data for the general population of Germany; 891211 persons (rows) x 366 features (columns).
Udacity_CUSTOMERS_052018.csv: Demographics data for customers of a mail-order company; 191652 persons (rows) x 369 features (columns).
Udacity_MAILOUT_052018_TRAIN.csv: Demographics data for individuals who were targets of a marketing campaign; 42982 persons (rows) x 367 (columns).
Udacity_MAILOUT_052018_TEST.csv: Demographics data for individuals who were targets of a marketing campaign; 42833 persons (rows) x 366 (columns).

Information regarding the data is included in:
DIAS Information Levels Attributes 2017.xlsx: is a top-level list of attributes and descriptions, organized by informational category. 
DIAS Attributes - Values 2017.xlsx: is a detailed mapping of data values for each feature in alphabetical order.

The following .csv files are created during the project to have the relevant data-sets saved at various stages of analysis for time efficiency:

azdias_clean.csv: cleaned general poplulation dataset
customers_clean.csv: cleaned customers dataset
azdias_clean_clustered.csv: cleaned general poplulation dataset with cluster column
customers_clean_clustered.csv: cleaned customers poplulation dataset with cluster column
mailout_train.csv: cleaned test dataset 
mailout_test.csv: cleaned test dataset

Under an agreement with AZ Direct GmbH's General Terms, none of data files have been included in the repository.

The project has four components: 

## A. Get to know the data

In this component a detailed inspection and cleaning of the general population data is undertaken. Based on this, a function was created to clean the other three data files at relevant stages of the project.

## B. Customer segmentation report 

In this component unsupervised learning techniques were used to describe the relationship between the demographics of the company's existing customers and the general population. 
The goal is to describe parts of the general population that are more likely to be part of the mail-order company's main customer base, and which parts of the general population are less so.

## C. Supervised learning model 

In this component similar data cleaning techniques were used to clean the test data to build three Supervised learning models that predicts whether or not each individual will respond to the campaign.

## D. Kaggle competition 

In this part, the chosen model is used to make predictions on the campaign data as part of a Kaggle Competition. 
The customes in the mailout_test dataset were ranked on how likely they are to convert to being a customer.

The entry to the competition was a CSV file with two columns. The first column is "LNR", which is as an ID number for each individual in the "TEST" partition.
The second column, "RESPONSE" is measure of how likely each individual is to became a customer. The competition used AUC to evaluate performance. 
The exact values of the "RESPONSE" column did not matter as much: only that the higher RESPONSE values would try to capture as many of the actual customers as possible, early in the ROC curve sweep. 

# 5. Instructions

Run the cells in the Arvato Project workbook.ipynb notebook for a detailed analysis or Modularised_code.ipynb for a concise analysis and output.

# 6. Results

The detailed analysis, main findings and recommended improvements of the project can be found at [a link](paste weblink here)

# 7. Licensing, Authors and Acknowledgments

Data Scientist Capstone, Data Scientist Nanodegree Program, Udacity, https://www.udacity.com/course/data-scientist-nanodegree--nd025

Capstone Project: Bertelsmann/Arvato Project, Udacity, https://www.udacity.com/course/data-scientist-nanodegree--nd025

scikit-learn, Machine Learning in Python - https://scikit-learn.org/stable/index.html
