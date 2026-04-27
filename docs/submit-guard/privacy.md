# Submit Guard Privacy

## Purpose
Document Submit Guard data handling for users, teams, and privacy reviewers.

## Who it is for
- Submit Guard users
- Security, privacy, and compliance reviewers
- Teams approving browser extension use

## Prerequisites
- Understanding that Submit Guard is a Chrome extension
- Access to the extension settings for the browser profile being reviewed

## Summary
Submit Guard is local-only.

- No SynapseWorks backend is used.
- No SynapseWorks account is required.
- Form contents are not sent to SynapseWorks.
- Form contents are not stored by the extension.
- Settings are stored locally in `chrome.storage.local`.

Website privacy page: [Submit Guard Privacy Policy](https://synapseworks.org/privacy/submit-guard/)

## Data processed locally
Submit Guard may inspect page content locally in the browser to decide whether to show a confirmation dialog. This inspection happens on the device and is used only for the extension's guard behaviour.

## Data stored locally
Submit Guard stores configuration data locally, such as:

- Per-site enablement settings
- Mode selections
- Configured risky phrase list, if used
- Local counters used by the extension

## Data not collected by SynapseWorks
- Form contents
- Submitted values
- Account credentials
- Remote analytics from form pages

## Third parties
Submit Guard does not use third-party analytics, remote code, or ads.

## Common issues
- Local settings are browser-profile specific.
- Uninstalling the extension removes locally stored extension settings according to normal browser extension behaviour.
- Enterprise-managed browsers may apply additional extension policies controlled by the organization.

## Related pages
- [Overview](overview.md)
- [How it works](how-it-works.md)
- [Troubleshooting](troubleshooting.md)
- [Trust and security overview](../common/trust-security.md)
