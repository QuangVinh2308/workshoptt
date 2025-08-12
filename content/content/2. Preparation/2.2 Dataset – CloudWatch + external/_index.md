---
title : "Create IAM Role"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

The accuracy of predictive scaling depends heavily on the quality and diversity of data used for training and evaluation.  
This project leverages both **internal AWS metrics** and **external contextual data**.

**Primary Data Sources:**
- **Amazon CloudWatch metrics**: CPU utilization, request count, network I/O, and any custom application metrics.
- **Auto Scaling Group history**: Historical scaling actions and instance lifecycle events.
- **S3-hosted logs**: Application or access logs that can be aggregated for workload analysis.

**External Data Sources:**
- Event calendars (e.g., holidays, marketing campaigns) that influence user traffic patterns.
- Industry-specific seasonal trends or peak hours data.
- Any third-party API providing relevant traffic signals.

**Data Preparation Notes:**
- Ensure datasets are **time-aligned** and **aggregated** to consistent intervals.
- Handle **missing values** and **outliers** before model training.
- Store processed datasets in **Amazon S3** for reproducibility and easy integration with SageMaker.

Having a rich dataset combining system metrics with contextual information greatly improves the performance of **LSTM** and **ARIMA** forecasting models, enabling more accurate proactive scaling.
