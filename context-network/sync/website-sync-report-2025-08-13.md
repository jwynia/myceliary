# Website Sync Report - 2025-08-13

## Executive Summary
- Pages analyzed: 27 markdown files
- Critical issues: 5 (broken internal links)
- High priority updates: 12
- New content available: 15+ items
- Enhancement opportunities: 8

## Critical Updates Required

### Broken Links (Internal References)
All links in docs/ reference `/context-network/` paths that don't exist on the Jekyll site:

1. **File**: `docs/_data/research_tasks.yml`
   - **Issue**: Links point to `/context-network/` which doesn't exist in the Jekyll build
   - **Fix**: Either copy context network files to docs/ or update to GitHub URLs
   - **Affected links**: 5 task references

2. **File**: `docs/_data/research_citations.yml`
   - **Issue**: Links to `/context-network/research_archives/` don't resolve
   - **Fix**: Update to proper GitHub URLs or relative paths
   - **Affected links**: 10+ citation references

### Outdated Task Statuses
1. **Research Tasks** (`_data/research_tasks.yml`)
   - **AI/ML Landscape**: Shows "In Progress" but marked **Completed** in context network
   - **Historical Case Studies**: Shows "In Progress" but marked **Completed** in context network
   - **Jekyll Setup Requirements**: Not listed but marked **Completed** in context network
   - Missing 15+ research tasks from context network

## High Priority Updates

### 1. Missing Technical Specifications
**7 Technical Specifications at Stage 5 (Design Complete)**
These are referenced in `/docs/cannae/index.md` but missing detailed specs:

1. **FreeSpeak Liberation Language** - Spec exists, page partially complete
2. **Consensus Engine** - No technical spec page
3. **Portable Identity Commons** - Basic page exists, needs spec details
4. **Careful AI Development** - Basic page exists, needs spec details
5. **Hyperlocal AI** - Basic page exists, needs spec details
6. **Craft Augmentation AI** - Not mentioned on website
7. **Community Resilience Mesh** - Not on website

**Action**: Create detailed specification pages using context network sources

### 2. Missing Organizational Documentation
**501(c)(3) Structure & Revenue Models**
- `/context-network/planning/myceliary_501c3_structure.md` - Complete guide not on website
- `/context-network/planning/myceliary_sustainable_revenue_models.md` - Revenue strategy not published
- `/context-network/planning/high_leverage_projects.md` - Strategic projects not documented

**Action**: Create new `/organization/` section with:
- `docs/organization/index.md` - Overview
- `docs/organization/501c3-structure.md` - Nonprofit structure
- `docs/organization/revenue-models.md` - Sustainability strategy
- `docs/organization/strategic-projects.md` - High-leverage initiatives

### 3. Missing Opportunities
**New Opportunities in Pipeline (Stage 3)**
- **Bureaucracy Navigation Assistant** - Added to opportunity tracker, not on website
- Multiple emerging opportunities listed in tracker not reflected on site

### 4. Outdated Statistics
- Homepage claims "8 Cannae opportunities" but tracker shows 9+ active
- Research tasks show 5 items but 20+ exist in context network
- Case studies incomplete (missing several documented in context network)

## Medium Priority Updates

### Enhanced Content Available

1. **Cannae Framework Documentation**
   - Context network has expanded vulnerability analysis
   - New patterns identified: AI development acceleration, mental model traps
   - Opposition counter-strategies documented
   - Skills/capacity building frameworks added

2. **Research Archives Enhancement**
   - Medium and deep research reports not displayed
   - Citation system more sophisticated than shown
   - Research synthesis and strategic recommendations available

3. **Implementation Progress**
   - Medical AI Data Dignity Cooperative spec complete (23k words)
   - Detailed implementation stages not shown
   - Federation work progress not documented

## Enhancement Opportunities

### 1. Better Navigation Structure
- Add implementation tracker dashboard
- Create research progress visualization
- Add opportunity pipeline view
- Include task status dashboard

### 2. Missing Visualizations
From context network pipeline tracker:
- Stage distribution chart
- Source method breakdown
- Effort application matrix
- Task relationship diagram

### 3. Cross-References
- Link between opportunities and their technical specs
- Connect research tasks to findings
- Reference implementation stages

## Recommended Actions

### Immediate (Do Now)
1. Fix broken internal links - convert to GitHub URLs
2. Update research task statuses in `_data/research_tasks.yml`
3. Correct opportunity count on homepage (8 → 9+)
4. Add Bureaucracy Navigation Assistant to Cannae section

### Short-term (This Week)
1. Create `/organization/` section with 501(c)(3) docs
2. Add missing technical specification pages
3. Update research archive to show all report types
4. Create implementation progress tracker

### Long-term (This Month)  
1. Enhance Cannae documentation with new patterns
2. Add visualization components for pipeline tracking
3. Improve cross-referencing between sections
4. Add research synthesis findings

## File Change Summary

### Files to Update
```yaml
Priority 1 (Critical):
- docs/_data/research_tasks.yml - Fix statuses, add missing tasks
- docs/_data/research_citations.yml - Fix broken links
- docs/index.md - Update statistics

Priority 2 (High):
- docs/cannae/index.md - Add new opportunities
- docs/research/index.md - Update task statuses
- docs/projects/index.md - Add implementation progress
```

### Files to Create
```yaml
Organizational:
- docs/organization/index.md
- docs/organization/501c3-structure.md  
- docs/organization/revenue-models.md
- docs/organization/strategic-projects.md

Technical Specs:
- docs/cannae/consensus-engine.md
- docs/cannae/craft-augmentation.md
- docs/cannae/community-resilience-mesh.md
- docs/cannae/bureaucracy-navigation.md

Enhanced Specs:
- Update existing Cannae pages with technical details
```

### Content Migration Suggestions
1. Research findings from context network → website
2. Technical specifications → dedicated pages
3. Implementation progress → project tracker
4. Planning documents → organization section

## Validation Checklist
- [ ] All internal links resolve correctly
- [ ] Statistics match context network counts
- [ ] Research task statuses accurate
- [ ] Technical specs have dedicated pages
- [ ] Organization section created
- [ ] Jekyll builds successfully
- [ ] No 404 errors on navigation

## Notes
- Website uses GitHub URLs for external links to context network
- Consider whether to copy files or maintain external links
- Jekyll constraints limit dynamic content generation
- GitHub Pages deployment must be considered for changes