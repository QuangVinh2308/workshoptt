---
title : "Connect to Public Instance"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---
Target Tracking Policies allow an Auto Scaling Group (ASG) to automatically maintain a specific performance metric at a target value, such as keeping average CPU utilization at 50%.

**Implementation Steps:**
1. Create a Launch Template or Launch Configuration for the EC2 instances.
2. Define the desired metric (e.g., CPUUtilization) and set the target value.
3. Attach the target tracking policy to the ASG.
4. Verify that scaling actions occur when the metric goes above or below the target.

**Pros:**
- Easy to configure.
- No need to manage complex scaling logic.

**Cons:**
- Reacts only **after** the metric changes.
- May cause performance dips during sudden load spikes.