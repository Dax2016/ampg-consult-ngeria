# AMPG Consult Platform

Production-oriented mobile-first and web-enabled consulting platform for AMPG Consult Nigeria.

## Product
- Staffing and recruitment
- Learner/training management
- CRM and marketing
- Business operations and analytics
- AI-assisted workflows

## Architecture
Android (Kotlin/Compose, offline-first) + Web (Next.js/TypeScript) → FastAPI → PostgreSQL/S3 → AWS AI/services.

## First vertical slice
Login → authentication → organization/role resolution → dashboard → offline operation → local change → reconnect → sync → web verification.

See `docs/` for the complete product requirements, architecture, database, security, AI, offline-sync, deployment, legal drafts, and Google Play checklist.

> Legal documents are starter drafts and require qualified Nigerian legal review before production publication.
