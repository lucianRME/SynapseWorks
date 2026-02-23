# Decision Register Overview

## Purpose
Explain how Decision Register creates an audit-style history from Jira issue change events.

## Who it is for
- Jira administrators and project leads
- PMO, governance, and audit teams
- Engineering managers reviewing delivery drift

## Prerequisites
- Decision Register app installed on Jira Cloud
- Access to Jira projects and issue history data

## Steps
1. Open Decision Register from the Jira Global Page or Admin Page.
2. Configure run filters for scope and period.
3. Run a scan to generate decision entries from issue history.
4. Review grouped or table output, counts, and metadata.
5. Export results for reporting or audit sharing.

## Capability summary
- Forge app exposed as Jira Global Page and Admin Page
- Generates audit-style register from issue change history
- Detects estimate, priority, scope or sprint, rollback or reopen, assignee, due date, and release or fix version changes
- Entry fields include issue key, summary, when, who, from, and to
- Supports run filters: project selection, time range, max issues scanned, issue types, and only-my-changes
- Estimate field handling supports auto-detect and optional `customfield` override
- Results in grouped or table views with per-group visibility controls
- Type counts and run metadata included
- Issue links in results for fast verification
- Export options: CSV plus fallback copy-to-clipboard
- Per-user preferences persisted in Forge storage with reset-to-defaults
- Resilience includes retries for rate-limit and server errors, first-run init message, and partial-result warnings

## Rovo positioning
Decision Register complements Atlassian AI/Rovo by adding structured, auditable change evidence for governance and operational review.

## Common issues
- Empty output is often caused by narrow filter scope or short time windows.
- Large scans can return partial warnings; use run metadata and rerun with adjusted limits.

## Related pages
- [Quickstart](quickstart.md)
- [Detections](detections.md)
- [Configuration](configuration.md)
- [Export](export.md)
- [Security and data](security-data.md)
- [Troubleshooting](troubleshooting.md)
- [Documentation index](../index.md)
