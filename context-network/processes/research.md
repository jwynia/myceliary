# Research Process & Citation Framework

## Purpose
This node provides a structured approach to conducting, archiving, and citing research for anti-capitalist AI applications. It defines research categories, query types, temporal organization, and citation requirements to support rigorous, traceable knowledge building.

## Classification
- **Domain:** Process Framework
- **Stability:** Semi-stable
- **Abstraction:** Detailed
- **Confidence:** Established

## Content

### Research Categories

**Basic Web Search** - Simple queries for foundational information and definitions
**News Search** - Current events, recent developments, and emerging trends
**Light Research Report** - 2-4 sources, focused synthesis on specific topics
**Standard Research Report** - 5-10 sources, comparative analysis across multiple perspectives
**Deep Research Report** - 10+ sources, comprehensive analysis with academic and practitioner sources
**Academic Literature Review** - Scholarly sources, theoretical frameworks, peer-reviewed research
**Case Study Analysis** - Detailed examination of specific implementations or failures

### One-Time Foundational Research

#### Theoretical Frameworks
**Query Type:** Deep Research Report
**Frequency:** One-time (update annually)

Example Queries:
- "anti-capitalist technology frameworks academic"
- "technology commons governance models"
- "digital sovereignty indigenous communities"
- "appropriate technology principles Schumacher"
- "convivial tools Ivan Illich technology"
- "socialist cybernetics Stafford Beer Chile"
- "platform cooperativism scholarly research"
- "technology resistance social movements"
- "decolonizing digital technology frameworks"
- "feminist technology design principles"

#### Historical Case Studies
**Query Type:** Standard Research Report
**Frequency:** One-time (expand database over time)

Example Queries:
- "Chile Project Cybersyn Allende government"
- "Zapatista autonomous technology networks"
- "Black Panthers survival programs technology"
- "cooperative technology initiatives history"
- "community technology centers movement"
- "mesh networking community resilience projects"
- "time banking software implementations"
- "participatory budgeting technology tools"
- "worker cooperative digital platforms"
- "mutual aid technology coordination tools"

#### AI/ML Technical Landscape
**Query Type:** Light Research Report
**Frequency:** One-time (quarterly updates)

Example Queries:
- "open source large language models community"
- "decentralized AI training federated learning"
- "edge computing community deployment"
- "AI bias algorithmic justice research"
- "explainable AI community accountability"
- "energy efficient AI models environmental"
- "local first software principles"
- "mesh networking AI applications"

### Ongoing Monitoring

#### Policy and Regulatory Developments
**Query Type:** News Search
**Frequency:** Weekly

Example Queries:
- "AI regulation policy developments"
- "platform regulation antitrust news"
- "digital rights legislation updates"
- "surveillance technology policy"
- "algorithmic accountability laws"
- "data protection community rights"
- "tech worker organizing news"
- "digital commons policy"

#### Movement and Organizing Developments
**Query Type:** News Search + Light Research Report
**Frequency:** Bi-weekly

Example Queries:
- "tech worker organizing union activity"
- "platform worker strikes digital organizing"
- "community technology organizing"
- "digital rights activism news"
- "algorithmic justice campaigns"
- "surveillance resistance community"
- "cooperative platform development"
- "mutual aid technology innovation"
- "climate activism technology tools"
- "housing justice digital organizing"

#### Academic and Research Developments
**Query Type:** Academic Literature Review
**Frequency:** Monthly

Example Queries:
- "critical algorithm studies new research"
- "decolonial computing recent papers"
- "platform cooperativism academic research"
- "community informatics studies"
- "participatory design technology justice"
- "digital commons governance research"
- "appropriate technology sustainability"
- "technology social movements scholarship"

#### Funding and Economic Models
**Query Type:** Standard Research Report
**Frequency:** Quarterly

Example Queries:
- "community technology funding models"
- "cooperative platform financing"
- "grant funding community tech projects"
- "alternative economics technology development"
- "commons based peer production economics"
- "social economy digital platforms"
- "cooperative development funding"
- "community ownership technology"

### Crisis and Event-Driven Research

#### During Economic/Political Crises
**Query Type:** News Search + Standard Research Report
**Frequency:** As needed during crisis periods

Example Queries:
- "mutual aid technology crisis response"
- "community resilience digital tools crisis"
- "alternative communication networks emergency"
- "decentralized coordination crisis organizing"
- "surveillance resistance protest technology"
- "community self-defense digital security"

#### Technology Sector Developments
**Query Type:** Light Research Report
**Frequency:** As events occur

Example Queries:
- "big tech layoffs worker organizing"
- "AI company consolidation antitrust"
- "platform policy changes community impact"
- "surveillance technology deployment"
- "algorithmic bias discrimination cases"
- "tech whistleblower revelations"

### Geographic and Cultural Context

#### Regional Variations
**Query Type:** Standard Research Report
**Frequency:** Semi-annually per region

Example Queries:
- "Global South community technology initiatives"
- "indigenous technology sovereignty projects"
- "European platform cooperatives development"
- "Latin American community networks"
- "African indigenous knowledge technology"
- "Asian cooperative digital platforms"
- "rural community technology access"

#### Sector-Specific Applications

**Healthcare:**
- "community health technology cooperative"
- "mutual aid healthcare coordination"
- "health commons digital platforms"

**Education:**
- "community education technology platforms"
- "popular education digital tools"
- "cooperative learning management systems"

**Housing:**
- "community land trust technology"
- "housing cooperative digital platforms"
- "tenant organizing technology tools"

**Food Systems:**
- "community supported agriculture technology"
- "food distribution cooperative platforms"
- "urban agriculture coordination tools"

**Energy:**
- "community energy cooperative technology"
- "microgrid management platforms"
- "energy democracy digital tools"

### Research Execution Requirements

#### MCP Tool Usage (REQUIRED)
All research tasks MUST be executed using appropriate MCP tools:

- Basic Web Search: Use Research MCP basicWebSearch tool
- Light Research Report: Use Research MCP lightResearchReport tool
- Standard Research Report: Use Research MCP mediumResearchReport tool
- Deep Research Report: Use Research MCP deepResearchReport tool
- URL Content Capture: Use Research MCP captureUrlContent tool
- Archive Search: Use Research MCP searchLocalArchives tool

**Critical Rule:** "Ambient" knowledge or direct web browsing MUST NOT be used as substitutes for MCP tools. This ensures:
- Consistent research methodology
- Traceable information sources
- Reproducible results
- Proper archiving of findings

**Key Finding from Practice:** Experience has demonstrated that using MCP tools REDUCES overhead compared to relying on ambient knowledge. While ambient knowledge often leads to circular reasoning and ungrounded exploration, MCP tools provide:
- Concrete starting points for research
- Verified external information to ground decisions
- Clear paths forward when stuck
- Efficient ways to validate or challenge assumptions

#### Research Archiving (CRITICAL REQUIREMENT)
**All research results MUST be archived completely and unmodified**

1. **Archive Directory Structure:**
   ```
   context-network/
   ├── research_archives/
   │   ├── web_searches/         # For basicWebSearch results
   │   ├── light_reports/        # For lightResearchReport results
   │   ├── medium_reports/       # For mediumResearchReport results
   │   ├── deep_reports/         # For deepResearchReport results
   │   ├── url_captures/         # For captureUrlContent results
   │   └── research_index.md     # Master index of all research
   ```

2. **Archiving Process:**
   - When using any Research MCP tool, save the complete result to the appropriate archives directory
   - Use the archive_entry_template.md template 
   - Follow the naming convention: YYYY-MM-DD_topic_type.md
   - Update research_index.md with the new entry
   - Document key insights after review
   - Maintain the relationship between research tasks and archived results

3. **Complete Preservation:**
   - NEVER omit or truncate any part of the research results
   - Include the exact query and all parameters used
   - Document the date and context of the research
   - Include metadata about source credibility and relevance

4. **Benefits of Archiving:**
   - Ensures traceability between findings and original sources
   - Allows verification of conclusions
   - Enables historical research comparisons
   - Prevents duplication of research efforts
   - Provides proper attribution to external sources
   - Builds institutional knowledge over time

#### Citation Requirements (CRITICAL REQUIREMENT)
**All findings and analyses MUST cite their source research archives**

1. **Citation Format:**
   ```markdown
   [Citation: Research Archives, "Title of Research", YYYY-MM-DD](../../../research_archives/type/YYYY-MM-DD_topic_type.md)
   ```

2. **Citation Locations:**
   - Every finding must include a "Sources and Citations" section
   - Each significant claim must be linked to its research source
   - Each data point must cite its origin
   - Analysis methods must reference their methodological sources

3. **Source Tracking:**
   - Archive entries must record where they are cited
   - The research index must track citation frequency
   - High-impact research should be flagged for regular updates

4. **Citation Validation:**
   - Before completing a finding, verify all claims are properly cited
   - Ensure citations link to permanent archive locations
   - Validate that cited research actually supports the claims made
   - Document any conflicts or inconsistencies between sources

### Research Task Management

#### Task and Archive Integration
The research tasks and archives must be tightly integrated:

**When Creating New Tasks:**
1. Create task file using task_template.md
2. Add task to appropriate section in research_tasks_index.md
3. Update status distribution counts
4. Update priority distribution counts
5. Add any new task relationships to the mermaid diagram
6. Update metadata and change history
7. **Create placeholder for expected archive entries**

**When Executing Research:**
1. Use the specified MCP tools from the task
2. Archive the complete results immediately using archive_entry_template.md
3. Link the archived research to the original task
4. Update the research index with the new entry
5. Document key insights from the research

**When Completing Tasks:**
1. Mark task as completed in index
2. Clear next run date (use "-")
3. Update status distribution counts
4. Document completion in change history
5. Ensure findings link to archived research in analysis/findings/
6. Verify all research results have been properly archived
7. Update the "Citations and Usage" section of all archive entries

**Monthly Research Review:**
1. Verify all research is properly archived and indexed
2. Update citation statistics in the research index
3. Identify frequently cited research for potential updates
4. Clean up and organize archive entries
5. Plan new research based on gaps identified
6. Validate the integrity of research-to-finding linkages

#### Research-to-Finding Workflow
The complete workflow must maintain traceability at every step:

1. **Research Task Creation:**
   - Define specific research objectives
   - Specify required MCP tools
   - Identify expected outputs

2. **Research Execution:**
   - Use specified MCP tools
   - Archive complete results
   - Update research index

3. **Finding Development:**
   - Analyze archived research
   - Cite specific archives for all claims
   - Link back to original research task

4. **Validation:**
   - Verify all claims have proper citations
   - Ensure all research is properly archived
   - Validate conclusions against raw research
   - Document any limitations or gaps

5. **Publication:**
   - Include complete citation information
   - Provide links to archived research when appropriate
   - Document the research methodology

### Research Process Notes

**Source Prioritization:**
1. Community organizations and practitioners
2. Critical academic research
3. Movement publications and alternative media
4. Government and policy sources (with critical analysis)
5. Corporate sources (for understanding threats and co-optation)

**Geographic Balance:**
- Ensure representation from Global South perspectives
- Include indigenous and decolonial frameworks
- Balance urban and rural contexts
- Consider different political and economic systems

**Temporal Considerations:**
- Track evolution of ideas and implementations over time
- Monitor both successes and failures
- Document changing political and economic contexts
- Note seasonal patterns in organizing and development

**Quality Assessment:**
- Prioritize sources that center affected communities
- Seek diverse perspectives within anti-capitalist frameworks
- Verify claims through multiple sources
- Document conflicts and contradictions in findings

**Citation and Archiving Quality:**
- Preserve the complete context of all research
- Maintain clear linkage between claims and sources
- Enable knowledge reuse through proper indexing
- Ensure findings remain verifiable over time
- Track the impact and usage of research over time

### Citation Best Practices

#### Types of Citations

1. **Direct Research Citations:**
   - Link directly to archived research results
   - Include page/section references when applicable
   - Specify exactly what information was derived from the source

2. **Secondary Citations:**
   - When citing sources mentioned within research reports
   - Always note that these are secondary citations
   - Attempt to locate and archive primary sources when possible

3. **Synthesized Citations:**
   - When a claim is supported by multiple research sources
   - Link to all contributing research archives
   - Explain how the sources were synthesized

#### Citation Context Requirements

1. **Claim Support:**
   - Every significant claim requires a citation
   - The citation must actually support the specific claim
   - The support should be explicit, not inferred

2. **Contextual Integrity:**
   - Maintain the original context of cited information
   - Note any limitations or caveats from the original
   - Avoid selective citation that distorts meaning

3. **Dissenting Views:**
   - Document contradictory sources when they exist
   - Explain reasoning for preferring one source over another
   - Acknowledge limitations in our understanding

4. **Source Evaluation:**
   - Include credibility and relevance assessments
   - Note potential biases or limitations
   - Document the date/currency of the information

#### Citation Format Examples

**Basic Citation:**
```markdown
The open-source LLM ecosystem includes models like LLaMA 3.1, BLOOM, and Falcon 180B. [Citation: Research Archives, "AI/ML Open Source Models Survey", 2025-05-15](../../../research_archives/light_reports/2025-05-15_ai_ml_models_light.md)
```

**Multiple Source Citation:**
```markdown
Community-controlled AI systems can operate effectively on edge hardware [Citation: Research Archives, "Edge Computing Requirements", 2025-05-10](../../../research_archives/medium_reports/2025-05-10_edge_computing_medium.md), with significantly reduced energy consumption [Citation: Research Archives, "AI Energy Efficiency", 2025-05-12](../../../research_archives/deep_reports/2025-05-12_ai_energy_deep.md).
```

**Contextual Citation:**
```markdown
While some research suggests federated learning can fully preserve privacy [Citation: Research Archives, "Federated Learning Claims", 2025-05-20](../../../research_archives/web_searches/2025-05-20_federated_learning_search.md), our analysis found significant vulnerabilities in practical implementations.
```

## Relationships
- **Parent Nodes:**
  - foundation/project_definition.md - is-child-of - Implements core project vision
- **Child Nodes:**
  - research_archives/research_index.md - is-parent-of - Provides structure for research archives
  - research_archives/archive_entry_template.md - is-parent-of - Defines standard format for archive entries
- **Related Nodes:**
  - analysis/frameworks/anti_capitalist_framework.md - supports - Provides research methodology for framework application
  - analysis/frameworks/capitalist_trap_detector.md - supports - Provides research methodology for trap detection
  - processes/analysis.md - relates-to - Guides analysis of research findings
  - processes/synthesis.md - relates-to - Guides synthesis of research findings
  - analysis/findings/finding_template.md - relates-to - Defines how research should be cited in findings

## Navigation Guide
- **When to Use:**
  - When starting new research initiatives
  - When monitoring ongoing developments
  - When responding to emerging events or crises
  - When expanding geographic or sector coverage
  - When archiving research results
  - When creating findings that cite research

- **Next Steps:**
  1. Select appropriate query type based on research needs
  2. Follow source prioritization guidelines
  3. Archive complete research results
  4. Document findings with proper citations
  5. Feed results into relevant analysis frameworks

- **Related Tasks:**
  - Research planning and coordination
  - Source evaluation and selection
  - Research archiving and citation
  - Finding synthesis and documentation
  - Knowledge base maintenance
  - Citation validation and verification

## Metadata
- **Created:** 2025-06-03
- **Last Updated:** 2025-06-11
- **Updated By:** Cline (Research Citation System Update)

## Change History
- 2025-06-11: Major update to add research archiving and citation requirements
- 2025-06-03: Initial integration from research_queries_framework.md into context network structure
