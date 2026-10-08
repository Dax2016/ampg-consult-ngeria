# Database Blueprint

Initial domains:

```text
organizations, users, roles, permissions, user_roles, organization_memberships
clients, contacts, leads, tasks
jobs, candidates, candidate_skills, applications, interviews, placements, contracts
programs, courses, modules, lessons, cohorts, learners, enrollments, attendance, assessments, submissions, certificates
campaigns, campaign_leads, marketing_content
documents, notifications, audit_logs, sync_operations
```

A person should not be duplicated unnecessarily. Separate person/profile, user account, organization membership and business roles.

Organization-scoped tables should generally include `organization_id`, `created_at`, `updated_at`, and actor fields where appropriate.
