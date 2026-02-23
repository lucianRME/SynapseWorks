# Synapse Quickstart

## Purpose
Run your first end-to-end Synapse flow from issue context to validated creation output.

## Who it is for
- Jira users and delivery leads
- Jira administrators validating rollout readiness

## Prerequisites
- Synapse installed and enabled in Jira
- Access to a Jira issue with enough context in summary or description
- Permission to create subtasks (for create-subtasks mode)

## Steps
1. Open a Jira issue and launch the Synapse panel.
2. Generate a preview from issue context.
3. Review grouped requirements and BDD-style scenarios.
4. Open `Refine with Synapse` for edits if needed.
5. Use dry-run to validate the creation path (`would be created`).
6. Run create-subtasks mode to create linked subtasks.
7. Record created issue keys and any returned errors.

## Example
- Parent issue: `PROJ-123`
- Action: generate preview, refine two items, run dry-run, then create subtasks
- Result: created keys returned in the panel for traceability

## Common issues
- "No preview output": verify issue summary and description quality.
- "Dry-run passes but nothing is created": this is expected in dry-run mode.
- "Some subtasks failed": check returned per-item errors and rerun after correction.

## Related pages
- [Overview](overview.md)
- [Workflow](workflow.md)
- [Troubleshooting](troubleshooting.md)
