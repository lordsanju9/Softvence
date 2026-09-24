# Deployment & Operations — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Environments
- Development.
- Staging/demo.

A separate production environment is out of scope and must not be assumed in the fixed price.

## CI/CD

Minimum pipeline:
- Build.
- Unit tests.
- Integration tests.
- Dependency/security scan.
- Staging deployment.

## Infrastructure

Use managed cloud services where practical. The prototype does not require multi-region infrastructure or complex autoscaling.

## Monitoring

Basic monitoring shall cover:
- API availability.
- Blockchain provider errors.
- AI tool failures.
- Transaction workflow errors.

## Handover

Client receives:
- Source repository.
- Deployment instructions.
- Environment variable documentation.
- Architecture documentation.
- Test results.
- Runbook for common failures.

Third-party accounts should be owned or controlled by Client where practical.
