---
title: "Collect Metrics"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 4.1 </b>"
---

Collect workload and performance data from multiple sources to serve as input for model training.

**Primary Sources:**
- **Amazon CloudWatch**: CPUUtilization, NetworkIn/Out, RequestCount, and any custom application metrics.
- **ASG Activity Logs**: Scaling events, instance lifecycle changes.
- **External Data**: Events, promotions, or seasonality patterns affecting traffic.

**Best Practices:**
- Align all data sources to a common time zone (preferably UTC).
- Store raw metrics in **Amazon S3** for traceability.
- Enable detailed monitoring in CloudWatch for higher granularity (e.g., 1-minute intervals).