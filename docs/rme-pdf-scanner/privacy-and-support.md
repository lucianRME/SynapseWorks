# RME PDF Scanner Privacy and Support

## Purpose

Summarize RME PDF Scanner data handling and provide the correct support and security paths.

## Who it is for

- RME PDF Scanner users and developers
- Security, privacy, and compliance reviewers
- Support teams

## Prerequisites

- Understanding that RME PDF Scanner is an Android app, not a cloud document service
- Access to the relevant device or test build when reporting an issue

## Privacy summary

The [RME PDF Scanner Privacy Policy](https://synapseworks.org/rme-pdf-scanner/privacy/) is the authoritative public policy. If this documentation and the policy differ, follow the policy and report the discrepancy.

- No RME PDF Scanner account or login
- No ads
- No RME PDF Scanner analytics or tracking
- No RME PDF Scanner backend or proprietary cloud storage
- No persistent RME PDF Scanner document library
- On-device processing of scan images, OCR text, and searchable-PDF content

RME PDF Scanner has no direct `INTERNET` permission and does not request camera permission directly. Camera scanning is provided by Google ML Kit Document Scanner. RME PDF Scanner may create temporary app-private files while processing or sharing a file.

## Third parties and destinations

The user chooses save destinations through Android SAF and share targets through the Android Sharesheet. External storage providers, viewers, and receiving apps have their own policies. RME PDF Scanner does not receive external-provider account credentials.

Google ML Kit performs document scanning and bundled Latin-script OCR on the device. ML Kit may transmit encrypted technical diagnostics, such as device or app information, configuration, performance or error data, and installation identifiers. This is SDK behavior, not RME PDF Scanner-operated analytics or tracking; it does not include document content.

## Support and security

For product help, use [SynapseWorks Support](https://synapseworks.org/support/). When reporting a defect, include the Android version, device model, RME PDF Scanner version, the action being tested, and redacted error details. Do not send sensitive documents, OCR text, saved-file paths, account credentials, or unredacted logs.

For security reports, use the [SynapseWorks security page](https://synapseworks.org/security/).

## Source and license

Source: [RME PDF Scanner Android repository](https://github.com/lucianRME/rme-pdf-scanner). RME PDF Scanner is licensed under the Apache License 2.0.

## Common issues

- Android or an external provider may retain a saved, shared, or copied item under its own controls.
- The lack of a direct `INTERNET` permission does not change the separate diagnostic disclosures for ML Kit.
- RME PDF Scanner is publicly available on [Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor); see [Getting started](getting-started.md) for installation and separate developer-build guidance.

## Related pages

- [Overview](overview.md)
- [Getting started](getting-started.md)
- [Scanning and export workflow](workflow.md)
- [Trust and security overview](../common/trust-security.md)
