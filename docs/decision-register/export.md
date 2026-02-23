# Decision Register Export

## Purpose
Explain how to extract register results for governance, audit, and operational reporting.

## Who it is for
- PMO and compliance teams
- Jira administrators and delivery managers

## Prerequisites
- Completed Decision Register run with visible results

## Steps
1. Run Decision Register with the required filters.
2. Review grouped or table output before export.
3. Export results to CSV for structured reporting.
4. If CSV is unavailable in your environment, use copy-to-clipboard fallback.
5. Store exported output according to your internal policy.

## Export content
- Detection entries with issue key, summary, when, who, from, and to
- Run metadata and counts available in UI for context

## Common issues
- CSV download blocked by endpoint policy: use clipboard fallback.
- Missing context in downstream reports: include run metadata and filter settings with the export.

## Related pages
- [Quickstart](quickstart.md)
- [Configuration](configuration.md)
- [Troubleshooting](troubleshooting.md)
