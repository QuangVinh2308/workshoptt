---
title : "Remove Resources"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 9.1 </b> "
---

**Steps:**
1. **Delete Auto Scaling Groups (ASG)**: Remove or disable associated scaling policies.
2. **Terminate EC2 Instances**: Ensure they are no longer in use.
3. **Remove CloudWatch Alarms**: Delete any alarms created for testing.
4. **Delete SageMaker Endpoints & Models**: Prevent ongoing hosting costs.
5. **Clean Up S3 Buckets**: Remove datasets and model artifacts, or archive if needed.
6. **Revoke IAM Roles & Policies**: Remove unused permissions to improve security.

**Best Practices:**
- Double-check billing reports to confirm resources are no longer incurring charges.
- Keep a list of deleted resources for documentation and auditing.