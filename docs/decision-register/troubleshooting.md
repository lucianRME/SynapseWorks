# Decision Register Troubleshooting

## Purpose
Resolve common run, filter, detection, and export issues in Decision Register.

## Who it is for
- Jira administrators
- Governance and reporting users
- Support teams

## Prerequisites
- Access to Decision Register run configuration and output
- Access to target Jira project context

## Steps
1. Identify whether the issue is run scope, detection output, or export.
2. Capture filters used, run metadata, and warning text.
3. Compare behaviour to expected detection and configuration rules.
4. Adjust run scope and rerun.
5. Escalate with captured evidence if unresolved.

## Common issues
- No entries returned:
  - Expand project scope or time range.
- Partial result warning:
  - Lower max issues or run narrower filter batches.
- Estimate changes not detected as expected:
  - Confirm estimate field auto-detect outcome or set explicit override.
- Export blocked:
  - Use copy-to-clipboard fallback.
- First run confusion:
  - Review the initialisation message and rerun with confirmed filters.

## Related pages
- [Quickstart](quickstart.md)
- [Detections](detections.md)
- [Support](../common/support.md)
