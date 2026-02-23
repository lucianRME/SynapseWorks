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

## First success checklist
- Start with one active project where issue history is known.
- Use a practical window (for example last 30 days).
- Set max issues scanned high enough for useful coverage.
- Keep filters light on first run (issue types only, only-my-changes off).
- Check grouped/table results before exporting.

## Copy-paste run setup example
Use this setup for a reliable first run.

```text
Projects: ENG
Time range: Last 30 days
Max issues scanned: 200
Issue types: Story, Bug
Only my changes: Off
Estimate field: Auto-detect
```

What the output means:
- Each entry shows issue key, summary, when, who, and the `from` to `to` change.
- Grouped view shows change-type counts; table view is useful for detailed review.
- Run metadata confirms scope (project, range, limits) used for that output.

## What good looks like
- Results include multiple valid change entries with issue links for verification.
- Change-type counts and run metadata match your selected scope.
- CSV export works, or clipboard fallback is used when download is blocked.

## Common mistakes
- Using a very short time range and assuming no changes exist.
- Setting max issues scanned too low for the selected project.
- Over-filtering issue types on the first run.
- Assuming export writes back to Jira issue data.

## Common issues
- No entries found: widen the time range or project selection.
- Scan too broad: reduce max issues or narrow issue types.
- Clipboard fallback needed: use when CSV download is blocked by local policy.

## Related pages
- [Overview](overview.md)
- [Configuration](configuration.md)
- [Export](export.md)
