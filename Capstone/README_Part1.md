# Capstone - Machine Learning Based Intrusion Detection System
**Author:** Anthony Feaster II<br>
**Assignment:** Capstone <br>
**Date:** May 2026

## Executive Summary
This project evaluates a critical workflow by analyzing network traffic data and providing valuable information to network security analysts. The machine learning based intrusion detection system aims to serve as an effective security monitoring tool allowing network security analysts to optimize their time for other important functions. A dataset of 2,000 network records was used to perform exploratory data analysis, data cleaning, feature engineering, and pipeline preprocessing. Three models were implemented to determine a baseline and evaluate their accuracy. The results demonstrated that the models performed similarly to a coin toss, indicating that more features might be needed to increase the accuracy of the predictions. 

## Rationale
Security analysts in a security operations center and cyber security engineer have to manually evaluate thousands of logs in order to keep their network safe and secure. There are tools that are used in this industry to help with this manual process but they are just alerting a human to potential anomalies. By using machine learning, alot of the network detection processes can be automated thus reducing false positives and enables efficiencies amongst the security analysts.

## Research Question
Can machine learning models accurately classify network traffic as malicious or normal using network flow data that contains features such as ports, packet counts, connection duration, protocols, source and destination IP address?

## Data Sources
The data used for this capstone project comes from a Kaggle dataset called, "Network Traffic Data for Intrusion Detection". This is a network flow dataset where each column contains different aspects of a standard network transaction.
* IP Attributes: Protocol, SourceIP, DestinationIP, SourcePort, DestinationPort
* Network Connection Attributes: Duration, PacketCount, ByteCount
* Label - Target Variable - identifies traffic as 'normal' or 'attack'

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

