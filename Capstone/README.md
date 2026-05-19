# Capstone - Machine Learning Based Intrusion Detection System
**Author:** Anthony Feaster <br>
**Assignment:** Capstone <br>
**Date:** May 2026

## Executive Summary

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

## Next Steps

