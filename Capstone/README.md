# Capstone - Machine Learning Based Intrusion Detection System
**Author:** Anthony Feaster II<br>
**Assignment:** Capstone <br>
**Date:** June 2026

## Executive Summary
This project evaluates whether machine learning models can classify network traffic as benign or malicious using network flow data. The dataset contains features such as source and destination IP addresses, protocols, packet count, traffic labels, source and destination ports, and byte count. 

Using these data features to perform initial data cleaning, exploratory data analysis, feature engineering, model training, hyperparameter tuning and model evaluation. Several additional engineered features such as ICMP indicators, source and destination frequency, rate-based traffic, and port categories were created to provide more network behavioral context.

Models were created and evaluated using accuracy, precision, recall, F1 score and confusion matrices. Logistic Regression performed the best among the classification models however, model performance remained close to the baseline. Since the dataset was nearly balanced between benign and malicious traffic, the performance suggest that existing features were not enough to distinguish between the two classes.

## Rationale
Security analysts in a Security Operations Center (SOC) often review large volumes of network logs and alerts to identify suspicious activity. Although there are security tools that can help with detecting anomalies, analysts still need to determine if traffic is benign or malicious. 

This is an interesting and important problem set because false positives and false negatives have different cybersecurity and business impacts. A false positive means unnecessary security alerts which could lead to analyst fatigue while a false negative may allow malicious traffic to go undetected.

## Research Question
Can machine learning models accurately classify network traffic as malicious or benign using network flow data that contains features such as ports, packet counts, connection duration, protocols, source and destination IP addresses?

## Data Sources
The data used for this capstone project comes from a Kaggle dataset called, "Network Traffic Data for Intrusion Detection". This is a network flow dataset where each column contains different aspects of a standard network transaction.
* IP Attributes: Protocol, SourceIP, DestinationIP, SourcePort, DestinationPort
* Network Connection Attributes: Duration, PacketCount, ByteCount
* Label - Target Variable - identifies traffic as 'normal' or 'attack'

The original labels were renamed to current cybersecurity terminology:
* Normal was renamed to Benign
* Attack was renamed to Malicious

# Methodology
For this project, I developed a machine learning based intrusion detection system designed to accurately categorize network traffic as either benign or malicious. The project followed standard machine learning workflow to include data acquisition and cleaning, exploratory data analysis, feature engineering, model training hyperparameter tuning and model evaluation.

* Data Acquisition and Cleaning
  * The dataset was loaded into a pandas DataFrame and checked for missing values, duplicate rows and data types. Target labels were renamed to be consistent with current cybersecurity terminology.
* Exploratory Data Analysis (EDA)
  * During this phase, analysis was performed to understand the dataset and identify potential traffic patterns. This included reviewing class balance between benign and malicious traffic, analyzing protocol distribution, rate-based correlation and exploring port behavior.
* Feature Engineering
  * Additional features were created to give the models with more network behavior context. These features included port categories, rate-based traffic, protocol indicators and frequency based features.
* Modeling
  * During this phase data was preprocessed and prepared for classification models. A Dummy Classifier was used to build a baseline model and Logistic Regression and Random Forest models were trained to evaluate performance. GridSearchCV was used to tune Random Forest model. Models performance were evaluated using accuracy, precision, recall, F1 score and confusion matrix. Evaluating the accuracy of a model alone was not sufficient  because false positives and false negatives have different cybersecurity and business impacts.

## Results
The results of the models performance close to baseline. The Logistic Regression model performed the best out of the classification models. Overall, the results suggest that existing features were not enough to distinguish between the two classes.

## Next Steps
* Future iterations of this project can include timestamped network traffic. This would allow analysis of traffic history and whether ICMP packets hit a destination IP before malicious traffic occurs. In addition the timestamped network traffic would allow for additional features to be created and analysis performed to determine deeper correlation of the data. Additional predictive models can be used to proactively monitor and detect network anomalies.

## Outline of Project
* https://github.com/anthonyfeaster/UCB-AIML/blob/main/Capstone/capstone_final.ipynb
