# Product Requirements

## Objective
Build a secure, reliable platform for AMPG Consult Nigeria covering staffing, learning/training, CRM, marketing and business operations across Android and web.

## Business objectives
- Centralize company information and workflows.
- Support useful work during poor connectivity.
- Improve candidate and learner lifecycle management.
- Connect training outcomes with employment opportunities.
- Give management operational visibility.
- Establish a production-grade Google Play-ready foundation.

## Core modules
### Staffing
Client → Job Request → Candidate Search → Screening → Interview → Shortlist → Placement → Onboarding.

### Learning
Lead → Enrollment → Program → Cohort → Learning → Assessment → Certificate → Career/Placement.

### Marketing/CRM
Lead → Contacted → Qualified → Proposal/Enrollment → Customer/Learner/Client.

## Roles
Super Administrator, Executive/Management, Operations Manager, HR/Staffing Manager, Recruiter, Training Manager, Instructor, Marketing Officer, Finance/Operations Officer, Employee/Staff, Learner, Client.

Roles map to granular permissions. The backend is authoritative.

## Authentication
User authenticates with email/phone/OTP as configured → organization membership is resolved → roles and permissions are resolved → authorized workspaces are shown → initial data sync occurs.

Users do not choose an arbitrary role to gain permissions.

## Offline-first mobile
Previously synchronized records, downloaded learning content, assessments, attendance, notes, drafts, candidate updates and tasks can work offline. Password reset, payment confirmation, some privileged operations, and cloud AI may require connectivity.

## Synchronization
User action → local transaction → sync queue → connectivity → server validation → conflict handling → acknowledgement → local reconciliation.

Visible states: Synced, Offline, Pending sync, Syncing, Sync failed.

## AI
CV/document extraction, candidate-job matching, learner weakness detection, personalized learning, marketing assistance and authorized business summaries. AI recommendations remain reviewable by humans.

## Non-functional requirements
Security, RBAC, encryption, auditability, retry-safe APIs, idempotent sync, automated testing, crash/error monitoring, backups, recovery, observability and low/mid-range Android performance.

## MVP
1. Authentication
2. Organization/users
3. RBAC
4. Android offline foundation
5. Synchronization
6. Web dashboard
7. Staffing core
8. Learning core
9. CRM/lead core
10. Basic reporting
11. Audit logs
12. Production deployment pipeline
