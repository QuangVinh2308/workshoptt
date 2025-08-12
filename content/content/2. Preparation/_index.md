---
title : "Preparation "
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

This section outlines the requirements and setup steps before implementing the intelligent Auto Scaling system.  
It ensures that all tools, permissions, and data sources are in place for both **reactive** and **predictive** scaling configurations.

**2.1 Prerequisites**  
Before starting, make sure you have:
- **AWS CLI** installed and configured with the correct profile and region.
- **IAM permissions** to create and manage EC2, Auto Scaling Groups, CloudWatch, SageMaker, and Lambda.
- Basic knowledge of **time-series forecasting** and AWS architecture patterns.
- A working AWS account with sufficient quota for EC2 instances and other required services.

**2.2 Dataset**  
The project will use:
- **CloudWatch metrics** such as CPU utilization, request count, and network I/O.
- **External datasets** for seasonal patterns or event-driven traffic (e.g., marketing campaigns, holidays).
- Historical data should cover enough time to capture patterns and trends for accurate forecasting.

By completing this preparation phase, you ensure the environment is ready for building and testing the **ML-powered Auto Scaling pipeline**.