# PageHarbor Scanning and Export Workflow

## Purpose

Describe how PageHarbor captures, processes, saves, and shares documents.

## Who it is for

- PageHarbor internal testers
- Android users reviewing local document handling
- Privacy and security reviewers

## Prerequisites

- An approved PageHarbor build on Android 8 (API 26) or later
- A non-sensitive sample document

## Steps

1. Start a scan and capture up to 10 pages with Google ML Kit Document Scanner, or import pages from the gallery.
2. Review the captured pages and choose a normal PDF, JPEG page export, OCR text, or searchable PDF.
3. Let PageHarbor prepare the chosen output locally on the device.
4. Choose a save destination through Android SAF, or use the Android Sharesheet to send a PDF to a receiving app.
5. Confirm the file in the destination or receiving app, which then handles it under its own policies.

## Output handling

| Output | Local processing | User-controlled exit |
| --- | --- | --- |
| Normal PDF | Prepared on the device | Saved through Android SAF |
| JPEG page | Prepared on the device | Saved through Android SAF |
| Recognized text | Bundled Latin-script OCR in the active session | Copied to the Android clipboard through **Copy Text** |
| Searchable PDF | Generated locally with an OCR text layer | Saved through Android SAF |
| Shared PDF | Prepared locally | Sent only after the user selects a target in Android Sharesheet |

## Storage and sharing boundaries

PageHarbor does not provide cloud storage or a persistent document library. SAF lets the user choose the final destination, which may be device storage or an installed external provider. PageHarbor does not receive that provider's account credentials or control its retention practices.

Temporary app-private files may be created for processing or sharing. They are not a persistent PageHarbor library. External viewers, storage providers, and share targets apply their own terms and privacy policies once a user selects them.

## Common issues

- The final filename and destination are controlled by the system picker or selected provider.
- A filename suggestion is category-based and editable; it is not an automatic document classification record.
- Do not use a shared file or an external destination as evidence that PageHarbor retains a copy.

## Related pages

- [Overview](overview.md)
- [Getting started](getting-started.md)
- [Privacy and support](privacy-and-support.md)
