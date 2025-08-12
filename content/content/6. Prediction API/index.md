---
title : "Prediction API"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 6. </b> "
---


WThis section describes how to deploy the selected forecasting model into a production environment and serve real-time predictions.

The API will:
1. Receive a request for upcoming traffic forecasts.
2. Run the model inference.
3. Return the predicted values to the scaling logic.