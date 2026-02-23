# Platform Pipeline (SaaS)

## Purpose
Show the end-to-end Synapse platform pipeline from transcript ingestion to Jira sync.

## Who it is for
- Platform operations teams
- Product owners and analysts
- Delivery leads evaluating transcript-driven requirement generation

## Prerequisites
- Platform access to upload transcript files
- Source transcripts in `.vtt` or `.txt` format

## Steps
1. Upload or drag and drop transcript files.
2. Run transcript cleanup and optional small-talk filtering.
3. Extract structured requirements from processed transcript content.
4. Generate BDD and Gherkin scenarios.
5. Run validation and deduplication.
6. Perform human review with approval controls or bulk approve.
7. Persist session outputs (SQLite and JSON persistence).
8. Export to CSV where needed.
9. Sync to Jira Cloud with idempotency and optional linking.

## Pipeline controls
- Session-aware processing for continuity across review stages
- Human approval gates before downstream sync
- Idempotent Jira sync path to reduce duplicate writes

## Common issues
- Low transcript quality can reduce extraction quality.
- Skipping human review can increase downstream correction work.
- Sync outcomes depend on external Jira project readiness.

## Related pages
- [Overview](overview.md)
- [Security and data](security-data.md)
