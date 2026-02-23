# Synapse Troubleshooting

## Purpose
Resolve common operational issues in preview, refine, dry-run, and create-subtasks flows.

## Who it is for
- Jira administrators
- Support and operations teams
- Delivery users running Synapse in day-to-day work

## Prerequisites
- Access to affected Jira issue
- Access to Synapse panel output or error messaging

## Steps
1. Identify the failing stage: preview, refine, dry-run, or create-subtasks.
2. Capture issue key, timestamp, and exact error output.
3. Validate expected behaviour against this page.
4. Apply the suggested corrective action.
5. Escalate through support if the issue persists.

## Common issues
- Panel does not load:
  - Check that Synapse is installed and the issue panel is available.
- Preview quality is poor:
  - Improve issue summary and description clarity before regenerating.
- Refine guidance appears unexpectedly:
  - Generate preview first, then reopen refine.
- Dry-run shows success but no subtasks exist:
  - Expected behaviour; dry-run does not create records.
- Partial subtask creation:
  - Review returned error details per item, then rerun after corrections.

## Related pages
- [Quickstart](quickstart.md)
- [Workflow](workflow.md)
- [Support](../common/support.md)
