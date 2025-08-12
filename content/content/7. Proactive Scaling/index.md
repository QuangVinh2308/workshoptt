---
title : "Proactive Scaling"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 7. </b> "
---

This section explains how to use **ML predictions** to proactively adjust Auto Scaling Group (ASG) capacity before demand spikes occur.  
By acting ahead of time, proactive scaling minimizes latency, improves user experience, and optimizes infrastructure cost.

The scaling logic takes predictions from the **real-time API** and updates the ASG desired capacity, maximum, and minimum limits accordingly.