---
title : "Data Pipeline"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

This section describes how to gather, clean, and prepare metrics for use in the Machine Learning forecasting models.  
A well-designed data pipeline ensures high-quality input data, which is critical for accurate predictions.

The pipeline consists of three main stages:
1. **Collect Metrics** from CloudWatch, ASG logs, and external sources.
2. **Clean and Feature Engineer** the data to make it suitable for model training.
3. **Store and Retrieve** the processed dataset for efficient use in training and inference.