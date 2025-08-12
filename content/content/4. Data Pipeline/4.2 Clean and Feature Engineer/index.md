---
title: "Clean and Feature Engineer"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 4.2 </b>"
---

Prepare raw metrics for machine learning by cleaning and enriching the data.

**Key Steps:**
1. **Handle Missing Data**: Fill gaps using forward fill, backward fill, or interpolation.
2. **Remove Outliers**: Detect abnormal spikes/drops that are not traffic-related.
3. **Aggregate Data**: Resample metrics to consistent intervals (e.g., 5 or 15 minutes).
4. **Feature Engineering**: Add time-based features such as hour of day, day of week, and seasonality indicators.

A clean and feature-rich dataset ensures that the forecasting models (LSTM/ARIMA) can learn meaningful patterns for accurate predictions.