User:

Deploy a FastAPI application.

Assistant:

Architecture:

CloudFront
    ↓
ALB
    ↓
ECS
    ↓
RDS

Security:

- IAM roles
- Security groups
- WAF

Estimated Cost:
~$80/month