---
title : "Connect to EC2 servers"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

This section establishes the **baseline scaling configuration** using AWS Auto Scaling Groups (ASG) with standard **reactive policies**.  
Reactive scaling adjusts capacity **after** a metric threshold is breached, serving as the control setup for later comparison with the **predictive scaling** solution.

**3.1 ASG with Target Tracking**  
Create an Auto Scaling Group with target tracking policies that maintain a specific metric (e.g., CPU utilization at 50%).  
When the metric rises above the target, ASG launches additional instances; when it drops, ASG terminates instances.  
This simple approach is easy to implement but reacts only after load changes occur, potentially causing short performance dips.

**3.2 CloudWatch Alarms**  
Set up CloudWatch alarms to monitor key performance metrics like CPU utilization, request count, or custom business metrics.  
These alarms trigger scaling actions when thresholds are exceeded.  
While effective for handling spikes, this method may introduce delays during scale-out events, especially for workloads sensitive to latency.

By completing this reactive setup, we establish a performance and cost baseline to compare against the **ML-powered proactive scaling** approach later in the project.