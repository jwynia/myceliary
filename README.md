# Analysis Context Network

This project is a specialized template for a context network focused on document, repository, and log analysis (more info about context networks at https://jwynia.github.io/context-networks/). It is designed to support projects where users need to analyze collections of documents, code repositories, log files, or similar sets of materials, and build a structured understanding of these materials using LLM agents.

## Purpose

This template provides a specialized structure for:

1. **Organizing Source Materials**: Tracking and managing documents, repositories, logs, or datasets that need to be analyzed
2. **Documenting Analysis Frameworks**: Capturing the methodologies and approaches used to analyze materials
3. **Recording Analysis Artifacts**: Systematically documenting entities, patterns, and relationships discovered during analysis
4. **Synthesizing Findings**: Developing coherent insights from analysis results
5. **Specifying Tool Requirements**: Documenting requirements for tools that can work with the analyzed materials

The template is particularly useful for:

- Research projects involving document analysis
- Code repository audits and understanding
- Log analysis and pattern identification
- Dataset exploration and insight generation
- Requirements gathering for tool development based on analysis findings

## Structure

The context network is organized into specialized sections:

```
context-network/
├── discovery.md                    # Navigation guide with analysis focus
├── foundation/                     # Core project information
│   ├── project_definition.md       # Analysis project goals
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
├── tools/                          # Tools for analysis
│   ├── requirements/               # Tool requirements
│   ├── evaluations/                # Tool evaluations
│   └── workflows/                  # Tool workflows
└── [additional standard sections]  # Decisions, connections, meta, etc.
```

## Getting Started

1. **Set Up Your Environment**:
   - Clone this template repository
   - Ensure you have an LLM agent with file access (see Tools section below)
   - Configure your agent with context network instructions

2. **Define Your Analysis Project**:
   - Update `foundation/project_definition.md` with your specific analysis goals
   - Document your analysis approach in `foundation/analysis_approach.md`

3. **Begin Source Material Management**:
   - Document your source materials in `source_material/inventory.md`
   - Record acquisition details in `source_material/acquisition.md`
   - Document any preprocessing in `source_material/preprocessing.md`

4. **Start Analysis**:
   - Follow the process in `processes/analysis.md`
   - Use the templates in `analysis/` directories to document your findings
   - Synthesize insights following `processes/synthesis.md`

5. **Develop Tool Requirements**:
   - Document tool requirements in `tools/requirements/` based on your analysis

## Analysis Workflow

The typical workflow for an analysis project using this template:

1. **Acquisition**: Identify and acquire source materials
2. **Ingestion**: Document and preprocess materials
3. **Framework Selection**: Choose appropriate analysis frameworks
4. **Analysis**: Identify entities, patterns, and relationships
5. **Synthesis**: Develop findings and insights
6. **Tool Requirements**: Specify requirements for tools based on analysis

## Tools

Context networks are intended to be used with an LLM agent that has file access to all of the files in the project folder.

Recommended tools include:

- **Cursor** (https://www.cursor.com/): All-in-one IDE with LLM chat and file access
- **VSCode** (https://code.visualstudio.com/) with **Cline** (https://cline.bot/): Code editor with agent capabilities
- **OpenRouter** (https://openrouter.ai/): Access to various LLM models

## Best Practices

### Classification System

This template includes an enhanced classification system specifically for analysis projects:

1. **Domain**: Primary knowledge area (Source Material, Analysis Framework, Pattern, Entity, Relationship, Finding, Tool)
2. **Source Type**: Type of source material (Document, Repository, Log, Dataset, Mixed)
3. **Analysis Stage**: Stage in the analysis process (Raw, Processed, Analyzed, Synthesized)
4. **Stability**: Change frequency expectation (Static, Semi-stable, Dynamic)
5. **Abstraction**: Detail level (Conceptual, Structural, Detailed)
6. **Confidence**: Information reliability (Established, Evolving, Speculative)
7. **Relevance**: Importance to analysis goals (Critical, High, Medium, Low)

### Relationship Types

The template includes specialized relationship types for analysis:

1. **Analysis Relationships**:
   - `extracted-from`: Information extracted from source
   - `supports`: Evidence supporting a finding
   - `contradicts`: Evidence contradicting a finding
   - `correlates-with`: Statistical correlation
   - `causes`: Causal relationship
   - `instance-of`: Example of a pattern

2. **Source Material Relationships**:
   - `version-of`: Different versions of same material
   - `derived-from`: Processed form of source
   - `references`: References another source
   - `contains`: Contains another source

### Plan/Act and Specific Scope

Use Plan mode aggressively to develop a clear analysis strategy before taking action. Break down complex analysis tasks into specific, manageable steps.

### Monitor and Validate

Regularly review analysis artifacts for accuracy and completeness. Validate findings against source materials and document confidence levels appropriately.

### Retrospective

Periodically review your analysis process and findings to identify improvements. Update the context network with lessons learned and refinements to your approach.

## Additional Resources

- Context Networks Guide: https://jwynia.github.io/context-networks/
- Custom Instructions: See `/inbox/custom-instructions-prompt.md` for agent configuration
