---
title : "Connect to Private instance"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 3.2. </b> "
---
CloudWatch Alarms trigger scaling actions when a monitored metric crosses a predefined threshold.

**Implementation Steps:**
1. Choose the metric to monitor (e.g., CPU utilization, request count).
2. Set a threshold value (e.g., CPU > 70% for 5 minutes).
3. Configure the alarm to execute a scaling policy when triggered.
4. Test the alarm by generating traffic or adjusting thresholds temporarily.

**Pros:**
- Allows scaling based on any measurable CloudWatch metric.
- Flexible thresholds for different workloads.

**Cons:**
- Scaling happens **after** the threshold is breached.
- May result in slower response to sudden traffic surges compared to predictive scaling.