# Will the Customer Accept the Coupon?
**Author:** Anthony Feaster <br>
**Assignment:** Practical Application #1 <br>
**Date:** Dec 2025

## Introduction
The goal of this assignment is to determine if external factors such as passenger type, age, occupation and others contribute to the acceptance rate of a coupon. The use of statistical analysis and visualizations will help show which drivers accepted the coupon vs drivers who did not.

## Data Source
This data comes from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk.

## Dataset Description
The dataset contains different attributes that describes the driver and provides context to their driving situation when surveyed.
* User Attributes: Gender, Age, Marital Status, Education, Occupation and Income
* Situational Attributes: Driving Destination, Weather, Temperature, Time and Passenger
* Coupon Attributes: Type of coupon (Bar, Coffee House, Restaurant, etc) and expiration

## Analysis
Overall, the acceptance rate for all coupons in the provided data set was about 57% but this figure varied by coupon type.

### Bar Coupon Analysis
* Humans are creatures of habit. Drivers who visit the bar at least once per month had a 76% acceptance rate showing that they are significantly more likely to accept the coupon compared to those who rarely visit.
* The rate of drivers who accepted coupons were elevated under social conditions. Drivers with adult passengers (friends or partners) were significantly more likely to accept a bar coupon in comparison to drivers with children.
* The data shows that younger drivers (30 and under) and those with lower incomes are more receptive to accepting the coupons.

### Independent Investigation - Coffee House Analysis
* I performed a comparative analysis of the Coffee House coupons to determine if a person's occupation made a difference in the acceptance rate.
* Healthcare and Building & Ground Maintenance workers had the highest acceptance rate out of all of the occupations. These industries typically align with shift work and are more prone to many caffeine runs.
## Recommendations
* Based on the analysis, future bar coupon campaigns should target adult individuals/drivers during the night and weekend hours when they are more likely to have adult passengers.
* The next marketing campaign for the Coffee House should target medical facility and industrial parks, possibly during 6AM/6PM time frame to capture the start/end of shifts for the healthcare and maintenance demographic.
