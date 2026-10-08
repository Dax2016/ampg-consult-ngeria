# Security Baseline

- TLS for all network traffic
- Managed authentication
- Short-lived sessions/tokens
- Server-side authorization
- Organization isolation
- Encryption at rest where supported
- Secure Android local storage
- Secrets outside Git
- Audit logs
- Rate limiting
- Input/file validation
- Backup and recovery
- Least-privilege IAM

Never commit AWS keys, API keys, database passwords, JWT secrets, production `.env` files or private certificates.
