# Practical Application III: Comparing Classifiers
**Author:** Anthony Feaster <br>
**Assignment:** Practical Application #3 <br>
**Date:** Apr 2026

## Introduction
This project uses a Portuguese bank dataset to make comparisons of several classification models. The purpose of this project is to predict whether a bank client will subscribe to a term deposit based on selected banking information. The following models were used for this assignment: Logistic Regression, K Nearest Neighbors (KNN), Decision Tree and Support Vector Model (SVM).

## Data Source
This data comes from the UCI Machine Learning Repository and is a collection of the results of multiple marketing campaigns from a Portuguese banking institution.

## Dataset Description
This dataset contains records from several market campaigns by a Portuguese baniking institution. Customers were contacted direcly once or multiple times by phone. 
* Demographics: Age, Job, Martial Status, Education
* Financial Attributes: Default, Balance, Housing, Loan
* Current Campaign Attributes: Contact, Day, Month, Duration
* Previous Campaign Attributes: Campaign, Pdays, Previous, Poutcome
* Target Variable: Y

## Exploratory Data Analysis (EDA)
During the exploratory data analysis (EDA) phase, I reviewed the entire dataset to include the shape of the data, missing values, column data types, duplicate and missing values. Several columns contained "unknown" values. I evaluated the overall effect of making changes before removing them from the job and marital columns. For the other columns, "uknown" made up too significant of entries to drop them. Also, all of the duplicate entries were found and removed before modeling.

* The dataset contains 21 columns with over 41k entries.
* Several columns contained "unkown' values

### Visualizations Created 
This project includes the following visualizations:
* Histplot - Client Distribution by Age
* Countplot - Loan Status by Occupation Type
* Boxplot - Age Distribution by Subscription Status
* Barplot - Subscription Rate by Marital Status

## Data Preparation



## Modeling
I used DummyClassifier to create a baseline model utilzing the 'most frequent' strategy. This model uses the majority class for its predictions.

I then used the following classification models to trained and later compared them:
* Logistic Regression
* K Nearest Neighbor (KNN)
* Decision Tree
* Support Vector Model (SVM)


## Model Evaluation
Models were evaluated by using the following:
* Train Time
* Train Accuracy
* Test Accuracy
  
## Key Findings

## Recommendations
