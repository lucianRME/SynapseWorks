# Decision Register Security and Data

## Purpose
Provide enterprise trust information for Decision Register data access, storage, and runtime.

## Who it is for
- Security, risk, and compliance teams
- Jira administrators approving app access

## Prerequisites
- Access to app scope and permissions review process
- Access to Decision Register behaviour documentation

## Steps
1. Review what data is read from Jira.
2. Confirm that the app is read-only against Jira records.
3. Review runtime and network model.
4. Confirm preference storage behaviour.
5. Record this summary in internal approval notes.

## Data read
- Jira issue change history for selected projects and period
- Jira issue metadata used in output (key and summary)

## Data written
- No writes to Jira issue data
- Per-user run preferences stored in Forge storage

## Runtime and access
- Runs on Atlassian infrastructure as a Forge app
- Uses scopes: `read:jira-work`, `storage:app`
- Jira access is read-only for this app
- No external network calls

## Stored data
- Per-user preferences for run configuration in Forge storage
- Reset-to-defaults support for preference baseline recovery

## Common issues
- Reviewers may assume write access because export exists; export does not write to Jira.
- Preferences are user-scoped; do not assume shared defaults across users.

## Related pages
- [Overview](overview.md)
- [Configuration](configuration.md)
- [Troubleshooting](troubleshooting.md)
