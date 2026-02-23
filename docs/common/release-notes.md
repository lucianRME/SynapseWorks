# Release Notes

## Purpose
Provide a standard format for documenting functional changes, fixes, and operational notes.

## Who it is for
- Product and release managers
- Jira administrators tracking behavioural changes
- Security reviewers tracking data-handling-impacting changes

## Prerequisites
- Confirmed change scope and deployment date
- Validation evidence (test notes, dry-run output, or production observation)

## Steps
1. Create a new entry using the template below.
2. List only verified changes and clearly label behavioural impact.
3. Add any security/data impact with links to the relevant security page.
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
