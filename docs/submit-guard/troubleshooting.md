# Submit Guard Troubleshooting

## Purpose
Resolve common Submit Guard installation, enablement, and confirmation issues.

## Who it is for
- Submit Guard users
- Support teams
- Browser extension administrators

## Prerequisites
- Submit Guard installed in Chrome or a Chromium-based browser
- Access to the site you are testing
- A safe test form or non-sensitive workflow for validation

## Steps
1. Confirm Submit Guard is installed and enabled in the browser profile.
2. Confirm Submit Guard is enabled for the current site.
3. Start with standard mode and test a native form submission.
4. If the site uses a modern app button instead of a native form, try advanced mode.
5. Refresh the page after changing site settings or modes.
6. Test again with non-sensitive input.
7. If the issue remains, contact [SynapseWorks Support](https://synapseworks.org/support/) with the browser version, site type, mode, and expected behaviour.

## Common issues
### No confirmation appears
- Submit Guard may not be enabled for the current site.
- The page may use a submit-like click that requires advanced mode.
- The page may be a browser-restricted or extension-restricted URL.

### Confirmation appears too often
- Review whether advanced mode is enabled.
- Check whether the site uses multiple submit-like buttons in the same workflow.
- Disable Submit Guard for sites where confirmation is not useful.

### Settings do not carry across browsers
Settings are stored locally in `chrome.storage.local` for the current browser profile. They are not stored in a SynapseWorks backend.

### Support asks for reproduction details
Do not send sensitive form contents. Share:

- Browser name and version
- Site domain or app type
- Submit Guard mode
- Whether the issue happens in standard or advanced mode
- Screenshots with sensitive content redacted

## Related pages
- [Overview](overview.md)
- [Install](install.md)
- [How it works](how-it-works.md)
- [Privacy](privacy.md)
