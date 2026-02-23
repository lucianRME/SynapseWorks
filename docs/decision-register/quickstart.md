# Decision Register Quickstart

## Purpose
Run your first Decision Register report and export the results.

## Who it is for
- Jira administrators
- Delivery and governance leads

## Prerequisites
- Decision Register installed and accessible in Jira
- Access to target Jira projects

## Steps
1. Open Decision Register from the Jira Global Page or Admin Page.
2. Select one or more projects using search and filter.
3. Set the time range and max issues scanned.
4. Optionally filter by issue type and only-my-changes.
5. Run the register.
6. Review grouped or table output, counts, metadata, and issue links.
7. Export to CSV, or use copy-to-clipboard fallback if needed.

## Example
- Projects: `OPS`, `ENG`
- Range: last 30 days
- Filters: `Story`, `Bug`, only-my-changes off
- Output: grouped by change type, exported to CSV for governance review

## Common issues
- No entries found: widen the time range or project selection.
- Scan too broad: reduce max issues or narrow issue types.
- Clipboard fallback needed: use when CSV download is blocked by local policy.

## Related pages
- [Overview](overview.md)
- [Configuration](configuration.md)
- [Export](export.md)
