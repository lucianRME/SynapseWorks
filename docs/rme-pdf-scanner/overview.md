# RME: PDF & Document Scanner

RME: PDF & Document Scanner is a privacy-first, local-first Android document scanner with a private document library, multilingual on-device OCR, searchable PDFs, safer-sharing tools, portable backup, and user-controlled export.

> PageHarbor is now RME: PDF & Document Scanner. The product and its privacy-first principles remain the same; only the public name has changed.

## Purpose

Explain what RME PDF Scanner does, its current availability, and its privacy-first operating model.

## Who it is for

- Android users installing RME PDF Scanner
- Android users evaluating local document-scanning workflows
- Security, privacy, and compliance reviewers

## Prerequisites

- Android 8 (API 26) or later
- RME PDF Scanner installed from Google Play, or a developer build from the open-source repository
- Non-sensitive sample documents for testing

## Current availability

RME: PDF & Document Scanner is publicly available on [Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor). The current stable version is **1.7.1**. Version 1.7.1 includes the major 1.7.0 feature set and improves deletion and cleanup reliability for saved documents.

## Product page

Website: [RME PDF Scanner](https://synapseworks.org/rme-pdf-scanner/)

## Capability summary

- Scan up to 20 pages in one interactive scanner session with Google ML Kit Document Scanner
- Import PDF, JPEG, PNG, and WebP files through Android's system picker, or receive supported files through Android sharing
- Save documents in an app-private local library with folders, subfolders, thumbnails, titles, sorting, and title or recognized-text search
- Run bundled Latin-script OCR or optional Chinese, Japanese, Korean, and Devanagari OCR delivered through Google Play services; review, correct, re-run, and batch-process recognized text on the device
- Create normal or searchable PDFs, export JPEG pages or recognized text, and save or share through Android system flows
- Merge documents, split or extract pages, and fit documents to common or custom upload-size targets
- Create Share-Safe copies with destructive blackout redaction, purpose/date watermarking, an optional file-size target, and final preview
- Place the front and back of an ID or card on one A4 or Letter page with zoom and pan review
- Import standard user-exported PDFs and images from other scanner apps without accessing their private storage, databases, accounts, or cloud services
- Create and restore portable library backups, with optional password protection
- Optionally require Android device authentication when opening RME

RME PDF Scanner requires no account and has no ads, RME-operated analytics or tracking, or proprietary document-processing backend. Saved documents and optional OCR text can remain in its app-private local library. Its [open-source code](https://github.com/lucianRME/rme-pdf-scanner) is available under the Apache License 2.0. Google ML Kit has separate resource-delivery and technical-diagnostic disclosures; see [Privacy and support](privacy-and-support.md).

## Common issues

- The interactive ML Kit scanner is limited to 20 pages per session. Import, migration, backup, and restore can preserve longer documents.
- A size target is a best effort: RME preserves readability and may not reach every arbitrary limit.
- Deleting a saved document is permanent; version 1.7.1 improves recovery when cleanup is interrupted but does not add a trash or restore layer.

## Related pages

- [Getting started](getting-started.md)
- [Scanning and export workflow](workflow.md)
- [Privacy and support](privacy-and-support.md)
- [Documentation index](../index.md)
- [RME PDF Scanner Android source](https://github.com/lucianRME/rme-pdf-scanner)
