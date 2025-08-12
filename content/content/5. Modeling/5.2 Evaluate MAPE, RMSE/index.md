---
title: "Evaluate MAPE, RMSE"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 5.2 </b>"
---

Evaluate the trained models to determine which provides the most accurate and reliable predictions.

**Evaluation Metrics:**
- **MAPE (Mean Absolute Percentage Error)**: Measures prediction accuracy as a percentage, useful for business interpretation.
- **RMSE (Root Mean Square Error)**: Penalizes larger errors, useful for detecting severe prediction mismatches.

**Process:**
1. Run both models on the validation dataset.
2. Compare MAPE and RMSE scores.
3. Select the model with the best balance between accuracy and robustness.
4. Document results for later inclusion in the final accuracy report.

Choosing the most accurate model ensures that proactive scaling decisions are based on reliable forecasts, reducing the risk of over-provisioning or under-provisioning.