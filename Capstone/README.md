# Capstone - Machine Learning Based Intrusion Detection System
**Author:** Anthony Feaster II<br>
**Assignment:** Capstone <br>
**Date:** June 2026

## Executive Summary
This project evaluates whether machine learning models can classify network traffic as benign or malicious using network flow data. The dataset contains features such as source and destination IP addresses, protocols, packet count, traffic labels, source and destination ports, and byte count. 

Using these data features to perform initial data cleaning, exploratory data analysis, feature engineering, model training, hyperparameter tuning and model evaluation. Several additional engineering features such as ICMP indicators, source and destination frequency, rate-based traffic, and port categories were created to provide more network behavioral context.

Models were created and evaluated using accuracy, precision, recall, F1 score and confusion matrices. Logistic Regression performed the best amongst the classification models however, model performance remained close to the baseline. Since the dataset was nearly balanced between benign and malicious traffic, the models performance suggest that existing features were not enough to distinguish between the two classes.

## Rationale
Security analysts in a Security Operations Center (SOC) often review large volumes of network logs and alerts to identify suspicious activity. Although there are security tools that can help with detecting anomalies, analysts still need to determine if traffic is benign or malicious. 

This is an interesting and important problem set because false positives and false negatives have different cybersecurity and business impacts. A false positive means unneccisary security alerts which could lead to analyst fatigue while a false negative may allow malicious traffic to go undetected.

## Research Question
Can machine learning models accurately classify network traffic as malicious or benign using network flow data that contains features such as ports, packet counts, connection duration, protocols, source and destination IP address?

## Data Sources
The data used for this capstone project comes from a Kaggle dataset called, "Network Traffic Data for Intrusion Detection". This is a network flow dataset where each column contains different aspects of a standard network transaction.
* IP Attributes: Protocol, SourceIP, DestinationIP, SourcePort, DestinationPort
* Network Connection Attributes: Duration, PacketCount, ByteCount
* Label - Target Variable - identifies traffic as 'normal' or 'attack'

The orginal labels were renamed to current cybersecurity terminology:
* Normal was renamed to Benign
* Attack was renamed to Malicious

# Methodology
For this project, I developed a machine learning based intrusion detection system designed to accurately categorize network traffic as either benign or malicious.  First loaded and used exploratory data analysis on the dataset to determine data quality and integrity. Next was feature engineering to ensure the proper features were used to find correlations. The data was preprocessed and put through pipelines to prepare it for being trained in models. Benchmarks were established to compare the accuracy of the trained models.

## Results
* Baseline Model achieved an accuracy of 52.25%
* Logistic Regression Model achieved an accuracy of 49.5%
* Random Forest Classifier Model achieved an accuracy of 51.5%
* All models performed near the baseline which is expected since the malicious and benign data is split almost 50/50.

## Next Steps
* Future iterations of this project can include additional feature engineering to analyze if ICMP packets  hit a destination IP before malicious traffic occurs. In a real world scenario, attackers often scan or ping a target to see if it’s online before launching an attack.
* Implementing additional predictive models to estimate the likelihood of malicious traffic targeting a specific IP or port.
