# PageHarbor Getting Started

## Purpose

Run a safe first PageHarbor session with an approved internal-testing build.

## Who it is for

- Approved internal testers
- Support teams reproducing a scan or export flow

## Prerequisites

- Android 8 (API 26) or later
- An approved PageHarbor internal-testing build
- Non-sensitive sample documents

## Steps

1. Open PageHarbor and start a document scan.
2. Capture pages in the ML Kit scanner flow, or import page images from the gallery.
3. Keep the session to 10 pages or fewer.
4. Review the result and choose the required output:
   - Normal PDF
   - Individual JPEG pages
   - Recognized text
   - Searchable PDF
5. For PDF or JPEG export, choose a destination in Android's system file picker.
6. For a PDF share, choose **Share** and select a receiving app in the Android Sharesheet.
7. For OCR text, select the text and use **Copy Text** only when you intend to place it on the Android clipboard.

## OCR and searchable PDFs

PageHarbor's bundled Latin-script OCR runs on the device. Recognized text is an active-session result unless you explicitly copy it. Searchable PDFs are generated locally from the scan and recognized text before you choose a destination through SAF.

For searchable-PDF saves, PageHarbor can suggest a safe filename from a broad document category. You can edit the suggested name; the SAF provider determines the final name and destination.

## Common issues

- No public Google Play installation link is available yet; do not describe internal testing as public availability.
- A saved or shared file is handled by the destination provider or receiving app after you choose it.
- Clipboard handling after **Copy Text** is controlled by Android and other apps on the device.

## Related pages

- [Overview](overview.md)
- [Scanning and export workflow](workflow.md)
- [Privacy and support](privacy-and-support.md)
