---
title: "Train LSTM & ARIMA Models"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 5.1 </b>"
---

Train two types of forecasting models — **LSTM** and **ARIMA** — to predict future traffic patterns for proactive scaling.

**Steps:**
1. **Split Data**: Divide historical metrics into training and validation sets.
2. **Train ARIMA**: Fit a statistical time-series model to capture linear patterns and seasonality.
3. **Train LSTM**: Build a recurrent neural network capable of learning complex, non-linear dependencies in the data.
4. **Hyperparameter Tuning**: Optimize model parameters for accuracy and performance.
5. **Save Models**: Store trained models in **Amazon S3** or directly in **SageMaker Model Registry**.

**Why Both Models?**
- **ARIMA** is simpler and interpretable, suitable for stable, linear patterns.
- **LSTM** handles long-term dependencies and complex seasonal effects.

By training both, we can compare their accuracy and choose the best for deployment.