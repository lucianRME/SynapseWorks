---
description: >-
  Install RME: Private PDF Scanner on Android and complete a first scan,
  on-device OCR, export, or portable backup.
---

# RME: Private PDF Scanner — Getting Started

## Purpose

Install RME PDF Scanner and complete a first local scan, OCR, or export session.

## Who it is for

- Android users installing RME PDF Scanner
- Support teams reproducing a scan or export flow

## Prerequisites

- Android 8 (API 26) or later
- RME PDF Scanner installed as described below
- Non-sensitive sample documents

## Install from Google Play

Install [RME: Private PDF Scanner from Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor), then open the app. The current stable version is **1.7.1**.

The Android application ID remains `org.synapseworks.pageharbor`; it identifies the existing app listing despite the new public name.

## GitHub and local development

For source code, contributions, or a manual installation, use [lucianRME/rme-pdf-scanner](https://github.com/lucianRME/rme-pdf-scanner) and follow its README and [build/signing guidance](https://github.com/lucianRME/rme-pdf-scanner/blob/main/docs/RELEASE_SIGNING.md). The latest stable APK is also available from [GitHub Releases](https://github.com/lucianRME/rme-pdf-scanner/releases/latest).

Google Play and GitHub APKs use different signing certificates, so Android cannot install one channel over the other as an update. Before changing channels, create a portable RME backup and confirm that you can access it; Android may require uninstalling the existing app, which removes its app-private library.

## Steps

1. Open RME PDF Scanner and choose **Scan** or **Import**.
2. Capture up to 20 pages in the ML Kit scanner flow, or select supported PDF, JPEG, PNG, or WebP files through Android's system picker.
3. Review the pages. Add, reorder, rotate, remove, or enhance them as needed.
4. Choose **Save to RME** to keep the document in the private on-device library, or continue directly to OCR, PDF, JPEG, text, or sharing actions.
5. For PDF or JPEG export, choose a destination in Android's system file picker. For sharing, select a receiving app in the Android Sharesheet.
6. For OCR text, review the result before using **Copy Text**. Copy only when you intend to place the selected text on the Android clipboard.
7. Use the library to rename, sort, search, move into folders, reopen, edit, or delete saved documents.

## OCR and searchable PDFs

RME PDF Scanner's bundled Latin-script OCR runs on the device. Optional Chinese, Japanese, Korean, and Devanagari models are delivered through Google Play services, then recognition runs on-device after the selected model is available. You can review and correct text, re-run OCR for one page or a whole document, batch-process documents, search recognized text across the library, and jump to a matching page.

Recognized text remains active-session data unless you explicitly save the document to RME or copy the text. When saved after recognition, OCR text is stored locally to support library search. Searchable PDFs are generated locally before you choose a destination through SAF.

## Back up or move a library

Use RME's backup action to create a portable library backup, optionally protected with a password, and choose its destination through Android's system file picker. A restore reconstructs supported folders, documents, editable pages, page order and edits, saved OCR state, and retained source assets. Keep the backup and any password under your control.

## Common issues

- For installation, use the Google Play or latest GitHub Release link above and check that your device meets the Android requirement. Include the installation channel and build type when requesting support.
- A saved or shared file is handled by the destination provider or receiving app after you choose it.
- Clipboard handling after **Copy Text** is controlled by Android and other apps on the device.
- Deleting a saved document permanently removes RME's private copy. Version 1.7.1 improves recovery and cleanup if deletion is interrupted.

## Related pages

- [Overview](overview.md)
- [Scanning and export workflow](workflow.md)
- [Privacy and support](privacy-and-support.md)
