# FAQ

## Purpose
Answer common cross-product questions for SynapseWorks products.

## Who it is for
- Jira administrators
- Browser extension users and reviewers
- Product owners and delivery managers
- Security and compliance reviewers

## Prerequisites
- Access to this documentation set
- Access to the relevant product environment for checks

## Steps
1. Check product scope first: Jira Apps, Browser Tools, or Android Apps.
2. Match your question to setup, workflow, export, security/data, or privacy topics.
3. If unresolved, follow the support process in [Support](support.md).

## FAQ
### What product groups does SynapseWorks document?
- Jira Apps: Synapse and Decision Register for Jira.
- Browser Tools: Submit Guard Chrome extension.
- Android Apps: RME: Private PDF Scanner.

### Does Synapse replace Atlassian AI or Rovo?
No. Synapse complements Atlassian AI/Rovo by enforcing consistent execution structure through subtasks and validation, instead of only providing suggestions.

### Which app is read-only in Jira?
Decision Register is read-only against Jira issue data and change history.

### Which app can create Jira artefacts?
Synapse can create subtasks from generated requirement previews.

### Where are user preferences stored?
- Decision Register: per-user preferences in Forge storage (`storage:app`).
- Synapse: auto-generate-on-open preference in browser `localStorage`.
- Submit Guard: local extension settings in `chrome.storage.local`.

### Are Jira credentials stored by SynapseWorks Jira apps?
No. Jira credentials are not stored by SynapseWorks Jira apps.

### Is Submit Guard a Jira or Atlassian product?
No. Submit Guard is a Chrome extension for browser workflows.

### Is RME PDF Scanner publicly available on Google Play?
Yes. RME: Private PDF Scanner is publicly available on [Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor). The current stable version is **1.7.1**. The latest stable APK is also available from [GitHub Releases](https://github.com/lucianRME/rme-pdf-scanner/releases/latest). For signing-channel and backup guidance, see [Getting started](../rme-pdf-scanner/getting-started.md).

### Does RME PDF Scanner upload documents to SynapseWorks?
No. RME PDF Scanner processes document content on the device and has no proprietary document backend or cloud library. A user can explicitly save documents in an app-private local library. Files leave the app only when the user chooses an Android SAF destination or Android Sharesheet target.

### Can I move my RME library to another installation or phone?
Yes. Create a portable RME backup, optionally protect it with a password, and choose its destination through Android's system file picker. Confirm that you can access the backup before uninstalling or changing between the differently signed Google Play and GitHub APK channels.

### Does Submit Guard send form contents to SynapseWorks?
No. Submit Guard is local-only, has no SynapseWorks backend, and does not send form contents to SynapseWorks.

## Common issues
- "Feature mismatch": verify whether you are reading the correct product docs (`docs/synapse/*`, `docs/decision-register/*`, `docs/submit-guard/*`, or `docs/rme-pdf-scanner/*`).
- "Permission errors": confirm Jira project permissions and app installation state.
- "Submit Guard does not appear": confirm the extension is installed and enabled for the current site.

## Related pages
- [Documentation index](../index.md)
- [Trust and security overview](trust-security.md)
- [Support](support.md)
- [Synapse security and data](../synapse/security-data.md)
- [Decision Register security and data](../decision-register/security-data.md)
- [Submit Guard privacy](../submit-guard/privacy.md)
- [RME: Private PDF Scanner privacy and support](../rme-pdf-scanner/privacy-and-support.md)
