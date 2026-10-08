# Product Architecture

```text
                         AWS CLOUD
                             |
                +------------+------------+
                |                         |
        Android App                  Web Application
       Kotlin/Compose                Next.js/TypeScript
        Offline-first                  Online-first
                |                         |
                +------------+------------+
                             |
                       FastAPI Backend
                             |
          +------------------+------------------+
          |                  |                  |
      PostgreSQL             S3             AI Gateway
                                             |
                                           Bedrock
```

## Android
Kotlin, Jetpack Compose, Room, WorkManager, secure local storage, connectivity monitoring.

UI → ViewModel → Use Cases → Repository → Local/Remote data sources.

## Web
Next.js + TypeScript. Responsive management/operations experience.

## Backend
Python + FastAPI + Pydantic + SQLAlchemy + Alembic + PostgreSQL. Start as a modular monolith; split services only when justified.

Suggested modules: auth, organizations, users, roles, permissions, CRM, staffing, learning, marketing, documents, notifications, reports, sync, AI, audit.

## AWS
Cognito, API Gateway/ALB, ECS/Fargate, RDS PostgreSQL, S3, CloudFront, SQS/EventBridge, CloudWatch, Secrets Manager/Parameter Store and Bedrock.

## Data ownership
PostgreSQL is authoritative for business data. Room is the local replica/offline operation store. S3 is authoritative for uploaded binary objects.

## Security
Every protected API request validates identity, organization membership, permission and resource scope. Never trust client-supplied roles.
