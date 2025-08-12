---
title : "Real-time Inference API"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 6.2 </b> "
---

Provide a REST API for on-demand traffic predictions.

**Core Features:**
- Accepts a forecast request specifying the time horizon (e.g., next 15 minutes).
- Runs inference using the deployed model.
- Returns predicted traffic metrics in JSON format.

**Implementation Notes:**
- Use **AWS API Gateway** to expose the endpoint.
- Integrate with AWS Lambda or directly with the SageMaker endpoint.
- Add authentication and rate limiting for security.
- Log all requests and responses for analysis and debugging.