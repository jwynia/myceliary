# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Critical: Context Network is Source of Truth

This project uses a Context Network for ALL planning, architecture, and coordination information. The context network location and structure are defined in `.context-network.md`.

### Your Primary Responsibilities

1. **ALWAYS check the context network FIRST** before starting any work
2. **NEVER duplicate information** between CLAUDE.md and the context network
3. **UPDATE the context network** as you work - don't wait until task completion
4. **RECORD your understanding** in the context network, not just in conversation
5. **CREATE discovery records** when finding important information in source files

## Workflow Requirements

### Before Starting ANY Task

```
1. Read `.context-network.md` to locate the context network
2. Navigate to relevant sections based on your task
3. Create a new task entry in the context network's active tasks section
4. Document your understanding of:
   - What you're trying to accomplish
   - Which existing components/systems are involved
   - Your planned approach
```

### During Work

**Every 3-5 significant changes or discoveries:**
1. STOP and update the context network with:
   - What you've learned
   - What you've changed
   - Any new connections or dependencies discovered
   - Questions or uncertainties that arose

**When you find yourself re-reading the same files:**
- This is a signal you haven't recorded your understanding
- Create a summary in the context network immediately

**When discovering important information:**
1. Create a discovery record with:
   - What you found
   - Exact file path and line numbers
   - Why it's significant
   - How it connects to your current task
2. Link this discovery to relevant concept nodes

### The 3-Line Rule

If you read more than 3 lines of code to understand something, you MUST record:
1. What question you were trying to answer
2. Where you found the answer (file:lines)
3. What the answer means in plain language

### After Completing Work

1. Update all modified nodes in the context network
2. Create/update the task completion record
3. Document any follow-up items or discovered issues

## Context Network Update Triggers

You MUST update the context network when:
- Starting a new task or subtask
- Making architectural decisions
- Discovering new relationships between components
- Finding bugs or issues
- Learning how a system works
- Planning implementation approach
- Every 10-15 minutes of active work
- **Finding important information in source files** (create a discovery record)

### Create Discovery Records For:
- **Entry points**: Where key processes begin
- **State changes**: Where important data is modified
- **Decisions**: Where the code chooses between alternatives
- **Connections**: Where components interact
- **Surprises**: Where reality differs from expectations

## What Goes Where

### Context Network (Team Memory)
- Architecture diagrams and decisions
- Implementation plans and strategies
- Task records and progress
- System understanding and documentation
- Research findings and explorations
- Bug investigations and solutions
- Design discussions and rationale
- **Discovery records and location indexes**

### Project Files (Build Artifacts)
- Source code
- Configuration files
- Tests
- Build scripts
- Public documentation
- Resources used by the application

## Information Organization Principles

### Create Small, Focused Documents

**NEVER create large, monolithic documents.** Instead:
- One concept = one file (atomic notes)
- 100-300 lines maximum per document
- Link extensively between related documents
- Use index/hub documents to provide navigation

### Discovery Record Format

```markdown
## [What You Were Looking For]
**Found**: `path/to/file.ts:45-67`
**Summary**: [One sentence explaining what this code does]
**Significance**: [Why this matters for understanding the system]
**See also**: [[related-concept]], [[another-discovery]]
```

### Maintain Specialized Indexes

1. **Location Indexes** (`discoveries/locations/[component].md`):
   ```markdown
   # [Component] Key Locations
   
   ## Configuration Loading
   - **What**: How config files are parsed and validated
   - **Where**: `src/config/parser.ts:45-72`
   - **Related**: [[config-schema]], [[validation-rules]]
   
   ## State Management
   - **What**: Central state store implementation
   - **Where**: `src/store/index.ts:12-38`
   - **Related**: [[state-shape]], [[action-patterns]]
   ```

2. **Concept Maps** (`concepts/[concept].md`):
   ```markdown
   # [Concept Name]
   
   ## Definition
   [Brief explanation]
   
   ## Implementations
   - [[location-index#section]] - Where this is implemented
   - [[example-usage]] - How it's used in practice
   
   ## Related Concepts
   - [[parent-concept]] - Broader context
   - [[sibling-concept]] - Alternative approach
   - [[child-concept]] - Specific implementation
   ```

3. **Task Discovery Logs** (`tasks/[date]-[task]/discoveries.md`):
   ```markdown
   # Discoveries for [Task Name]
   
   ## Key Findings
   1. **Config validation happens in two places**
      - Primary: `src/config/parser.ts:45`
      - Secondary: `src/runtime/validate.ts:23`
      - This seems unintentional - [[tech-debt-001]]
   ```

### Linking Patterns

Use consistent link types:
- `[[concept]]` - Link to concept definition
- `[[location-index#section]]` - Link to specific location
- `[[task/discoveries]]` - Link to task-specific findings
- `→ file.ts:line` - Direct code reference (non-linked)

### Navigation Hubs

Create navigation hubs at multiple levels:
- Domain hubs: Overview of a functional area
- Component hubs: Entry point for understanding a component
- Task hubs: Central point for all task-related information

### Search Optimization

Name files and sections for discoverability:
- Use consistent naming patterns
- Include keywords in headers
- Create "alias" sections for alternative terms
- Maintain a glossary of project-specific terms

### Discovery Index Maintenance

Every 5-10 discoveries:
1. Check if they share a theme
2. Create or update a concept document that links them
3. Add entries to the appropriate location index
4. Update navigation hubs to include new findings

## Prohibited Practices

NEVER:
- Create planning documents outside the context network
- Wait until task completion to update the context network
- Rely solely on reading source code without documenting understanding
- Make architectural decisions without recording them
- Duplicate information between CLAUDE.md and context network
- Keep mental notes of "I saw this somewhere" without recording it
- Create long documents explaining entire files (use focused records instead)
- Assume you'll remember why something was important
- Create duplicate explanations of the same code (link to existing records)

## Context Network Structure Reference

The context network structure is defined within the network itself. Always refer to the network's own navigation guide rather than maintaining a duplicate here.

## Quick Checklist

Before claiming a task is complete, verify:
- [ ] Context network task entry exists and is updated
- [ ] All architectural decisions are documented
- [ ] Implementation approach is recorded
- [ ] Discovered relationships are mapped
- [ ] Discovery records created for all significant findings
- [ ] Location indexes updated with new discoveries
- [ ] Navigation hubs updated if needed
- [ ] Follow-up items are noted
- [ ] No planning documents exist outside the context network
- [ ] All documents follow the 100-300 line limit

## Project Overview

Myceliary is a research and documentation project developing anti-capitalist AI frameworks and tools for non-capitalist benefits to community and mutual aid with the assistance of AI. The project uses a "context network" structure to organize knowledge about identifying, evaluating, and building AI applications that serve human needs outside capitalist structures.

## Repository Structure

```
/workspaces/myceliary/
├── context-network/          # Core knowledge base
│   ├── foundation/          # Project definition, principles, approach
│   ├── analysis/            # Frameworks, patterns, findings
│   ├── processes/           # Research and analysis workflows
│   └── research_archives/   # Citation system and research reports
├── docs/                    # Jekyll static site (published via GitHub Actions)
└── .devcontainer/          # VS Code development container config
```


### Jekyll Site (for website publishing)

The Jekyll site in `/docs` is primarily managed through GitHub Actions for publishing. Local development is not typically needed.

## Architecture & Key Components

### Context Network Structure
- **Foundation**: Core project vision, principles, and methodology
- **Analysis**: Anti-capitalist framework, capitalist trap detector, and findings
- **Processes**: Research methodology, analysis workflows, and synthesis approaches
- **Research Archives**: Citation management system with light/medium/deep reports

### Citation System
The project uses a structured citation system in `context-network/research_archives/`:
- `research_index.md` - Central index of all research
- `light_reports/` - Quick research summaries
- `medium_reports/` - In-depth analysis
- `url_captures/` - Archived web content

### Key Frameworks
1. **Anti-Capitalist AI Framework** (`analysis/frameworks/anti_capitalist_framework.md`)
   - Systematic methodology for identifying AI applications outside capitalist incentives
   - Analysis of market failures, counter-hegemonic potential, democratization

2. **Capitalist Trap Detector** (`analysis/frameworks/capitalist_trap_detector.md`)
   - Methods for identifying when AI solutions serve capitalist interests
   - Analysis of trap patterns: efficiency, individualization, platform dependency

## Working Guidelines

### Document Integration
When adding new research or analysis:
1. Follow the process in `processes/document_integration.md`
2. Add citations to `research_archives/research_index.md`
3. Create appropriate report files in the research archives

### Git Workflow
- Main branch: `main`
- Current working files may be in progress (check git status)
- The project focuses on documentation, not code deployment

### Content Focus
This is a research project, not a software application. Focus on:
- Developing and refining analytical frameworks
- Documenting research findings
- Building the knowledge base through markdown files
- Maintaining citation consistency