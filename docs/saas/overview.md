# Platform Overview (SaaS)

## Purpose
Describe the Synapse platform capability track separate from Marketplace app functionality.

## Who it is for
- Platform evaluators
- Product and operations stakeholders
- Teams planning transcript-to-requirement workflows

## Prerequisites
- Understanding that this section documents platform capabilities and roadmap context, not Marketplace app behaviour unless explicitly stated

## Steps
1. Use this section for platform workflow and controls.
2. Use `docs/synapse/*` and `docs/decision-register/*` for Marketplace app behaviour.
3. Align rollout expectations by keeping platform and app scope separate.

## Scope statement
This section documents Synapse SaaS capabilities as platform context. It is not a statement that these capabilities are available as Atlassian Marketplace app features unless explicitly stated elsewhere.

## Capability summary
- Transcript upload and drag-drop for `.vtt` and `.txt`
- Transcript cleanup and optional small-talk filtering
- Structured requirement extraction
- BDD and Gherkin scenario generation with validation and deduplication
- Human review UI with approval controls and bulk approval
- Session-aware workflow with persistence to SQLite and JSON
- CSV export support
- Jira Cloud sync with idempotency and optional linking
- Hardening controls: auth, rate limiting, payload limits, host validation, and license hooks
- Operations endpoints: health checks, privacy, cookies, `robots.txt`, and sitemap

## Common issues
- Platform capabilities are sometimes assumed to be in Jira apps; verify product scope first.
- Governance reviews often need both platform and app security pages for full context.

## Related pages
- [Pipeline](pipeline.md)
- [Security and data](security-data.md)
- [Documentation index](../index.md)
