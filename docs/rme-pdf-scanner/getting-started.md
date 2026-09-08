# RME PDF Scanner Getting Started

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

Install [RME: PDF & Document Scanner from Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor), then open the app. The current version is **1.2.0**.

The Android application ID remains `org.synapseworks.pageharbor`; it identifies the existing app listing despite the new public name.

## GitHub and local development

For source code, contributions, or a manual development installation, use [lucianRME/rme-pdf-scanner](https://github.com/lucianRME/rme-pdf-scanner) and follow its README and [build/signing guidance](https://github.com/lucianRME/rme-pdf-scanner/blob/main/docs/RELEASE_SIGNING.md). Developer builds are separate from the normal Google Play installation path. Use non-sensitive sample documents when testing a build.

## Steps

1. Open RME PDF Scanner and start a document scan.
2. Capture pages in the ML Kit scanner flow, or import page images from the gallery.
3. Keep the session to 20 pages or fewer.
4. Review the result and choose the required output:
   - Normal PDF
   - Individual JPEG pages
   - Recognized text
   - Searchable PDF
5. For PDF or JPEG export, choose a destination in Android's system file picker.
6. For a PDF share, choose **Share** and select a receiving app in the Android Sharesheet.
7. For OCR text, select the text and use **Copy Text** only when you intend to place it on the Android clipboard.

## OCR and searchable PDFs

RME PDF Scanner's bundled Latin-script OCR runs on the device. Recognized text is an active-session result unless you explicitly copy it. Searchable PDFs are generated locally from the scan and recognized text before you choose a destination through SAF.

For searchable-PDF saves, RME PDF Scanner can suggest a safe filename from a broad document category. You can edit the suggested name; the SAF provider determines the final name and destination.

## Common issues

- For installation, use the Google Play link above and check that your device meets the Android requirement. For a local development build, include the build type when requesting support.
- A saved or shared file is handled by the destination provider or receiving app after you choose it.
- Clipboard handling after **Copy Text** is controlled by Android and other apps on the device.

## Related pages

- [Overview](overview.md)
- [Scanning and export workflow](workflow.md)
- [Privacy and support](privacy-and-support.md)
