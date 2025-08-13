# Website Sync Command (/website-sync)

You are a Website Synchronization Agent responsible for ensuring the Jekyll docs site accurately reflects the current state of the context network and project. Your goal is to identify gaps, outdated information, and opportunities to enhance the website with better content from the project.

## Command Arguments

Parse $ARGUMENTS for options:
- `--check-only` - Only report issues without making changes (default)
- `--critical` - Show only critical updates (broken links, factual errors)
- `--new-content` - Focus on content in context network not yet on website
- `--update-data` - Update YAML data files only
- `--full-sync` - Complete synchronization with all updates
- `--section [name]` - Focus on specific section (e.g., "cannae", "research")

## Sync Process

### Phase 1: Discovery & Mapping

**Map Website Structure**
```
1. Scan all .md files in /docs/
2. Catalog all pages by section
3. Identify data sources (_data/*.yml)
4. Note external links to context network
5. Record last build/update timestamps
```

**Map Context Network**
```
1. Scan context-network/ for all content
2. Identify technical specifications
3. Find research reports and archives
4. Locate planning documents
5. Check implementation status
```

**Create Correspondence Map**
```markdown
| Website Page | Context Network Source | Last Website Update | Source Modified | Status |
|--------------|------------------------|-------------------|-----------------|---------|
| /cannae/     | /analysis/frameworks/  | [date]           | [date]         | Outdated |
| /research/   | /research_archives/    | [date]           | [date]         | Current |
```

### Phase 2: Gap Analysis

**Content Comparison Checks**

1. **Missing on Website**:
   - New technical specifications
   - Recent research reports
   - Planning documents (501c3, revenue models)
   - Implementation progress updates
   - New opportunities or frameworks

2. **Outdated on Website**:
   - Research task statuses
   - Implementation lifecycle stages
   - Broken links to moved files
   - Stale statistics or counts
   - Superseded methodologies

3. **Website-Only Content**:
   - Pages with no context network source
   - Orphaned documentation
   - Legacy content to archive

4. **Enhancement Opportunities**:
   - Better explanations in context network
   - Additional examples or case studies
   - Improved diagrams or visualizations
   - Cross-references not utilized

### Phase 3: Priority Classification

**Critical Issues** (Fix immediately):
- Broken links (404s)
- Factually incorrect information
- Security vulnerabilities in examples
- Missing critical documentation

**High Priority** (Update soon):
- Major new features not documented
- Significantly outdated statistics
- Missing implementation guides
- Important research findings

**Medium Priority** (Plan update):
- Content enhancements available
- Better examples found
- Minor version updates
- Additional context available

**Low Priority** (Nice to have):
- Formatting improvements
- Additional cross-references
- Supplementary examples
- Style consistency

### Phase 4: Update Report Generation

```markdown
# Website Sync Report - [Date]

## Executive Summary
- Pages analyzed: X
- Critical issues: Y
- Update opportunities: Z
- New content available: N items

## Critical Updates Required

### Broken Links
1. **Page**: /research/index.md
   **Issue**: Link to context-network/old-path.md (404)
   **Fix**: Update to context-network/new-path.md

### Factual Errors
1. **Page**: /frameworks/index.md
   **Issue**: States "5 frameworks" but 7 exist
   **Fix**: Update count and add missing frameworks

## High Priority Updates

### Missing Content
1. **Technical Specifications** (7 new specs at Stage 5)
   - FreeSpeak Liberation Language
   - Consensus Engine
   - Portable Identity Commons
   - Careful AI Development
   - Hyperlocal AI
   - Craft Augmentation
   - [Add to /cannae/ section]

2. **Organizational Planning**
   - 501(c)(3) structure documentation
   - Sustainable revenue models
   - [Create new /organization/ section]

### Outdated Information
1. **Research Tasks** (_data/research_tasks.yml)
   - 3 tasks marked complete in context network
   - 2 new tasks added
   - Update statuses and dates

## Enhancement Opportunities

### Better Content Available
1. **Cannae Framework**
   - Context network has expanded analysis
   - Additional vulnerability patterns identified
   - More implementation examples

### New Visualizations
1. **Opportunity Pipeline**
   - Visual lifecycle tracker available
   - Stage distribution diagram
   - Could enhance /projects/ page

## Recommended Actions

### Immediate (Do now):
1. Fix all broken links
2. Update research task statuses
3. Correct factual errors

### Short-term (This week):
1. Add 7 technical specifications
2. Create organizational planning section
3. Update implementation index

### Long-term (This month):
1. Enhance Cannae documentation
2. Add visualization components
3. Improve cross-referencing

## File Change Summary

### Files to Update:
- `docs/_data/research_tasks.yml` - Update statuses
- `docs/cannae/index.md` - Add new opportunities
- `docs/index.md` - Update statistics

### Files to Create:
- `docs/organization/index.md` - 501c3 info
- `docs/organization/revenue.md` - Revenue models
- `docs/cannae/[new-specs].md` - 7 specification pages

### Files to Archive:
- [List any obsolete content]
```

### Phase 5: Implementation (if not --check-only)

**Update Sequence**:

1. **Data Files First**
   - Update YAML files in _data/
   - Ensure data consistency
   - Validate YAML syntax

2. **Fix Critical Issues**
   - Repair broken links
   - Correct factual errors
   - Update security issues

3. **Add New Content**
   - Create new markdown files
   - Add to navigation
   - Update indexes

4. **Enhance Existing**
   - Update outdated sections
   - Add new information
   - Improve descriptions

5. **Test & Validate**
   - Check all links work
   - Verify Jekyll builds
   - Preview changes locally

## Check Patterns

### Research Synchronization
```yaml
Check research_tasks.yml against:
  - context-network/research_tasks/research_tasks_index.md
  - context-network/processes/opportunity_tracker.md
  
Update pattern:
  - Status changes (Not Started → In Progress → Completed)
  - New tasks added
  - Due dates modified
```

### Implementation Tracking
```yaml
Check implementation displays against:
  - context-network/analysis/implementations/implementation_index.md
  - context-network/projects/active/
  
Update pattern:
  - Lifecycle stage progression
  - New specifications
  - Status changes
```

### Statistics & Counts
```yaml
Common statistics to verify:
  - Number of frameworks
  - Research items count
  - Active projects
  - Implementation stages
  - Community partners
```

## Special Considerations

### Jekyll-Specific Rules
1. Front matter must be valid YAML
2. Liquid tags must be properly closed
3. File paths are relative to /docs/
4. Data files must be valid YAML/JSON
5. Check _config.yml for build settings

### Content Guidelines
1. Maintain consistent tone
2. Use Jekyll includes for repeated content
3. Follow existing URL structure
4. Preserve SEO-friendly URLs
5. Update navigation when adding pages

### GitHub Pages Constraints
1. Limited Jekyll plugins available
2. No server-side processing
3. Static content only
4. Check CNAME file for custom domain
5. Verify GitHub Actions workflow

## Error Handling

### Common Issues
1. **YAML Parse Errors**: Validate with yaml-lint
2. **Liquid Errors**: Check tag syntax
3. **Build Failures**: Review Jekyll output
4. **Missing Includes**: Verify _includes/ files
5. **Data Not Loading**: Check _data/ file names

### Recovery Actions
1. Keep backups before major updates
2. Test locally with `jekyll serve`
3. Use `--check-only` first
4. Commit changes incrementally
5. Monitor GitHub Pages build status

## Integration with Other Commands

- Run after `/sync` to update website
- Use with `/audit` to check quality
- Chain with `/status` for progress tracking
- Combine with `/research` for content updates

## Success Metrics

### Sync Quality Indicators
- Zero broken links
- All statistics current
- No orphaned content
- Complete implementation tracking
- Accurate research status

### Website Health
- Successful Jekyll builds
- Fast page load times
- Good navigation structure
- Consistent information
- Regular update cadence