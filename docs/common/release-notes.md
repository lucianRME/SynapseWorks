# Release Notes

## Purpose
Provide a standard format for documenting functional changes, fixes, and operational notes.

## Who it is for
- Product and release managers
- Jira administrators tracking behavioural changes
- Browser extension users and reviewers tracking behavioural changes
- Security reviewers tracking data-handling-impacting changes

## Prerequisites
- Confirmed change scope and deployment date
- Validation evidence (test notes, dry-run output, extension test result, or production observation)

## 2026-10-14 - RME PDF Scanner 1.7.1

### Fixed
- Made saved-document deletion more reliable when database or private-file cleanup is interrupted.
- Improved automatic recovery of interrupted document deletion after an application restart.
- Added conservative cleanup for safely identifiable private document files left behind by earlier deletion failures, while preserving files whose ownership cannot be established safely.

### Security and data impact
- No change to RME's account, network-permission, backend, analytics, advertising, or cloud-storage boundaries.
- Cleanup remains limited to private files whose ownership RME can establish safely; external imported files are not deleted.

## 2026-10-11 - RME PDF Scanner 1.7.0

### Added
- Share-Safe copies with destructive blackout redaction, purpose/date watermarking, optional file-size targets, and final preview before save or share.
- Fit Upload Limit with common and custom targets, readability-aware processing, and preservation of documents that already fit.
- Two-sided ID/card copy with A4 or Letter layouts and zoom/pan review.
- Improved migration from standard PDFs and images exported by other scanner apps.

### Changed
- Improved OCR review, correction, re-recognition, batch processing, page-aware search, searchable-PDF workflows, document review, navigation, accessibility, large-text behavior, and the Graphite Teal interface.

### Fixed
- Improved import and tool continuation, first-run OCR result presentation, Share-Safe preparation, already-fits handling, redaction direct manipulation, and related reliability behavior.

### Security and data impact
- Share-Safe creates a separate copy and leaves the original unchanged.
- Document-content processing remains on-device; migration uses user-exported PDFs and images and does not access another app's private storage, database, account, or cloud.

## Steps
1. Create a new entry using the template below.
2. List only verified changes and clearly label behavioural impact.
3. Add any security/data/privacy impact with links to the relevant product page.
4. Publish the update in GitBook after review.

## Entry template
```markdown
## YYYY-MM-DD - Release name

### Added
- Item

### Changed
- Item

### Fixed
- Item

### Operational notes
- Item

### Security and data impact
- None
```

## Common issues
- Unverified claims in release notes can cause support rework.
- Missing behavioural impact notes increase rollout risk.

## Related pages
- [Documentation index](../index.md)
- [Support](support.md)
- [Submit Guard overview](../submit-guard/overview.md)
- [RME PDF Scanner overview](../rme-pdf-scanner/overview.md)
