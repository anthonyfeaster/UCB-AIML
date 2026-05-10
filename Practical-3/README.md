# Practical Application III: Comparing Classifiers
**Author:** Anthony Feaster II<br>
**Assignment:** Practical Application #3 <br>
**Date:** Apr 2026

## Introduction
This project uses a Portuguese bank dataset to make comparisons of several classification models. The purpose of this project is to predict whether a bank client will subscribe to a term deposit based on selected banking information. The following models were used for this assignment: Logistic Regression, K Nearest Neighbors (KNN), Decision Tree and Support Vector Machine (SVM).

## Data Source
This data comes from the UCI Machine Learning Repository and is a collection of the results of multiple marketing campaigns from a Portuguese banking institution.

## Dataset Description
This dataset contains records from several market campaigns by a Portuguese banking institution. Customers were contacted directly once or multiple times by phone. 
* Demographics: Age, Job, Marital Status, Education
* Financial Attributes: Default, Housing, Loan
* Current Campaign Attributes: Contact, Day, Month, Duration
* Previous Campaign Attributes: Campaign, Pdays, Previous, Poutcome
* Target Variable: Y

## Exploratory Data Analysis (EDA)
During the exploratory data analysis (EDA) phase, I reviewed the entire dataset to include the shape of the data, missing values, column data types, duplicate and missing values. The dataset is quite large as it contains 21 columns and over 41k entries. I noticed several columns that contained "unknown" values. These entries will need to be further evaluated before modeling.

### Visualizations Created 
This project includes the following visualizations:
* Histplot - Client Distribution by Age
* Countplot - Loan Status by Occupation Type
* Boxplot - Age Distribution by Subscription Status
* Barplot - Subscription Rate by Marital Status

## Data Preparation
After evaluating the overall effect of making changes to the "unknown" values throughout the dataset, it was determined that removing them from the job and marital columns was ok because it only represented .8% and .19% of the data. For the other columns, "unknown" made up too significant of entries to drop them. In addition, all of the duplicate entries were found and removed before modeling.

## Modeling
I used DummyClassifier to create a baseline model utilizing the 'most frequent' strategy. This model uses the majority class for its predictions.

I then used the following classification models to train and later compared them:
1. Logistic Regression
2. K Nearest Neighbor (KNN)
3. Decision Tree
4. Support Vector Machine (SVM)

## Model Evaluation
Models were evaluated by using the following:
* Train Time
* Train Accuracy
* Test Accuracy
  
## Key Findings
* The dataset is imbalanced. Most clients are not subscribers to a term deposit
* Using the majority class, the baseline model predicted with high accuracy
* The SVM model was the most accurate but took the longest time to train
* The Decision Tree model showed signs of overfitting. GridSearchCV improved the accuracy by reducing overfitting.

## Recommendations
* For future work to this project I recommend retraining models using campaign related or economic features to improve performance. Also recommend tuning the Logistic Regression and KNN models to see if accuracy improves.
