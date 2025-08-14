# sync

Synchronize research plans with actual progress and discoveries

## Usage

Detect and correct drift between planned research activities and actual research progress, ensuring the context network reflects current reality.

## Sync Objectives

When executing a /sync command:
1. **Detect Research Drift**: Identify discrepancies between planned and actual research
2. **Update Status**: Mark completed research as done
3. **Document Discoveries**: Capture undocumented findings and insights
4. **Realign Plans**: Adjust future research based on current understanding
5. **Preserve Context**: Maintain history of what was discovered vs. what was expected

## Command Arguments

Parse $ARGUMENTS for options:
- `--last [timeframe]` - Only check research from specified timeframe (e.g., "7d", "2w", "1m")
- `--domain [area]` - Sync specific research domain only
- `--confidence [high|medium|low]` - Only apply updates at specified confidence level
- `--dry-run` - Preview changes without applying them
- `--verbose` - Include detailed evidence in output
- `--interactive` - Prompt for confirmation on ambiguous cases

## Sync Process

### Phase 1: Research Reality Assessment

**Scan Research Artifacts**
```
1. List all files changed in the last [timeframe]
2. Identify new research documents created
3. Review recent research reports
4. Check for new citations and sources
5. Scan framework updates
6. Review synthesis documents
```

**Extract Research Signals**
- New framework sections that match planned research
- Citation additions in specific areas
- Research reports completed
- Analysis documents with conclusions
- Updated methodology notes
- New discovery records

### Phase 2: Research Plan Comparison

**Load Active Research Plans**
```
From context network, gather:
- Current research sprint tasks
- Active investigation plans
- In-progress research questions
- Recent research handoffs
- Pending synthesis items
```

**Create Research Comparison Matrix**
```markdown
| Planned Research | Expected Outputs | Found Outputs | Status | Confidence |
|------------------|------------------|---------------|---------|------------|
| Literature Review X | research_reports/x.md | ✓ Exists | Likely Done | High |
| Framework Study Y | analysis/y_framework.md | ✗ Not found | Not Started | High |
| Citation Update Z | Updated citations in doc | ✓ Partial | In Progress | Medium |
```

### Phase 3: Research Drift Detection

**Identify Research Completion Patterns**

1. **Definitely Completed**:
   - Research report exists with conclusions
   - Citations added to target documents
   - Framework sections updated
   - Synthesis integrated into context network
   - Follow-up questions documented

2. **Partially Completed**:
   - Research started but not concluded
   - Some sources gathered but not synthesized
   - Draft analysis without final conclusions
   - Citations collected but not integrated

3. **Not Started**:
   - No research artifacts found
   - No progress on investigation
   - No preliminary notes or sources

4. **Divergent Research**:
   - Investigation took different direction
   - Different methodology used
   - Scope changed during research
   - Unexpected findings led elsewhere

### Phase 4: Research Evidence Gathering

**For Each Suspected Research Completion**:

```markdown
## Evidence for Research Completion: [Research Question]

### Direct Evidence
- Report created: `path/to/report.md` (created: timestamp)
- Analysis completed: `path/to/analysis.md` (covers X aspects)
- Citations added: `document.md` (line numbers)

### Supporting Evidence
- Sources referenced: [list of new citations]
- Framework updates: [sections modified]
- Cross-references created: [links added]
- Discovery records: [insights documented]

### Counter-Evidence
- Missing expected outputs: [list]
- Incomplete synthesis: [what's not integrated]
- No validation: [claims not verified]

### Confidence Assessment: [High/Medium/Low]
Reasoning: [Why we believe this research is/isn't complete]
```

### Phase 5: Context Network Updates

**Generate Research Update Operations**:

1. **Research Task Status Updates**
```markdown
## Research Task: [Research Question]
Old Status: Planned/In Progress  
New Status: Completed
Evidence: [Summary of research outputs]
Completed Date: [Best estimate from file timestamps]
Researched By: [From document history if available]
Findings Summary: [Key discoveries]
Deviations from Plan: [Any scope changes noted]
```

2. **New Documentation Needs**
```markdown
## Undocumented Research: [Investigation]
What Exists: [Reports/analysis found]
What's Missing: [Integration gaps]
Key Findings: [Inferred from research]
Synthesis Needs: [Framework integration required]
```

3. **Research Plan Adjustments**
```markdown
## Research Plan Realignment: [Domain]
Original Plan: [What was intended to research]
Actual Research: [What was investigated]
Key Findings: [What was discovered]
Remaining Questions: [What still needs investigation]
Recommended Next Steps: [Based on current understanding]
```

### Phase 6: Research Sync Report

**Generate Comprehensive Research Sync Report**:

```markdown
# Research Sync Report - [Timestamp]

## Sync Summary
- Planned research checked: X
- Completed but undocumented: Y
- Partially completed: Z
- Divergent investigations: N
- Research questions resolved: M

## Completed Research Discovered

### High Confidence Completions
1. **[Research Question]**
   - Evidence: [Research outputs found]
   - Location: [Path to reports/analysis]
   - Key Findings: [Main discoveries]
   - Action: Mark as complete in [network location]

### Medium Confidence Completions
1. **[Research Question]**
   - Evidence: [What we found]
   - Uncertainty: [What's unclear about completion]
   - Recommended verification: [How to confirm findings]

### Partial Research
1. **[Research Question]**
   - Completed: [What research was done]
   - Remaining: [What questions remain]
   - Blockers: [Access/source issues if identifiable]

## Network Updates Required

### Immediate Updates (Automated)
- [ ] Update research status for [completed investigations]
- [ ] Create synthesis stubs for [completed research needing integration]
- [ ] Update progress indicators in [research plans]
- [ ] Add findings to [framework documents]

### Manual Review Needed
- [ ] Verify partial research completion of [investigation]
- [ ] Investigate divergent research path for [question]
- [ ] Resolve ambiguous research status of [investigation]
- [ ] Update research methodology for [domain]

## Research Drift Patterns Detected

### Systematic Issues
- Documentation lag: [Time between research and integration]
- Synthesis gaps: [Research not integrated into frameworks]
- Citation inconsistencies: [Missing or inconsistent attributions]

### Recommendations
1. [Research process improvement suggestion]
2. [Integration automation opportunity]
3. [Quality checkpoint addition recommendation]

## Applied Changes

### Files Updated
- `path/to/research-status.md`: Marked 3 investigations complete
- `path/to/research-plan.md`: Updated progress metrics
- `path/to/findings-log.md`: Added discovered research

### Files Created
- `path/to/undocumented-research.md`: Research integration stub
- `path/to/research-drift-log-YYYY-MM-DD.md`: Detailed drift record

### Validation Needed
- Please review: `path/to/ambiguous-research.md`
- Confirm completion: `path/to/partial-investigation.md`
```

## Research Detection Heuristics

### Research Pattern Matching
```yaml
Research Planning → Completion Patterns:
  Literature Review:
    planned: "Review research on X topic"
    evidence:
      - research_archives/*/x_topic*.md
      - citations added to related docs
      - synthesis in analysis/
      
  Framework Analysis:
    planned: "Analyze Y framework"
    evidence:
      - analysis/frameworks/y_analysis.md
      - comparison documents
      - integration notes
      
  Citation Research:
    planned: "Find sources for Z claims"
    evidence:
      - new citations in target documents
      - source quality improvements
      - citation format updates
```

### Research Confidence Scoring
```
High Confidence (90%+):
- Research report with conclusions exists
- Citations properly integrated
- Framework sections updated
- Synthesis documented

Medium Confidence (60-89%):
- Research started with some findings
- Sources gathered but not fully synthesized
- Some integration completed
- Questions partially answered

Low Confidence (30-59%):
- Only preliminary research exists
- Sources collected but not analyzed
- No conclusions documented
- Could be coincidental activity
```

## Special Research Cases

### Handling Research Pivots
When research took different direction than planned:
1. Check for scope change documentation
2. Look for new research questions emerged
3. Scan for methodology adjustments
4. Check for unexpected findings impact

### Handling Incomplete Research
When partial research is found but stale:
1. Check last activity dates
2. Look for "TODO" or "INVESTIGATE" markers
3. Check if superseded by other research
4. Look for blocking access/source issues

### Handling Serendipitous Discoveries
When unexpected research outputs are found:
1. Check for "discovery" or "insight" markers
2. Look for cross-domain connections
3. Check for new research directions opened
4. Look for framework implications

## Sync Command Options

```bash
/sync                      # Full sync of all active research
/sync --last 7d           # Only check research from last 7 days  
/sync --domain frameworks # Sync specific research domain
/sync --confidence high   # Only apply high-confidence updates
/sync --dry-run          # Preview changes without applying
/sync --verbose          # Include detailed evidence
/sync --interactive      # Prompt for ambiguous cases
```

## Red Flags During Research Sync

1. **Large undocumented research activity** - May indicate major investigations not tracked
2. **Citations without corresponding research** - May indicate external input not documented
3. **Conflicting findings** - May indicate research quality issues
4. **Multiple analyses of same topic** - May indicate coordination issues
5. **"SPECULATION" or "UNVERIFIED" in new content** - May indicate preliminary research

## Post-Sync Actions

1. **Notify relevant researchers** of discovered completions
2. **Create follow-up tasks** for partial research
3. **Update research velocity metrics** based on actual completion
4. **Flag process improvements** based on drift patterns
5. **Schedule deep-dive review** for ambiguous research status

## Integration with Other Commands

- Run `/sync` before any research planning session
- Run `/sync` after any major research period
- Run `/sync` when onboarding new researchers
- Include `/sync --dry-run` in regular knowledge health checks
- Chain with audit command: `/sync && /audit`