# Decision Register Detections

## Purpose
Document which Jira change events are detected and how each entry is represented.

## Who it is for
- Audit and compliance teams
- PMO and delivery governance leads
- Jira administrators validating reporting scope

## Prerequisites
- Decision Register run output or test project history
- Understanding of Jira field usage in your projects

## Steps
1. Run Decision Register on a project and period with known change activity.
2. Review entries by detection type.
3. Validate `from` and `to` transitions against source issue history.
4. Export results for review evidence if required.

## Detection types
- Estimate changes
- Priority changes
- Scope or sprint changes
- Status rollback or reopen events
- Assignee changes
- Due date changes
- Release or fix version changes

## Entry format
Each entry includes:
- Issue key
- Issue summary
- When the change happened
- Who made the change
- Previous value (`from`)
- New value (`to`)

## Common issues
- Field naming differences can affect estimate interpretation; use estimate field override when needed.
- Teams may treat reopen patterns differently; align operational definition before audit reporting.

## Related pages
- [Configuration](configuration.md)
- [Export](export.md)
- [Troubleshooting](troubleshooting.md)
