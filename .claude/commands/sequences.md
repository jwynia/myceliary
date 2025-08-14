# sequences

Research workflow sequences for systematic knowledge management

## Usage

This document defines logical sequences of research commands that work together to accomplish common knowledge management workflows. These sequences can be run manually or automated.

## Daily Research Sequences

### Morning Research Review
**Purpose**: Start the day with understanding of research progress and identify ready investigations.
**When**: Daily at start of research work (e.g., 9:00 AM)

```bash
/sync --last 1d --dry-run     # Check what research was completed yesterday
/status --brief --research     # Quick research health check
/groom --ready-only           # Show today's actionable research tasks
```

**Expected Time**: 5-10 minutes
**Key Outcomes**:
- Understanding of yesterday's research progress
- Current research domain status
- Clear list of today's research priorities

### Evening Research Synthesis
**Purpose**: Capture research insights before context is lost, sync documentation with actual findings.
**When**: Daily at end of research work (e.g., 5:30 PM)

```bash
/checklist                    # Ensure no research insights are lost
/discovery                    # Document any research learnings from today
/sync --last 1d              # Update research statuses to reflect reality
```

**Expected Time**: 10-15 minutes
**Key Outcomes**:
- No lost research insights or discoveries
- Research task statuses reflect reality
- Context network is current with findings

## Weekly Research Sequences

### Monday Research Planning
**Purpose**: Start week with clear understanding of research progress and focus areas.
**When**: Monday morning (e.g., 9:00 AM)

```bash
/sync --last 1w              # Sync last week's research progress
/status --detailed --metrics  # Full research health assessment
/retrospective               # Document research lessons from last week
/groom --stale 7            # Re-groom aging research tasks
/groom --generate-sprint    # Plan the week's research sprint
```

**Expected Time**: 30-45 minutes
**Key Outcomes**:
- Last week's research properly documented
- Research lessons learned captured
- Fresh, actionable research task backlog
- Clear research sprint plan for the week

### Friday Research Quality Review
**Purpose**: Quality control, cleanup, and risk identification before weekend.
**When**: Friday afternoon (e.g., 3:00 PM)

```bash
/audit --scope research      # Review week's research quality
/review-frameworks          # Check framework quality for week's work
/maintenance                 # Clean up and organize research archives
/status --research --risks   # End-of-week research risk assessment
```

**Expected Time**: 45-60 minutes
**Key Outcomes**:
- Research quality issues identified
- Framework consistency validated
- Research archives organized
- Research risks documented for Monday

## Research Sprint Sequences (Bi-Weekly)

### Research Sprint Start
**Purpose**: Clean slate for new research sprint with properly groomed research backlog.
**When**: First day of research sprint

```bash
/sync --all                  # Full research reality sync
/groom --all                # Comprehensive research grooming
/plan research-sprint-goals  # Define sprint research architecture needs
/status --detailed          # Research baseline status
```

**Expected Time**: 60-90 minutes
**Key Outcomes**:
- Complete alignment with research reality
- All research tasks properly groomed
- Research framework needs identified
- Research sprint baseline established

### Research Sprint End
**Purpose**: Close out research sprint properly with full documentation and quality review.
**When**: Last day of research sprint

```bash
/sync --research            # Final research sprint sync
/retrospective             # Research sprint retrospective
/audit --scope research    # Research sprint quality review
/status --metrics --detailed # Research sprint metrics and analysis
/maintenance --deep        # Deep research cleanup between sprints
```

**Expected Time**: 90-120 minutes
**Key Outcomes**:
- Research sprint work fully documented
- Research retrospective insights captured
- Research quality metrics recorded
- Ready for next research sprint

## Monthly Research Sequences

### Monthly Knowledge Base Health Check
**Purpose**: Deep research health assessment and proactive maintenance.
**When**: First Monday of month (e.g., 10:00 AM)

```bash
/sync --all --verbose              # Deep research sync with evidence
/audit --all --strict             # Comprehensive research quality audit
/maintenance --deep               # Thorough research archive cleanup
/reorganize --metrics            # Identify knowledge organization opportunities
/status --detailed --metrics --risks # Full research health report
```

**Expected Time**: 2-3 hours
**Key Outcomes**:
- Complete research system health assessment
- All research quality issues identified
- Knowledge reorganization opportunities catalogued
- Comprehensive research status report

### Monthly Framework Development Review
**Purpose**: Strategic research assessment and framework planning.
**When**: Mid-month (e.g., 15th at 2:00 PM)

```bash
/audit --scope frameworks         # Framework health check
/review-frameworks --all         # Framework consistency analysis
/groom --complexity large        # Review complex research tasks
/research "framework evolution"  # Research framework improvement strategies
```

**Expected Time**: 2-3 hours
**Key Outcomes**:
- Framework issues identified
- Research consistency gaps found
- Complex research tasks re-evaluated
- Framework evolution strategies researched

## Research Integration Sequences

### Pre-Synthesis Sequence
**Purpose**: Prepare research for framework integration.
**When**: Before major research synthesis

```bash
/review-frameworks --target      # Review target framework consistency
/audit --scope citations        # Quick citation quality check
```

**Expected Time**: 2-5 minutes
**Key Outcomes**:
- Framework integration readiness validated
- No obvious citation issues in synthesis

### Post-Integration Sequence
**Purpose**: Ensure integrated research is documented and validated.
**When**: After research integration into frameworks

```bash
/sync --last 1h               # Sync integrated changes
/audit --scope integration    # Audit integrated research
/discovery                   # Document any new patterns/learnings
```

**Expected Time**: 10-15 minutes
**Key Outcomes**:
- Integrated changes tracked
- Research quality verified
- Integration patterns documented

## Special Research Event Sequences

### Research Onboarding Sequence
**Purpose**: Quickly bring new researcher up to speed.
**When**: New researcher joins

```bash
/status --detailed           # Current research state overview
/discovery --all            # Share all research discoveries
/groom --ready-only        # Show available research tasks
```

**Expected Time**: 30-45 minutes
**Key Outcomes**:
- New researcher understands current research state
- Has access to team research knowledge
- Knows what research tasks are available

### Research Crisis Recovery Sequence
**Purpose**: Recover from and learn from research methodology issues.
**When**: After research methodology problems

```bash
/sync --all                 # Understand current research reality
/status --risks            # Identify all research risks
/audit --methodology --sources # Deep methodology/source check
/retrospective            # Document research issue learnings
/plan "research-quality-measures" # Plan research quality improvements
```

**Expected Time**: 2-4 hours
**Key Outcomes**:
- Current research state understood
- All research risks identified
- Research methodology validated
- Lessons documented
- Quality improvement plan created

### Knowledge Publication Preparation Sequence
**Purpose**: Ensure readiness for knowledge publication or presentation.
**When**: Before major knowledge publication

```bash
/sync --all                    # Ensure research documentation current
/audit --all --strict         # Full research quality check
/review-frameworks --all      # Verify framework consistency
/status --detailed --risks    # Research risk assessment
/checklist                    # Final pre-publication check
```

**Expected Time**: 3-4 hours
**Key Outcomes**:
- All research changes documented
- Research quality validated
- Framework consistency confirmed
- Research risks identified
- Publication checklist complete

## Research Automation Configuration

These sequences can be automated using research management tools. Example configuration:

```yaml
# .claude/research-schedules.yaml
version: 1
schedules:
  daily:
    morning_research_review:
      time: "09:00"
      timezone: "America/New_York"
      workdays_only: true
      commands:
        - "/sync --last 1d --dry-run"
        - "/status --brief --research"
        - "/groom --ready-only"
      notify_on_error: true
      
    evening_synthesis:
      time: "17:30"
      workdays_only: true
      commands:
        - "/checklist"
        - "/discovery"
        - "/sync --last 1d"
      optional: true
  
  weekly:
    monday_research_planning:
      day: "monday"
      time: "09:00"
      commands:
        - "/sync --last 1w"
        - "/status --detailed --metrics"
        - "/retrospective"
        - "/groom --stale 7"
        - "/groom --generate-sprint"
      requires_confirmation: true
    
    friday_quality_review:
      day: "friday"
      time: "15:00"
      commands:
        - "/audit --scope research"
        - "/review-frameworks"
        - "/maintenance"
        - "/status --research --risks"
      generate_report: true
  
  monthly:
    knowledge_health_check:
      day_of_month: 1
      time: "10:00"
      commands:
        - "/sync --all --verbose"
        - "/audit --all --strict"
        - "/maintenance --deep"
        - "/reorganize --metrics"
        - "/status --detailed --metrics --risks"
      output_to: "monthly-research-health-report.md"
  
  triggered:
    pre_synthesis:
      trigger: "research:pre-synthesis"
      commands:
        - "/review-frameworks --target"
        - "/audit --scope citations"
      blocking: true
    
    post_integration:
      trigger: "research:post-integration"
      commands:
        - "/sync --last 1h"
        - "/audit --scope integration"
        - "/discovery"
      async: true
```

## Research Sequence Principles

### 1. Order Matters
- **Start with sync** - Always understand research reality first
- **Document before forgetting** - Run discovery/retrospective while research context is fresh
- **Clean as you go** - Regular maintenance prevents research debt buildup
- **Review at boundaries** - Sprint/week ends are good for research quality checks
- **Plan with fresh data** - Groom and plan after syncing research status

### 2. Escalate Research Depth Over Time
- **Daily**: Quick research checks (5-15 min)
- **Weekly**: Thorough research review (30-60 min)
- **Sprint**: Comprehensive research assessment (1-2 hours)
- **Monthly**: Deep research analysis (2-4 hours)

### 3. Fail Fast, Recover Gracefully
- Pre-synthesis checks should be fast and blocking
- Daily sequences should be resilient to research failures
- Weekly/monthly sequences should generate reports even on partial failure

### 4. Research Context Preservation
- Each sequence should be self-contained
- Output from one command should inform the next research step
- Final command should summarize or checkpoint research status

## Research Customization Guide

### Creating Custom Research Sequences

1. **Identify the Research Goal**: What research outcome do you want?
2. **Determine Research Frequency**: How often should this research run?
3. **Order Research Commands**: What research sequence makes sense?
4. **Set Research Time Budget**: How long can this research take?
5. **Define Research Success**: What indicates research completion?

### Example Custom Research Sequence

```bash
# "Framework Friday" - Weekly framework development focus
/audit --scope frameworks         # Find framework issues
/groom --tag "framework"          # Groom framework tasks
/synthesize --safe --preview      # Identify safe synthesis opportunities
/plan "framework-development"     # Plan framework work
/status --tag "framework"         # Report on framework status
```

## Research Monitoring & Metrics

Track research sequence effectiveness:

### Research Success Metrics
- **Completion Rate**: How often do research sequences finish?
- **Time to Complete**: Are they within research budget?
- **Research Issues Found**: What research problems do they catch?
- **Research Action Items Generated**: What research work do they identify?

### Research Health Indicators
- Increasing sequence duration → Growing research complexity
- Decreasing issues found → Improving research quality
- Skipped sequences → Research team overload
- Failed sequences → Research environment issues

## Research Best Practices

1. **Start Small**: Begin with daily research sequences, add weekly, then monthly
2. **Monitor Research Fatigue**: If sequences are ignored, they're too frequent
3. **Adjust Research Timing**: Run sequences when team can act on research results
4. **Keep It Relevant**: Remove commands that rarely provide research value
5. **Document Research Changes**: Track why research sequences were modified
6. **Review Research Quarterly**: Assess if sequences still serve research purpose

## Quick Start Research Recommendations

For a new research project, start with these three sequences:

1. **Daily Morning Research Review** - Maintains daily research alignment
2. **Weekly Monday Research Planning** - Keeps research backlog fresh
3. **Research Sprint End Sequence** - Ensures proper research closure

These provide the minimum viable process for maintaining research project health and documentation currency.