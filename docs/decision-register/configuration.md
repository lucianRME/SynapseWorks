# Decision Register Configuration

## Purpose
Define the run settings and preference controls used to tune register output.

## Who it is for
- Jira administrators
- Governance owners managing report standards

## Prerequisites
- Access to Decision Register page
- Project access in Jira

## Steps
1. Select projects using search and filter.
2. Set the time range for the reporting window.
3. Set max issues scanned for performance and coverage balance.
4. Filter by issue types where needed.
5. Toggle only-my-changes for personal activity views.
6. Configure estimate field handling:
   - Use auto-detect by default
   - Set optional `customfield` override if your estimate field differs
7. Save and rerun; preferences persist per user in Forge storage.
8. Use reset-to-defaults when standardising configuration.

## Configuration reference
- Project selection: searchable multi-project scope
- Time range: controls event window
- Max issues scanned: limits scan size
- Issue type filter: narrows scope by issue class
- Only-my-changes: returns changes performed by current user
- Estimate field mode: auto-detect or explicit override
- Preference persistence: Forge storage per user

## Common issues
- Overly broad scans can produce partial warnings and slower runs.
- Wrong estimate field mapping can hide expected estimate events.
- Users may assume shared settings; preferences are per user.

## Related pages
- [Quickstart](quickstart.md)
- [Detections](detections.md)
- [Security and data](security-data.md)
