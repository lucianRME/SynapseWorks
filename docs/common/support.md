# Support

## Purpose
Define a consistent path for triage, escalation, and resolution across SynapseWorks documentation topics.

## Who it is for
- Jira administrators managing app rollout
- Browser extension users and reviewers
- Operational owners handling incidents and user queries

## Prerequisites
- Access to the relevant product environment
- Access to app or extension output relevant to the issue

## Steps
1. Capture scope: product (`Synapse`, `Decision Register`, `Submit Guard`, or `PageHarbor`) and expected outcome.
2. Capture evidence relevant to the product.
3. Confirm behaviour against the relevant documentation page.
4. Raise a support request through [SynapseWorks Support](https://synapseworks.org/support/) or, for Jira apps, the Marketplace support path, including captured evidence.
5. Record workaround and resolution in your internal runbook.

## Evidence to include
### Jira Apps
- Jira site URL and project key
- Issue keys, timestamps, selected filters, and any error text
- App mode or action used
- Screenshots with sensitive content redacted

### Submit Guard
- Browser name and version
- Site domain or app type
- Whether standard mode or advanced mode is enabled
- Whether Submit Guard is enabled for the current site
- Screenshots with sensitive form contents redacted

### PageHarbor
- Android version and device model
- PageHarbor version and build type
- Whether the issue occurred during scanning, saving, sharing, OCR, or searchable-PDF generation
- Redacted error text and safe reproduction steps

Do not send passwords, tokens, session cookies, MFA codes, or sensitive form contents.

## Common issues
- Missing issue keys or timestamps can delay diagnosis.
- Screenshots alone are often insufficient without product, filter, browser, or mode details.
- Mixed product context can lead to incorrect routing.

## Related pages
- [Documentation index](../index.md)
- [FAQ](faq.md)
- [Release notes](release-notes.md)
- [PageHarbor privacy and support](../pageharbor/privacy-and-support.md)
