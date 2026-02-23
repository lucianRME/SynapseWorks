# Trust & Security Overview

## Purpose
Provide a single trust and security overview for SynapseWorks Atlassian Marketplace apps.

## Who it is for
- Security, risk, and compliance teams
- Jira administrators approving rollout
- Procurement and governance stakeholders

## Prerequisites
- Access to Synapse and Decision Register documentation
- Understanding of your Jira permission and data governance model

## Steps
1. Start with this overview for shared vendor and compliance context.
2. Review each app-specific security page for full operational detail.
3. Map responsibilities below into your internal approval process.
4. Record the privacy policy link in your governance artefacts.

## App-specific security pages
- [Synapse security and data](../synapse/security-data.md)
- [Decision Register security and data](../decision-register/security-data.md)

## Privacy and compliance statement
SynapseWorks provides Marketplace apps with least-privilege scopes and documented data handling.  
Security and compliance are a shared responsibility:
- SynapseWorks is responsible for app-level controls, documented runtime behaviour, and credential handling controls.
- Customers are responsible for Jira permissions, project configuration, retention policies, and internal compliance governance.

## Data handling summary (Marketplace apps)
### Synapse
- Data read:
  - Jira issue summary
  - Jira issue description (ADF and plain text)
  - Jira comments
  - Jira labels
  - Jira issue type
  - Jira project information
- Data written:
  - Subtasks linked to the current issue (create-subtasks mode only)
  - Creation status output in UI (created keys and errors)
- Storage/runtime notes:
  - Auto-generate preference in browser `localStorage`
  - Atlassian-hosted Forge runtime (Runs on Atlassian eligible)
  - No external backend or external storage for Synapse
  - Redacted logs for sensitive fields

### Decision Register
- Data read:
  - Jira issue change history for selected projects and period
  - Jira issue metadata used in output (issue key and summary)
- Data written:
  - No writes to Jira issue data
  - Per-user run preferences in Forge storage
- Storage/runtime notes:
  - Runs on Atlassian infrastructure as a Forge app
  - No external network calls

## Credential handling confirmation
- Jira credentials are not stored by SynapseWorks Marketplace apps.
- Sensitive credentials are not stored externally by these apps.
- Decision Register is read-only against Jira issue data.

## Privacy policy
- [SynapseWorks Privacy Policy](https://synapseworks.org/privacy/)

## Example review checklist
- Confirm required scopes match your approved access model.
- Confirm app storage locations (`storage:app` and `localStorage`) are acceptable.
- Confirm write behaviour aligns with expected app function:
  - Synapse may create subtasks.
  - Decision Register does not write to Jira issue data.

## Common issues
- Teams review app pages in isolation and miss shared governance expectations.
- Browser-side storage (`localStorage`) is sometimes omitted from risk assessments.
- Read-only status can be misunderstood when export functions are present.

## Related pages
- [Documentation index](../index.md)
- [FAQ](faq.md)
- [Support](support.md)
