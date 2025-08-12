---
title : "Calculate Desired Capacity & Update ASG"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 7.1 </b> "
---

**Process:**
1. **Receive Prediction Data**: Pull forecast values from the Prediction API.
2. **Determine Desired Capacity**: Translate forecasted traffic into the number of EC2 instances required.
3. **Update ASG Settings**: Use AWS SDK or CLI to set the ASG’s `DesiredCapacity`, `MaxSize`, and `MinSize`.
4. **Apply Guardrails**: Ensure scaling does not exceed budget or drop below minimum safe capacity.
5. **Cooldown Periods**: Add cooldowns to prevent rapid, unnecessary scaling actions.

**Best Practices:**
- Implement safety checks for prediction anomalies.
- Keep logs of all scaling actions for monitoring and auditing.
- Combine predictive scaling with a minimal reactive backup to handle unexpected events.
