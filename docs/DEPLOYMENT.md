# Deployment Blueprint

## Environments
Development → CI → Staging → Acceptance → Production.

## Backend
Containerized FastAPI on ECS/Fargate, RDS PostgreSQL, S3, CloudWatch and Secrets Manager/Parameter Store.

## Android
Local development → Internal testing → Closed testing → Production on Google Play.

## Release gates
Automated tests, security checks, offline/network testing, performance checks, release signing, privacy policy, Terms, data safety declaration, store assets, crash/ANR monitoring and rollback procedure.

Production secrets are never committed.
