# Platform Security and Data (SaaS)

## Purpose
Summarise security and data-handling controls for the Synapse platform documentation track.

## Who it is for
- Security and compliance reviewers
- Platform operators
- Stakeholders assessing governance readiness

## Prerequisites
- Access to platform workflow documentation
- Internal policy context for transcript and requirement data

## Steps
1. Review data ingress, processing, storage, and export points.
2. Confirm controls for authentication, rate limiting, and host validation.
3. Confirm operational endpoint coverage for governance artefacts.
4. Record approved controls in internal review output.

## Data handled
- Transcript uploads (`.vtt`, `.txt`)
- Processed transcript content after cleanup and optional small-talk filtering
- Structured requirements and generated BDD or Gherkin scenarios
- Session and review state with approval actions

## Storage and export
- Session-aware persistence to SQLite and JSON
- CSV export for downstream analysis or reporting

## Integration and hardening
- Jira Cloud sync supports idempotency and optional linking
- Hardening controls include authentication, rate limiting, payload limits, host validation, and license hooks
- Operational endpoints include health checks, privacy, cookies, `robots.txt`, and sitemap

## Common issues
- Review scope may omit operational endpoints; include them in compliance checks.
- Data retention policy alignment should be confirmed for SQLite and JSON persistence.

## Related pages
- [Overview](overview.md)
- [Pipeline](pipeline.md)
- [Support](../common/support.md)
