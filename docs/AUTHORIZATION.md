# Authentication and Authorization

Authentication answers: **Who are you?**

Authorization answers: **What are you allowed to do here?**

Recommended identity provider: Amazon Cognito.

Use RBAC plus granular permissions such as:

```text
candidate.read
candidate.create
candidate.update
job.read
job.create
learner.read
learner.assess
learner.grade
campaign.read
campaign.create
campaign.publish
```

Organization isolation and server-side permission checks are mandatory.
