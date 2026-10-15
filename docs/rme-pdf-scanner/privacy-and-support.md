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
- On-device processing of scan images, imported content, OCR text, document tools, and searchable-PDF content
- An app-private local library only when the user chooses **Save to RME**
- User-initiated portable backup and restore, with optional password protection

RME PDF Scanner declares neither the `INTERNET` nor `ACCESS_NETWORK_STATE` permission and does not request camera permission directly. Camera scanning is provided by Google ML Kit Document Scanner. It also declares no broad-storage, account, location, contacts, microphone, phone, or advertising permission.

An unsaved session is not recovered after process death. When the user explicitly saves a document to RME, the app stores page copies, thumbnails, metadata, folder assignments, edits, and any explicitly recognized text needed for local search in private app storage. Android automatic backup and device transfer are disabled for this data.

## Third parties and destinations

The user chooses save destinations through Android SAF and share targets through the Android Sharesheet. External storage providers, viewers, and receiving apps have their own policies. RME PDF Scanner does not receive external-provider account credentials.

Google ML Kit performs document scanning and OCR content processing on the device. Latin recognition is bundled. Optional Chinese, Japanese, Korean, and Devanagari models, as well as scanner resources, may be downloaded or updated by Google Play services. ML Kit may transmit encrypted technical diagnostics, such as device or app information, configuration, performance or error data, and installation identifiers. This is SDK behavior, not RME PDF Scanner-operated analytics or tracking; according to Google's ML Kit documentation, it does not include document images, text input, or recognition output.

## Retention and deletion

Saved library documents remain in app-private storage until the user deletes the document, clears app data, or uninstalls RME. Deleting a document permanently removes RME's page copies, thumbnail, metadata, and indexed OCR text; it never deletes the external files originally imported. Deleting a folder keeps its documents and moves them out of that folder. Version 1.7.1 makes deletion recovery more reliable and conservatively cleans private files that can be safely identified as leftovers from earlier interrupted deletions.

Exports, shared files, clipboard contents, and portable backups are controlled separately by Android and the destination or receiving app. A password-protected backup keeps its password under the user's control; do not lose it or include it in a support report.

## Support and security

For product help, use [SynapseWorks Support](https://synapseworks.org/support/). When reporting a defect, include the Android version, device model, RME PDF Scanner version, installation channel, the action being tested, and redacted error details. Do not send sensitive documents, OCR text, saved-file paths, backup passwords, account credentials, or unredacted logs.

For security reports, use the [SynapseWorks security page](https://synapseworks.org/security/).

## Source and license

Source: [RME PDF Scanner Android repository](https://github.com/lucianRME/rme-pdf-scanner). RME PDF Scanner is licensed under the Apache License 2.0.

## Common issues

- Android or an external provider may retain a saved, shared, or copied item under its own controls.
- The lack of `INTERNET` and `ACCESS_NETWORK_STATE` permissions in RME does not change the separate resource-delivery and diagnostic disclosures for Google ML Kit and Google Play services.
- RME PDF Scanner is publicly available on [Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor); see [Getting started](getting-started.md) for installation and separate developer-build guidance.

## Related pages

- [Overview](overview.md)
- [Getting started](getting-started.md)
- [Scanning and export workflow](workflow.md)
- [Trust and security overview](../common/trust-security.md)
