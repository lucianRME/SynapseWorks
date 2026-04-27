# Submit Guard Install

## Purpose
Install Submit Guard and enable it on the sites where you want submit confirmation.

## Who it is for
- Chrome users installing Submit Guard
- Teams validating extension rollout steps
- Support teams checking installation state

## Prerequisites
- Chrome or a Chromium-based browser
- Permission to install Chrome extensions
- Access to the site where you want to enable Submit Guard

## Steps
1. Open the [Submit Guard product page](https://synapseworks.org/products/submit-guard/).
2. Follow the Chrome Web Store install link.
3. Install the extension in Chrome.
4. Open a site where you want Submit Guard protection.
5. Enable Submit Guard for that site.
6. Choose standard mode first.
7. Use advanced mode only when the site uses submit-like clicks that standard mode does not catch.
8. Test with a non-sensitive form or safe test workflow before relying on it for important submissions.

## What is configured locally
- Per-site enablement settings
- Mode selections
- Risky phrase settings, if configured
- Local counters used by the extension

These settings are stored locally in `chrome.storage.local`.

## Common issues
- The extension is installed but not enabled for the current site.
- The browser profile does not allow extensions on the target page.
- Advanced mode is needed for modern web apps that do not use native form submission.

## Related pages
- [Overview](overview.md)
- [How it works](how-it-works.md)
- [Privacy](privacy.md)
- [Troubleshooting](troubleshooting.md)
