# Trust & Security Overview

## Purpose
Provide a single trust and security overview for the SynapseWorks product portfolio.

## Who it is for
- Security, risk, and compliance teams
- Jira administrators approving rollout
- Browser extension reviewers
- Procurement and governance stakeholders

## Prerequisites
- Access to the product-specific documentation for the product being reviewed
- For Jira apps: understanding of your Jira permission and data governance model
- For browser tools: understanding of your browser extension policy and local device controls

## Steps
1. Start with this overview for shared vendor and compliance context.
2. Review each product-specific security, data, or privacy page for full operational detail.
3. Map responsibilities below into your internal approval process.
4. Record the privacy policy link in your governance artefacts.

## Product-specific pages
- [Synapse security and data](../synapse/security-data.md)
- [Decision Register security and data](../decision-register/security-data.md)
- [Submit Guard privacy](../submit-guard/privacy.md)

## Privacy and compliance statement
SynapseWorks provides privacy-first workflow tools with documented product-specific data handling.
Security and compliance are a shared responsibility:
- SynapseWorks is responsible for app-level controls, documented runtime behaviour, and credential handling controls.
- Customers are responsible for Jira permissions, project configuration, browser extension policies, local device controls, retention policies, and internal compliance governance.

## Data handling summary
### Jira Apps
Synapse and Decision Register are Jira/Atlassian products.

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

### Browser Tools
Submit Guard is a Chrome extension. It is not a Jira app and does not run on Atlassian.

### Submit Guard
- Data processed locally:
  - Page content needed to decide whether to show a confirmation
  - Current-site state needed for per-site enablement
- Data stored locally:
  - Per-site enablement settings
  - Mode selections
  - Configured risky phrase list, if used
  - Local counters used by the extension
- Runtime notes:
  - Local-only Chrome extension
  - No SynapseWorks backend
  - No SynapseWorks account
  - Form contents are not sent to SynapseWorks
  - Form contents are not stored by the extension

## Credential handling confirmation
- Jira credentials are not stored by SynapseWorks Jira apps.
- Sensitive credentials are not stored externally by SynapseWorks Jira apps.
- Decision Register is read-only against Jira issue data.
- Submit Guard does not require a SynapseWorks account and does not send form contents to SynapseWorks.

## Privacy policy
- [SynapseWorks Privacy Policy](https://synapseworks.org/privacy/)
- [Submit Guard Privacy Policy](https://synapseworks.org/privacy/submit-guard/)

## Example review checklist
- Confirm required Jira scopes or browser permissions match your approved access model.
- Confirm product storage locations (`storage:app`, browser `localStorage`, Chrome `chrome.storage.local`) are acceptable.
- Confirm behaviour aligns with expected product function:
  - Synapse may create subtasks.
  - Decision Register does not write to Jira issue data.
  - Submit Guard confirms browser submissions locally and does not send form contents to SynapseWorks.

## Common issues
- Teams review app pages in isolation and miss shared governance expectations.
- Browser-side storage (`localStorage`) is sometimes omitted from risk assessments.
- Read-only status can be misunderstood when export functions are present.
- Portfolio-wide claims can be inaccurate; review each product boundary separately.

## Related pages
- [Documentation index](../index.md)
- [FAQ](faq.md)
- [Support](support.md)
