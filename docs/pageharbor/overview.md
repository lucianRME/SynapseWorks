# PageHarbor Overview

## Purpose

Explain what PageHarbor does, its current availability, and its privacy-first operating model.

## Who it is for

- Approved internal testers
- Android users evaluating local document-scanning workflows
- Security, privacy, and compliance reviewers

## Prerequisites

- Android 8 (API 26) or later
- Access to an approved PageHarbor internal-testing build
- Non-sensitive sample documents for testing

## Current availability

PageHarbor `v0.8.0-dev` is complete and tagged. It is being prepared for Google Play internal testing and is not publicly available on Google Play. This documentation is not a public download or installation guide.

## Product page

Website: [PageHarbor](https://synapseworks.org/pageharbor/)

## Capability summary

- Scan up to 10 pages in one scanner session with Google ML Kit Document Scanner
- Import page images from the gallery
- Create a normal PDF or export individual JPEG pages
- Share a PDF using the Android Sharesheet
- Run bundled, offline Latin-script OCR and select recognized text
- Copy recognized text only through the explicit **Copy Text** action
- Generate searchable PDFs locally
- Suggest safe, category-based filenames for searchable-PDF saves
- Choose export destinations through Android's Storage Access Framework (SAF)

PageHarbor has no account, ads, PageHarbor analytics or tracking, PageHarbor backend, or persistent document library.

## Common issues

- A scanner session is limited to 10 pages; start another session for additional pages.
- A Google Play internal-testing build is not a public Google Play release.
- Use non-sensitive documents during testing and do not rely on PageHarbor as a document archive.

## Related pages

- [Getting started](getting-started.md)
- [Scanning and export workflow](workflow.md)
- [Privacy and support](privacy-and-support.md)
- [Documentation index](../index.md)
- [PageHarbor Android source](https://github.com/lucianRME/pageharbor-android)
