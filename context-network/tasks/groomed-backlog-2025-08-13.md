# Groomed Task Backlog - 2025-08-13

## 🚀 Ready for Implementation

### 1. Enhance Research Archives Display
**One-liner**: Add 12 medium research reports and deep research to the website archives page  
**Effort**: 1-2 hours  
**Files to modify**: 
- `/docs/research/archives.md`
- `/docs/_data/research_citations.yml` (potentially)

<details>
<summary>Full Implementation Details</summary>

**Context**: The research archives page currently only shows 4 light reports, but we have 12 medium reports and deep research that aren't visible to users. This represents significant research value that's hidden from the community.

**Acceptance Criteria**:
- [ ] Display all 12 medium research reports with summaries
- [ ] Add deep research reports section
- [ ] Show research synthesis findings
- [ ] Display strategic recommendations
- [ ] Improve citation system visibility
- [ ] Add categorization by research type (light/medium/deep)
- [ ] Include research methodology section

**Implementation Guide**:
1. Scan `/context-network/research_archives/medium_reports/` for all 12 reports
2. Extract title, date, key findings from each medium report
3. Check `/context-network/research_archives/deep_reports/` for any deep research
4. Read `/context-network/research_archives/research_index.md` for synthesis
5. Update `/docs/research/archives.md` with new sections:
   - Medium Research Reports (with expandable summaries)
   - Deep Research Analysis
   - Research Synthesis & Strategic Recommendations
6. Consider adding filtering UI (by date, type, topic)
7. Test page loads correctly with all new content

**Watch Out For**: 
- Large page size with all reports - consider pagination or lazy loading
- Maintaining consistent formatting across report types
- Ensuring all links to context network use GitHub URLs
- Jekyll liquid template syntax for dynamic content

**Source Materials Available**:
- 12 medium reports in `/context-network/research_archives/medium_reports/`
- Research index at `/context-network/research_archives/research_index.md`
- Deep reports directory exists
- Strategic recommendations in analysis findings

</details>

---

### 2. Create Consensus Engine Technical Specification
**One-liner**: Document the participatory budgeting consensus engine design  
**Effort**: 1-1.5 hours  
**Files to create**: 
- `/docs/cannae/consensus-engine.md`

<details>
<summary>Full Implementation Details</summary>

**Context**: The Consensus Engine is at Stage 5 (Design Complete) but lacks a public technical specification page. This is blocking community understanding and potential implementation.

**Acceptance Criteria**:
- [ ] Create comprehensive technical specification page
- [ ] Include architecture overview
- [ ] Document consensus mechanisms
- [ ] Provide implementation examples
- [ ] Add participatory budgeting use cases
- [ ] Link from main Cannae index
- [ ] Follow existing Cannae page format

**Implementation Guide**:
1. Review opportunity tracker entry for Consensus Engine
2. Search for any existing specs in context network
3. Create page following pattern of `bureaucracy-navigation.md`
4. Include sections:
   - Problem space (decision-making challenges)
   - Solution architecture
   - Consensus algorithms
   - Use cases (participatory budgeting, community decisions)
   - Implementation roadmap
   - Technical requirements
5. Add appropriate Jekyll front matter
6. Update Cannae index if needed

**Watch Out For**: 
- Maintaining consistent tone with other Cannae pages
- Technical accuracy while keeping accessible
- Proper parent-child navigation setup

</details>

---

### 3. Create Craft Augmentation AI Specification
**One-liner**: Document AI tools that enhance rather than replace human craft  
**Effort**: 1-1.5 hours  
**Files to create**: 
- `/docs/cannae/craft-augmentation.md`

<details>
<summary>Full Implementation Details</summary>

**Context**: Craft Augmentation AI is at Stage 5 (Design Complete) and represents a key anti-automation approach, but lacks documentation on the website.

**Acceptance Criteria**:
- [ ] Create technical specification page
- [ ] Explain augmentation vs automation philosophy
- [ ] Provide craft domain examples
- [ ] Document technical approach
- [ ] Include implementation patterns
- [ ] Add sustainability focus

**Implementation Guide**:
1. Research existing mentions of craft augmentation in context network
2. Create page structure similar to other Cannae opportunities
3. Focus on human-centered design principles
4. Include examples: woodworking, textiles, food production, arts
5. Document how AI enhances human skill rather than replacing it
6. Add technical architecture for augmentation systems

**Watch Out For**: 
- Clearly differentiating from automation
- Emphasizing human agency and skill development
- Connecting to broader anti-capitalist framework

</details>

## ⏳ Ready Soon (Minor Blockers)

### Community Resilience Mesh Specification
**Blocker**: Options development still in progress (🔄)  
**Estimated unblock**: When options analysis completes  
**Prep work possible**: Can research mesh network technologies and resilience patterns

### Update Navigation Menu
**Blocker**: Need to verify Jekyll navigation configuration  
**Estimated unblock**: Quick investigation needed  
**Prep work possible**: Document which pages need nav links

## 🔍 Needs Decisions

### Technical Specifications Format
**Decision needed**: Should we create individual spec pages or one comprehensive specs document?  
**Options**: 
- Individual pages (better SEO, easier navigation)
- Single document (easier maintenance, better overview)
**Recommendation**: Individual pages for better discoverability

### Research Archive Structure
**Decision needed**: How to handle 12+ medium reports without overwhelming the page?  
**Options**:
- Expandable sections with summaries
- Separate pages per report
- Pagination system
**Recommendation**: Expandable sections for best UX

## 🗑️ Completed/Archived Tasks

### Fix Research Citations Links - **Status**: Completed in last session
### Create Organization Section - **Status**: Completed with 4 pages
### Add Bureaucracy Navigation - **Status**: Completed and published

## Summary Statistics
- Total tasks reviewed: 5 website update tasks
- Ready for work: 3
- Blocked: 1 (Community Resilience Mesh)
- Completed since last groom: 3
- Archived: 0

## Top 3 Recommendations

1. **Enhance Research Archives** - Quick win (1-2 hours) that surfaces valuable hidden content
2. **Create Consensus Engine Spec** - Unblocks community understanding of key tool
3. **Create Craft Augmentation Spec** - Demonstrates anti-automation philosophy clearly

## Implementation Order Suggestion

Given current state:
1. Start with Research Archives (lowest effort, highest immediate value)
2. Then tackle Consensus Engine (enables participatory budgeting discussions)
3. Follow with Craft Augmentation (philosophical importance)
4. Leave visualizations for dedicated frontend session

All three top tasks can be completed in a 4-5 hour focused session.