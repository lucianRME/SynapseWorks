# Submit Guard How It Works

## Purpose
Describe the Submit Guard behaviour model without implying remote processing or SynapseWorks server involvement.

## Who it is for
- Users configuring Submit Guard
- Security reviewers checking extension behaviour
- Support teams diagnosing missed confirmations

## Prerequisites
- Submit Guard installed
- Submit Guard enabled for the target site
- Basic understanding of the site's form workflow

## Steps
1. Submit Guard checks whether the current site is enabled in your local settings.
2. If enabled, the extension runs local browser logic on that page.
3. Standard mode watches for native HTML form submissions.
4. Advanced mode can also watch for submit-like clicks in modern web apps.
5. When a guarded action is detected, Submit Guard shows a confirmation step before the action proceeds.
6. If you confirm, the submission continues.
7. If you cancel, the submission is stopped.

## Runtime model
- Runs inside the browser extension environment
- Uses local browser APIs and locally stored settings
- Does not call a SynapseWorks backend
- Does not require a SynapseWorks account
- Does not send form contents to SynapseWorks

## Modes
### Standard mode
Use standard mode first. It is intended for native HTML form submissions.

### Advanced mode
Use advanced mode when a modern web app uses buttons or scripts that behave like form submission without using a native form submit event.

## Common issues
- Some web apps intercept or replace browser events in ways that require advanced mode.
- Some browser pages and extension-restricted URLs cannot be guarded by normal extension scripts.
- Confirmation appears only on sites where Submit Guard is enabled.

## Related pages
- [Overview](overview.md)
- [Install](install.md)
- [Privacy](privacy.md)
- [Troubleshooting](troubleshooting.md)
