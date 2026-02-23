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

## First success checklist
- Use an issue with clear problem and acceptance context in the summary or description.
- Generate preview before opening `Refine with Synapse`.
- Run dry-run first and confirm all items show `would be created`.
- Run create-subtasks mode only after dry-run is clean.
- Capture created issue keys for traceability.

## Copy-paste acceptance criteria example
Paste this into a Jira issue description, then generate preview in Synapse.

```text
Acceptance Criteria
1. Given a user can access the password reset page, when they submit a valid email, then a reset email is sent.
2. Given a reset link is expired, when the user opens the link, then an expiry message is shown and a new link can be requested.
3. Given a user provides a valid new password, when they confirm it, then the password is updated and old sessions are revoked.
4. Given reset processing fails, when the request is submitted, then the user sees a retry message and the failure is logged.
```

## What good looks like
- Preview output is grouped and each item has executable BDD-style scenarios.
- Dry-run validates the creation path with no unexpected failures.
- Create-subtasks returns created keys and no blocking errors.

## Common mistakes
- Running create-subtasks mode before dry-run.
- Using minimal issue context, which reduces preview quality.
- Expecting dry-run to create Jira records.
- Missing permission to create subtasks in the target project.

## Common issues
- "No preview output": verify issue summary and description quality.
- "Dry-run passes but nothing is created": this is expected in dry-run mode.
- "Some subtasks failed": check returned per-item errors and rerun after correction.

## Related pages
- [Overview](overview.md)
- [Workflow](workflow.md)
- [Troubleshooting](troubleshooting.md)
