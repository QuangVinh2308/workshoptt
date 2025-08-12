---
title: "Modeling"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 5. </b>"
---

This section covers the implementation of **forecasting models** for predicting traffic patterns.  
We use two approaches — **ARIMA** (statistical) and **LSTM** (deep learning) — to compare accuracy and select the best model for deployment.

The process includes:
1. Preparing time-series data.
2. Training both ARIMA and LSTM models.
3. Evaluating accuracy using MAPE and RMSE.
4. Selecting the optimal model for proactive scaling.