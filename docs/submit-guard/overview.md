# Submit Guard Overview

## Purpose
Explain what Submit Guard does and where it fits in everyday browser workflows.

## Who it is for
- People who want an extra confirmation step before sending web forms
- Teams that use sensitive or irreversible web workflows
- Security and privacy reviewers assessing extension behaviour

## Prerequisites
- Chrome or a Chromium-based browser
- Submit Guard installed from the Chrome Web Store
- A site where you want confirmation before submit

## Product type
Submit Guard is a Chrome extension. It is not a Jira app, not an Atlassian Marketplace app, and does not run on Atlassian Forge.

Website: [Submit Guard product page](https://synapseworks.org/products/submit-guard/)

## Capability summary
- Adds a confirmation step before form submissions on sites you enable
- Standard mode confirms native HTML form submissions
- Advanced mode can guard submit-like clicks in modern web apps when enabled
- Per-site controls let you decide where Submit Guard runs
- Local settings are stored in `chrome.storage.local`
- No SynapseWorks account is required
- No SynapseWorks backend is used
- Form contents are not sent to SynapseWorks

## Privacy summary
Submit Guard is local-only. It may inspect page content in your browser to decide whether to show a confirmation, but it does not transmit form contents to SynapseWorks and does not store form contents.

## Common issues
- Submit Guard is disabled for the current site.
- The site uses a custom submit-like button that may require advanced mode.
- Browser extension permissions or site restrictions prevent injection on the current page.

## Related pages
- [Install](install.md)
- [How it works](how-it-works.md)
- [Privacy](privacy.md)
- [Troubleshooting](troubleshooting.md)
- [Documentation index](../index.md)
