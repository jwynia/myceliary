# apply-recommendations

Intelligently triage and apply research, documentation, and framework recommendations

## Usage

Analyze recommendations from audits, reviews, or manual input and decide what to address immediately versus what requires deeper investigation or planning.

## Recommendations to Process
$ARGUMENTS

## Command Options

Parse $ARGUMENTS for options:
- `--quick-only` - Only apply simple, low-risk improvements
- `--defer-all` - Convert all recommendations to research tasks
- `--risk-threshold [low|medium|high]` - Maximum risk level for immediate action
- `--effort-limit [trivial|small|medium]` - Maximum effort to apply now
- `--dry-run` - Show what would be done without applying
- `--source [audit|review|research|manual]` - Source type for context

## Core Principle: Smart Research Triage

Not all recommendations require immediate action. Some can be quickly addressed, while others need deeper research, synthesis, or collaborative discussion.

## Processing Workflow

### Phase 1: Parse and Categorize

1. **Extract Recommendations**
   - Parse input for actionable items
   - Identify severity levels (Critical/High/Medium/Low)
   - Extract document paths and sections
   - Note provided rationale or evidence

2. **Assess Each Recommendation**
   
   For each item, determine:
   
   **Effort Required:**
   - Trivial: < 5 minutes, simple edits
   - Small: 5-30 minutes, single document
   - Medium: 30-60 minutes, 2-3 documents
   - Large: > 60 minutes, multiple documents or new research
   
   **Risk Level:**
   - Low: Typos, formatting, clarifications
   - Medium: Citation updates, minor restructuring
   - High: Framework changes, contradicting existing research
   
   **Dependencies:**
   - Independent: Can be done in isolation
   - Local: Requires understanding immediate context
   - Research: Needs additional investigation
   - Collaborative: Needs discussion or consensus

### Phase 2: Triage Decision Matrix

Apply this decision logic:

```
APPLY NOW if ALL of:
- Effort: Trivial or Small
- Risk: Low or (Medium with clear evidence)
- Dependencies: Independent or Local
- Clear improvement is obvious
- Won't contradict existing frameworks

DEFER TO TASK if ANY of:
- Effort: Large
- Risk: High
- Dependencies: Research or Collaborative
- Requires new research
- Needs synthesis of multiple sources
- Could change fundamental understanding
- Touches core frameworks
```

### Phase 3: Apply Immediate Improvements

For items marked "Apply Now":

1. **Citation Updates**:
   - Fix broken links
   - Update outdated references
   - Add missing page numbers
   - Correct formatting

2. **Documentation Clarity**:
   - Fix typos and grammar
   - Clarify ambiguous statements
   - Add helpful examples
   - Improve navigation

3. **Organization Improvements**:
   - Split oversized documents
   - Create missing indexes
   - Update navigation hubs
   - Fix broken cross-references

### Phase 4: Create Research Tasks

For items marked "Defer to Task":

1. **Create Task Entry** with:
   - Clear research question
   - Context from recommendation
   - Success criteria
   - Estimated effort
   - Required sources noted
   - Link to original recommendation

2. **Categorize by Type**:
   - Deep research → `/tasks/research/`
   - Framework development → `/tasks/frameworks/`
   - Synthesis needed → `/tasks/synthesis/`
   - Organization → `/tasks/reorganization/`

### Phase 5: Update Context Network

1. **Document Applied Changes**:
   - What was changed and why
   - Evidence supporting change
   - Any uncertainties noted

2. **Record Deferred Items**:
   - Create or update research backlog
   - Note priority and rationale
   - Link related investigations

## Recommendation Categories

### Critical Research Issues → ALWAYS APPLY NOW
- Factual errors with clear corrections
- Missing critical citations
- Broken reference links
- Contradictory statements (if resolution clear)
- Misleading summaries

### High Priority Documentation → USUALLY APPLY NOW
- Outdated information (if update clear)
- Navigation breakdowns
- Missing glossary terms
- Unclear framework steps
- Accessibility barriers

### Knowledge Organization → SELECTIVE APPLICATION
**Apply Now:**
- Document splitting (if over 300 lines)
- Simple cross-reference additions
- Index updates
- Navigation hub improvements
- Dead link removal

**Defer to Tasks:**
- Major restructuring
- New categorization schemes
- Complex relationship mapping
- Framework overhauls
- Comprehensive reorganization

### Research Quality → SELECTIVE APPLICATION
**Apply Now:**
- Add missing citations (if source known)
- Fix citation formatting
- Update publication dates
- Correct author names
- Add DOIs or stable URLs

**Defer to Tasks:**
- Find better sources
- Investigate contradictions
- Validate controversial claims
- Expand evidence base
- Add counter-perspectives

### Framework Improvements → USUALLY DEFER
- Logical restructuring
- New component additions
- Scope modifications
- Implementation guidance updates
- Validation methodology changes

## Output Format

```markdown
# Recommendation Application Report

## Summary
- Total recommendations: [X]
- Applied immediately: [Y]
- Deferred to research tasks: [Z]

## ✅ Applied Immediately

### 1. [Recommendation Title]
**Type**: [Citation/Documentation/Organization/Clarity]
**Documents Modified**: 
- `path/to/document.md` - [What changed]

**Changes Made**:
- [Specific change description]
- Evidence basis: [Source or rationale]
- Risk: [Low/Medium]

### 2. [Next Applied Item...]
[...]

## 📋 Deferred to Research Tasks

### High Priority Tasks Created

#### Task: [Clear Research Question]
**Original Recommendation**: [What was recommended]
**Why Deferred**: [Needs research/synthesis/discussion]
**Research Required**: [What investigation needed]
**Created at**: `/tasks/[type]/[filename].md`

### Medium Priority Tasks Created
[...]

### Low Priority Tasks Created
[...]

## Validation

### For Applied Changes:
- [ ] Citations remain valid
- [ ] No contradictions introduced
- [ ] Navigation paths work
- [ ] Document sizes appropriate
- [ ] Changes are well-reasoned

### For Deferred Tasks:
- [ ] Research questions are clear
- [ ] Success criteria defined
- [ ] Dependencies documented
- [ ] Tasks properly categorized

## Next Steps

1. **Immediate Actions**:
   - Review applied changes
   - Update affected indexes
   - Check cross-references

2. **Research Planning**:
   - Prioritize deferred research
   - Identify quick wins
   - Schedule deep investigations

3. **Follow-up Recommendations**:
   - [Patterns requiring attention]
   - [Systemic issues needing discussion]

## Statistics

- **Quick Improvements**: [Count of trivial fixes]
- **Research Avoided**: [Items needing investigation]
- **Knowledge Gaps Found**: [Count of research needs]
- **Organization Impact**: [Documents affected]
```

## Decision Examples

### Example: Apply Now
```
Recommendation: "Fix broken link to research paper in framework.md:45"
Decision: APPLY NOW
Rationale: Trivial effort, clear fix, improves accessibility
```

### Example: Defer to Task
```
Recommendation: "Add counter-arguments to anti-capitalist framework"
Decision: DEFER TO TASK
Rationale: Requires research into opposing viewpoints, synthesis needed
```

### Example: Conditional Application
```
Recommendation: "Update citation to latest edition"
Decision: APPLY NOW (if edition available), DEFER (if needs obtaining)
Rationale: Simple if we have access, research task if not
```

## Quality Guidelines

1. **Preserve research integrity** - Don't guess at facts
2. **Maintain citation quality** - Verify before updating
3. **Respect uncertainty** - Note when unsure
4. **Document reasoning** - Explain all decisions
5. **Group related changes** - Keep updates logical
6. **Incremental progress** - Many small improvements build knowledge

## Special Handling

### For Factual Errors
- Correct immediately if certain
- Create research task if uncertain
- Document source of correction
- Note any controversy

### For Missing Research
- Only add if source readily available
- Defer if requires investigation
- Create specific research question
- Estimate effort required

### For Framework Issues
- Only apply if logic clear
- Defer structural changes
- Document validation needs
- Consider downstream impacts

Remember: The goal is maintaining research quality while making steady progress. It's better to defer uncertain changes than to introduce errors or unsupported claims.