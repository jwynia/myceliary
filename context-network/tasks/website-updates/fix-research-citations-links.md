# Task: Fix Research Citations Data File Links

## Priority: Medium

## Source
- Generated from website sync report 2025-08-13
- Original recommendation: Fix broken links in research_citations.yml

## Description
Update all internal `/context-network/` links in the research citations data file to use proper GitHub URLs.

## Acceptance Criteria
- [ ] Update all links in `docs/_data/research_citations.yml`
- [ ] Convert `/context-network/` paths to GitHub URLs
- [ ] Verify all links resolve correctly
- [ ] Maintain YAML syntax validity
- [ ] Test Jekyll build after changes

## Current Issues
- 10+ citation links point to `/context-network/` paths
- These don't resolve in Jekyll build
- Need consistent URL pattern

## Effort Estimate: Small (30 minutes)

## Risk Level: Low
- Simple URL replacements
- No logic changes
- Data file only

## Dependencies
- None - straightforward link updates

## Why Deferred
- While low risk, there are many links to update
- Needs systematic approach to ensure consistency
- Should verify all target files exist on GitHub