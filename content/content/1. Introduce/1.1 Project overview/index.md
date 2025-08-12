---
title: "Project Overview"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 1.1 </b>"
---

This project develops an **intelligent Auto Scaling system** that uses **Machine Learning** to predict application traffic and scale AWS resources **proactively**.

Instead of waiting for spikes and reacting late, the system **forecasts workload** using:
- **Amazon CloudWatch metrics** (CPU, requests, network, custom),
- **External data sources** (campaigns, seasonality, events),
- **Custom forecasting algorithms**: **LSTM** and **ARIMA**.

A **real-time prediction API** serves the forecasts to the scaling logic, which updates **Auto Scaling Groups (ASG)** ahead of demand (desired/min/max capacity, cooldown guardrails).  
This approach aims to **reduce latency**, **improve uptime**, and **cut costs** versus traditional reactive scaling.

We will run **A/B testing** (Reactive vs Predictive) on real traffic, and produce detailed **accuracy reports** (MAPE, RMSE) plus a **cost-saving analysis** to quantify the benefits.
