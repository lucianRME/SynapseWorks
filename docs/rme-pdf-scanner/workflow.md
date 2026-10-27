---
description: >-
  Scan, import, organize, process, and export documents locally with
  RME: Private PDF Scanner, including searchable PDFs and Share-Safe copies.
---

# RME: Private PDF Scanner — Scanning and Export Workflow

## Purpose

Describe how RME PDF Scanner captures, imports, organizes, processes, saves, and shares documents in version 1.7.1.

## Who it is for

- RME PDF Scanner users
- Android users reviewing local document handling
- Privacy and security reviewers

## Prerequisites

- RME PDF Scanner installed on Android 8 (API 26) or later
- A non-sensitive sample document

## Steps

1. Start a scan and capture up to 20 pages with Google ML Kit Document Scanner, or import supported PDFs and images through Android's system picker or sharing flow.
2. Review the pages and add, reorder, rotate, remove, or enhance them as needed.
3. Choose **Save to RME** to keep a private local-library copy, or continue without saving to the library.
4. Run OCR when needed, review or correct its output, and choose a normal PDF, searchable PDF, JPEG page export, recognized text, or a document tool.
5. Let RME PDF Scanner prepare the chosen result locally on the device.
6. Choose a destination through Android SAF, or use the Android Sharesheet to send the result to a receiving app.
7. Confirm the file in the destination or receiving app, which then handles it under its own policies.

## Output handling

| Output | Local processing | User-controlled exit |
| --- | --- | --- |
| Normal PDF | Prepared on the device | Saved through Android SAF |
| JPEG page | Prepared on the device | Saved through Android SAF |
| Recognized text | On-device OCR in the active session; optionally retained in a saved library document | Copied to the Android clipboard through **Copy Text** |
| Searchable PDF | Generated locally with an OCR text layer | Saved through Android SAF |
| Share-Safe copy | Redaction, watermarking, optional size targeting, and final preview performed locally | Saved through Android SAF or sent to a user-selected share target |
| Fit Upload Limit copy | Readability-aware processing with preservation of documents that already fit | Saved through Android SAF |
| Two-sided card copy | Front and back placed on one A4 or Letter page after zoom/pan review | Saved through Android SAF |
| Shared document | Prepared locally | Sent only after the user selects a target in Android Sharesheet |

## Library and document tools

The app-private library can retain document pages, thumbnails, titles, timestamps, page order and edits, folder assignments, and optional saved OCR text. You can reopen and edit a saved document, use folders and subfolders, sort the library, search titles or recognized text, and jump to matching pages.

Version 1.7.0 adds Share-Safe copies, Fit Upload Limit, two-sided card copy, and improved migration from standard PDFs and images exported by other scanner apps. Share-Safe creates a separate output, applies destructive blackout redaction and optional purpose/date watermarking, and leaves the original unchanged. Fit Upload Limit is best effort because readability takes priority over reaching every arbitrary size.

RME can also merge documents and split or extract pages. The interactive scanner retains its 20-page limit, while migration, import, backup, and restore can preserve longer documents without silently truncating them.

## Storage and sharing boundaries

RME PDF Scanner does not provide cloud storage or a proprietary document backend. Its persistent library is local and app-private. SAF lets the user choose an export or backup destination, which may be device storage or an installed external provider. RME PDF Scanner does not receive that provider's account credentials or control its retention practices.

Temporary app-private files may be created for importing, processing, or sharing. External viewers, storage providers, and share targets apply their own terms and privacy policies once a user selects them. RME's private library and database are excluded from Android automatic backup and device transfer; portable backup and restore occur only when the user explicitly starts them.

## Common issues

- The final filename and destination are controlled by the system picker or selected provider.
- Changing from the Google Play build to a GitHub APK, or back, may require uninstalling the current app because the channels use different signing certificates. Create and verify a portable backup first.
- Deleting a saved document permanently removes RME's private copies and database records, not the external source originally imported. Version 1.7.1 improves recovery after interrupted deletion and safely cleans identifiable leftovers from earlier failures.

## Related pages

- [Overview](overview.md)
- [Getting started](getting-started.md)
- [Privacy and support](privacy-and-support.md)
