# What drives the price of a car?
**Author:** Anthony Feaster <br>
**Assignment:** Practical Application #2 <br>
**Date:** Feb 2026

## Introduction
This project will analyze a large used car dataset to identify attributes such as color, milage, cylinders, etc contribute to the pricing of a vehicle. The goal is to provied used car dealerships with adequate information so they can competitively price their vehicles.

## Data Source
The data used for this assignment comes from a Kaggle used car dataset.

## Dataset Description
The dataset contains different attributes for serveral types of vehicles.
* Price
* Year
* Odometer
* Cyclinder
* Model
* Manufacture
* Condition
* Fuel Type
* Transmission
* Vehicle Type
* Paint Color

## Exploratory Data Analysis (EDA)
* After examining the dataset, it was evident that the data set is large with over 427k vehicle records 
* Dataset contained many null entries
* Looked for the unique values for several columns
* Created a few visualizations to gain a better understanding of the data:
* * Distribution of Vehicle Prices
  * Barplot of Odometer Distribution
  * Scatterplot of Milage vs Price
  * Condition vs Price

## Data Preparation
The following steps were performed to clean the data
* Removed unncessary columns that will not affect vehicle prices (ie: VIN, ID, etc)
* Stripped strings from the cylinder column and converted the values to numeric values
* Deteremined the percentage of NaN rows in each column to determine if the column should be dropped for filled with other values. Filled NaN rows with 'unknown'
* Removed rows missing a year value
* Filtered out extreme outliers for visualization purposes

### Key Insights
* The vehicle prices generally decreases as the milage increases
* New vehicles tend to higher pricesses
* The manufacturer can also influence the price of vehicles

## Modeling
1. Linear Regression
2. Ridge Regression
3. Random Forest Regression (had to comment it out because the program kept freezing due to compute restraints)
