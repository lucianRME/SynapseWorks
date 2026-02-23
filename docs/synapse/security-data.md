# Synapse Security and Data

## Purpose
Provide a clear security and data-handling view for enterprise review.

## Who it is for
- Security, risk, and compliance teams
- Jira administrators approving app rollout

## Prerequisites
- Access to Synapse functional documentation
- Understanding of your Jira permission model

## Steps
1. Confirm what data Synapse reads from Jira issue context.
2. Confirm when Synapse writes data back to Jira.
3. Review runtime and token model.
4. Confirm what preferences are stored and where.
5. Include this page in internal security approval records.

## Data read
- Jira issue summary
- Jira issue description (ADF and plain text)
- Jira comments
- Jira labels
- Jira issue type
- Jira project information

## Data written
- Subtasks linked to the current issue (only in create-subtasks mode)
- Creation status outputs in UI (created keys and errors)

## Runtime and auth model
- Runs as a Forge app in the Atlassian-hosted runtime (Runs on Atlassian eligible)
- Synapse runs fully on Atlassian Forge with no external backend or external storage.
- Uses minimal scopes: `read:jira-work`, `write:jira-work`, `read:app-user-token`
- Jira credentials are not stored

## Stored data
- Browser `localStorage`: auto-generate-on-open preference
- Logs: redacted logging approach for sensitive fields

## Common issues
- Security reviews often miss browser-side storage; include `localStorage` in assessments.
- Write permissions are required for create-subtasks mode.

## Related pages
- [Overview](overview.md)
- [Configuration](configuration.md)
- [Troubleshooting](troubleshooting.md)
