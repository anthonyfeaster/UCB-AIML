# What Drives the Price of a Car?
**Author:** Anthony Feaster <br>
**Assignment:** Practical Application #2 <br>
**Date:** Feb 2026

## Introduction
This project analyzes a large used car dataset to identify which attributes (such as color, milage, cylinders, etc) are associated with vehicle pricing. The goal is to provide used car dealerships with adequate information so they can competitively price their vehicles.

## Data Source
The data used for this assignment comes from a Kaggle used car dataset.

## Dataset Description
The dataset contains different attributes for over 427,000 vehicles, including:

* Price
* Year
* Odometer
* Cylinder
* Model
* Manufacture
* Condition
* Fuel Type
* Transmission
* Vehicle Type
* Paint Color

## Exploratory Data Analysis (EDA)
* After examining the dataset, it was evident that the data set is large with over 427k vehicle records
* Several columns contained missing (NaN) values
* Explored dataset for unique values to better understand categorical variables.

 ### Visualizations Created 
  * Distribution of Vehicle Prices
  * Barplot of Odometer Distribution
  * Scatterplot of Milage vs Price
  * Boxplot of Condition vs Price

## Data Preparation
The following steps were performed to clean the data:

* Removed unnecessary columns that will not affect vehicle prices (ie: VIN, ID, etc)
* Exacted numeric values from the cylinders column and converted them to numeric values
* Filled missing (NaN) categorical values with 'unknown'
* Removed rows with missing year values
* Filtered out extreme outliers for visualization purposes

## Modeling
The following regression models were used:
1. Linear Regression
2. Ridge Regression
3. Random Forest Regression (had to comment it out due to computational restraints)

## Model Evaluation
* R2 - Coefficient
* RMSE - Root Mean Squared Error

## Recommendations
* Based on the analysis, dealerships should prioritize inventory vehicles with lower milage to maintain higher resale value
* To determine an estimated fair market value, use regression modeling as your baseline tool
* Consider year, condition, and manufacturer when pricing 

### Key Insights
* The vehicle prices generally decreases as the milage increases
* New vehicles tend to higher prices
* The manufacturer can also influence the price of vehicles
