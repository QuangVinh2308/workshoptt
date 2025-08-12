---
title : "Prerequisites"
date : "`r Sys.Date()`"
weight : 2.1
chapter : false
pre : " <b> 2.1 </b> "
---

Before implementing the intelligent Auto Scaling system with Machine Learning, ensure the following prerequisites are met:

- **AWS CLI** is installed and configured with the correct credentials and default region.
- **IAM permissions** for managing EC2, Auto Scaling Groups, CloudWatch, SageMaker, Lambda, and S3.
- **Python environment** (3.8 or higher) with essential libraries such as `boto3`, `pandas`, `numpy`, `scikit-learn`, `statsmodels`, and `tensorflow/keras` for LSTM.
- Access to **CloudWatch metrics** and any **external data sources** relevant to traffic forecasting.
- Familiarity with **time-series forecasting** concepts and AWS architecture patterns.
- A working AWS account with sufficient **service quotas** for launching instances and using managed services.

These prerequisites ensure that your environment is fully prepared for both **reactive scaling** baseline setup and **predictive scaling** implementation using ML.
