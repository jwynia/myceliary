# Context Network Navigation Guide for Analysis Projects

## Overview

This context network contains all planning documents, conceptual work, and coordination information for analysis projects. It is specifically designed to support the analysis of document collections, repositories, logs, or similar sets of files, facilitating collaborative work with LLM agents to understand these materials and develop tools to work with them.

## Structure

The context network is organized as follows:

```
context-network/
├── discovery.md                    # This navigation guide
├── foundation/                     # Core project information
│   ├── project_definition.md       # Analysis project purpose and goals
│   ├── structure.md                # Project structure overview
│   ├── principles.md               # Analysis principles and standards
│   └── analysis_approach.md        # Overall analysis methodology
├── source_material/                # Information about source materials
│   ├── inventory.md                # Catalog of all source materials
│   ├── acquisition.md              # How materials were acquired
│   └── preprocessing.md            # Any preprocessing applied
├── analysis/                       # Analysis-specific information
│   ├── frameworks/                 # Analysis frameworks used
│   ├── patterns/                   # Identified patterns
│   ├── entities/                   # Key entities discovered
│   ├── relationships/              # Relationships between entities
│   └── findings/                   # Key findings from analysis
├── processes/                      # Process documentation
│   ├── ingestion.md                # Source material ingestion process
│   ├── analysis.md                 # Analysis workflows
│   ├── validation.md               # Validation procedures
│   └── synthesis.md                # Synthesizing findings
├── decisions/                      # Key decisions
│   ├── decision_index.md           # Index of all decisions
│   └── [individual decision records]
├── planning/                       # Planning documents
│   ├── roadmap.md                  # Analysis roadmap
│   └── milestones.md               # Analysis milestones
├── tools/                          # Tools for analysis
│   ├── requirements/               # Tool requirements
│   ├── evaluations/                # Tool evaluations
│   └── workflows/                  # Tool workflows
├── connections/                    # Cross-cutting concerns
│   ├── dependencies.md             # Dependencies between elements
│   └── interfaces.md               # Interface definitions
├── meta/                           # Information about the network itself
│   ├── updates.md                  # Record of network changes
│   └── maintenance.md              # Network maintenance procedures
└── archive/                        # Archived documents from the inbox
```

## Navigation Paths

### For New Project Members
1. Start with `foundation/project_definition.md` to understand the project's purpose
2. Review `foundation/principles.md` to understand analysis principles
3. Explore `foundation/analysis_approach.md` for the overall methodology
4. Check `source_material/inventory.md` to understand what's being analyzed

### For Understanding Source Materials
1. Start with `source_material/inventory.md` for a catalog of materials
2. Review `source_material/acquisition.md` to understand how materials were obtained
3. Check `source_material/preprocessing.md` for any preprocessing steps applied
4. Follow the process in `processes/ingestion.md` for adding new materials

### For Conducting Analysis
1. Start with `processes/analysis.md` to understand the analysis workflow
2. Review relevant analysis frameworks in `analysis/frameworks/`
3. Check existing patterns in `analysis/patterns/` and entities in `analysis/entities/`
4. Document new findings in `analysis/findings/`

### For Tool Development
1. Start with `tools/requirements/` to understand tool needs
2. Review `tools/evaluations/` for existing tool assessments
3. Check `tools/workflows/` for how tools are used in the analysis process
4. Document new tool requirements based on analysis needs

### For Understanding Key Decisions
1. Start with `decisions/decision_index.md`
2. Navigate to specific decision records of interest
3. Review related analysis frameworks and findings

## Maintenance

This context network is maintained according to the procedures documented in `meta/maintenance.md`. All changes to the network structure should be recorded in `meta/updates.md`.

## Classification System

Information nodes in this context network are classified along these dimensions:

1. **Domain**: [Primary knowledge area]
   - Examples: Source Material, Analysis Framework, Pattern, Entity, Relationship, Finding, Tool

2. **Source Type**: [Type of source material]
   - Document, Repository, Log, Dataset, Mixed

3. **Analysis Stage**: [Stage in the analysis process]
   - Raw, Processed, Analyzed, Synthesized

4. **Stability**: [Change frequency expectation]
   - Static: Fundamental principles unlikely to change
   - Semi-stable: Established patterns that evolve gradually
   - Dynamic: Frequently changing information

5. **Abstraction**: [Detail level]
   - Conceptual: High-level ideas and principles
   - Structural: Organizational patterns and frameworks
   - Detailed: Specific implementations and examples

6. **Confidence**: [Information reliability]
   - Established: Verified and reliable information
   - Evolving: Partially validated but subject to refinement
   - Speculative: Exploratory ideas requiring validation

7. **Relevance**: [Importance to analysis goals]
   - Critical, High, Medium, Low
