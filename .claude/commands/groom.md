# groom

Transform research tasks into clear, actionable items ready for investigation or synthesis

## Usage

Analyze research tasks, investigation needs, and knowledge gaps to create a well-organized backlog of actionable research work.

## Grooming Request
$ARGUMENTS

## Command Options

Parse $ARGUMENTS for options:
- `--ready-only` - Only show tasks ready for immediate research
- `--blocked` - Focus on identifying and unblocking research blockers
- `--stale [days]` - Re-groom tasks older than specified days
- `--domain [name]` - Groom tasks for specific research domain only
- `--complexity [trivial|small|medium|large]` - Filter by research complexity
- `--generate-sprint` - Create research sprint plan from groomed tasks

## Grooming Process

### Phase 1: Research Task Inventory & Classification

**Scan all task sources:**
- `/tasks/research/*.md`
- `/tasks/synthesis/*.md`
- `/tasks/frameworks/*.md`
- `/planning/research-backlog.md`
- `/analysis/**/*.md` (for follow-up research)
- `/context-network/**/*.md` (for research questions)
- Files with "RESEARCH:", "INVESTIGATE:", "VALIDATE:" markers

**Classify each task as:**
- **A: Research Complete** - Marked done but needs synthesis or integration
- **B: Ready to Research** - Clear question, sources identified, no blockers
- **C: Needs Refinement** - Vague research question or missing context
- **D: Blocked** - Waiting on access, prior research, or decisions
- **E: Obsolete** - No longer relevant or superseded by findings

### Phase 2: Research Reality Check

For each task, assess:
- **Still Relevant?** Check against current framework state
- **Prerequisites Met?** Identify missing background research
- **Research Question Clear?** Flag ambiguities or scope issues
- **Success Criteria Defined?** Note what constitutes "answered"
- **Complexity Estimate:** Trivial/Small/Medium/Large/Unknown

### Phase 3: Research Task Enhancement

Transform vague research into actionable investigations with:
- Specific, answerable research question
- Clear research context and rationale
- Source requirements and access needs
- Success criteria and deliverables
- Research methodology notes
- Dependencies on other investigations
- Effort estimate (hours/days)
- Related framework/document links

### Phase 4: Research Dependency Analysis

Create dependency map showing:
- Research ready now (no dependencies)
- Research ready after current investigations
- Blocked chains with specific access/knowledge blockers
- Decision points or framework choices needed

### Phase 5: Research Priority Scoring

Score tasks based on:
- Framework impact (High/Medium/Low)
- Research urgency (High/Medium/Low)
- Effort required (Trivial/Small/Medium/Large)
- Dependencies (None/Few/Many)
- Source accessibility (Easy/Moderate/Difficult)

### Phase 6: Generate Groomed Research Backlog

## Output Format

```markdown
# Groomed Research Backlog - [Date]

## 🔍 Ready for Research

### 1. [Specific Research Question]
**One-liner**: [What this investigation will determine]
**Effort**: [Time estimate]
**Sources needed**: 
- [List key sources or source types]

<details>
<summary>Full Research Details</summary>

**Context**: [Why this research is needed]
**Success Criteria**:
- [ ] [Specific, measurable outcome]
- [ ] [Another deliverable]

**Research Plan**:
1. [First concrete research step]
2. [Second step]

**Key Sources to Investigate**:
- [Primary sources]
- [Secondary sources]

**Watch Out For**: [Bias, limitations, or methodological issues]

**Deliverable**: [What document/section will be created/updated]

</details>

---

[Additional ready research tasks...]

## ⏳ Ready Soon (Blocked)

### [Research Question]
**Blocker**: [What's preventing research]
**Estimated unblock**: [When access/info expected]
**Prep work possible**: [Background reading or framework prep]

## 🔍 Needs Decisions

### [Research Question]
**Decision needed**: [Methodological or scope question]
**Options**: [Different research approaches with pros/cons]
**Recommendation**: [Suggested approach]

## 🔄 Synthesis Ready

### [Completed Research]
**Status**: Research complete, needs synthesis
**Key Findings**: [Brief summary]
**Integration Target**: [Which framework/document to update]

## 🗑️ Archived Tasks

### [Research Question] - **Reason**: [Why removed/superseded]

## Summary Statistics
- Total research tasks reviewed: X
- Ready for investigation: Y
- Blocked: Z
- Synthesis ready: N
- Archived: M

## Top 3 Recommendations
1. [Most important research to tackle]
2. [Quick research win opportunity]
3. [Blocker to resolve for other research]
```

## Research Red Flags to Identify

- Research question has been "almost ready" for multiple periods
- No one can explain what "answered" looks like
- "Just investigate X" - usually hides scope problems
- Dependencies on "ongoing discussions" about methodology
- Question contains "and" - should be split into separate investigations
- "Research everything about X" without concrete deliverable
- References outdated or inaccessible sources
- Question too broad to be answerable
- Lacks clear connection to project frameworks

## Quality Checklist for Groomed Research Tasks

A well-groomed research task should allow a researcher to:
- Start investigation within 10 minutes of reading
- Know exactly what constitutes a complete answer
- Understand the research context without extensive background
- Identify all required sources and access methods
- Have realistic time estimates
- See all research dependencies explicitly listed
- Know the obvious first research step
- Understand how findings will be integrated

## Research Task Types

### Literature Review Tasks
- Systematic survey of existing research
- Clear scope and inclusion criteria
- Defined synthesis approach

### Empirical Investigation Tasks
- Specific claims to validate
- Methodology for gathering evidence
- Standards for evidence quality

### Framework Development Tasks
- Clear theoretical foundation needed
- Integration with existing frameworks
- Validation criteria

### Citation and Source Tasks
- Specific claims needing better sources
- Broken references to fix
- Source quality improvements

Remember: The goal is to transform research confusion into a prioritized list of answerable questions that any researcher can pick up and investigate successfully.