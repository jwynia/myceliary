# plan

Research planning and framework development mode

## 🚫 Implementation Restrictions

**THIS IS A PLANNING-ONLY COMMAND**

You are now in Research Planning Mode for: $ARGUMENTS

In this mode, you MUST:
- ✅ Research and understand the topic/domain
- ✅ Document findings in the context network
- ✅ Design frameworks and methodologies
- ✅ Create research task breakdowns
- ✅ Identify research dependencies and gaps

You MUST NOT:
- ❌ Write implementation code
- ❌ Create files outside context-network/
- ❌ Modify existing research without proper integration
- ❌ Make claims without supporting evidence
- ❌ Skip documentation of research process

## Research Planning Process

### Phase 1: Research Domain Understanding 🔍

1. **Define the Research Question**
   - What are we trying to understand?
   - Why does this research matter?
   - Who will benefit from these findings?
   - What are the success criteria for this investigation?

2. **Explore the Current Knowledge State**
   - Search existing context network for related research
   - Check research archives for prior investigations
   - Identify what already exists in the knowledge base
   - Document current gaps and limitations

3. **Gather Research Requirements**
   - Research scope and boundaries
   - Quality standards for evidence
   - Methodological constraints
   - Assumptions to validate

### Phase 2: Literature & Knowledge Discovery 🔬

1. **Research Existing Knowledge**
   - Academic literature and theoretical foundations
   - Similar frameworks in the knowledge base
   - External sources and expert perspectives
   - Case studies and practical applications

2. **Source Evaluation**
   - Available sources and their credibility
   - Compatibility with existing frameworks
   - Researcher expertise requirements
   - Long-term maintenance of findings

3. **Document Research Findings**
   ```
   context-network/research/$ARGUMENTS/
   ├── overview.md           # Research question and scope
   ├── findings.md          # Detailed discoveries
   ├── sources.md           # Source evaluation and citations
   └── gaps.md              # Knowledge gaps identified
   ```

### Phase 3: Framework Design 📐

1. **Conceptual Framework**
   - Core concepts and definitions
   - Relationship mappings
   - Theoretical foundations
   - Logical structure

2. **Detailed Framework Components**
   - Create framework specifications
   - Document design rationale
   - Specify evaluation criteria
   - Define application boundaries

3. **Integration Planning**
   - How this fits with existing frameworks
   - Connection points with current knowledge
   - Synthesis strategy for conflicting information
   - Validation requirements

4. **Document Framework**
   ```
   context-network/analysis/frameworks/$ARGUMENTS/
   ├── overview.md          # Framework summary
   ├── components.md        # Detailed components
   ├── relationships.md     # How components interact
   ├── validation.md        # How to validate framework
   └── applications.md      # How to apply framework
   ```

### Phase 4: Research Task Decomposition 📋

1. **Break Down Into Research Tasks**
   Each research task should be:
   - **Independent**: Can be investigated in isolation
   - **Scoped**: Clear research boundaries and deliverables
   - **Answerable**: Defined success criteria
   - **Estimated**: Rough effort estimate (Hours/Days/Weeks)

2. **Research Task Template**
   ```markdown
   ## Research Task: [Research Question]
   
   ### Scope
   - What this investigation includes
   - What this investigation excludes
   
   ### Dependencies
   - Prerequisites: [What knowledge/research must come first]
   - Blockers: [What could prevent completion]
   
   ### Success Criteria
   - [ ] Criterion 1 (specific, measurable)
   - [ ] Criterion 2 (specific, measurable)
   
   ### Estimated Effort
   - Duration: [Hours/Days/Weeks]
   - Complexity: [Low/Medium/High]
   
   ### Research Methodology
   - Information sources to consult
   - Analysis approach
   - Validation methods
   ```

3. **Create Research Plan**
   ```
   context-network/planning/$ARGUMENTS/
   ├── research-breakdown.md    # All research tasks with details
   ├── dependencies.md          # Research dependency graph
   └── research-sequence.md     # Suggested investigation order
   ```

### Phase 5: Research Risk Assessment ⚠️

1. **Identify Research Risks**
   - Source availability risks (access, quality)
   - Methodology risks (bias, validity)
   - Integration risks (conflicting findings)
   - Scope risks (too broad/narrow)
   - Timeline risks (underestimation)

2. **Research Risk Register**
   ```markdown
   ## Risk: [Risk Name]
   
   ### Description
   [What could compromise the research]
   
   ### Probability
   [Low/Medium/High]
   
   ### Impact
   [Low/Medium/High]
   
   ### Mitigation
   - Preventive measures
   - Alternative approaches
   
   ### Early Warning Signs
   - What to watch for during research
   ```

3. **Document Research Risks**
   ```
   context-network/planning/$ARGUMENTS/
   └── research-risks.md   # All identified research risks
   ```

### Phase 6: Quality Assurance Planning 🎨

Before finalizing the research plan, check:

1. **Methodological Rigor**
   - Is the approach systematic?
   - Are biases acknowledged?
   - Is validation planned?

2. **Evidence Standards**
   - What constitutes adequate evidence?
   - How will conflicting sources be handled?
   - What are the citation requirements?

3. **Integration Strategy**
   - How will findings be synthesized?
   - What documentation is required?
   - How will quality be maintained?

4. **Research Completeness**
   - Are all aspects covered?
   - Have alternative perspectives been considered?
   - Is the scope appropriate?

5. **Alternative Approaches**
   - Have we considered other methodologies?
   - Why is this approach best?
   - What are we trading off?

6. **Framework Validation**
   - How will we test the framework?
   - What are the application criteria?
   - How will we measure success?

## Deliverables Checklist

### Required Documentation
- [ ] Research question definition in context network
- [ ] Literature review and source evaluation
- [ ] Framework design with validation criteria
- [ ] Research task breakdown with estimates
- [ ] Research dependency graph
- [ ] Research risk assessment
- [ ] Research readiness checklist

### Framework Artifacts
- [ ] Conceptual framework document
- [ ] Component specifications
- [ ] Relationship mappings
- [ ] Application guidelines
- [ ] Validation methodology

### Planning Artifacts
- [ ] Scoped research task list
- [ ] Investigation sequence
- [ ] Resource requirements
- [ ] Timeline estimates
- [ ] Success metrics

## Research Readiness Checklist

Before any investigation begins, ensure:

### Understanding
- [ ] Research question is clearly defined
- [ ] Scope is documented
- [ ] Constraints are identified
- [ ] Quality standards are established

### Design
- [ ] Framework structure is planned
- [ ] Validation criteria are specified
- [ ] Integration points are defined
- [ ] Methodological approach is chosen

### Planning
- [ ] Research tasks are broken down
- [ ] Dependencies are mapped
- [ ] Risks are assessed
- [ ] Sequence is determined

### Preparation
- [ ] Sources have been identified
- [ ] Access requirements are met
- [ ] Documentation standards are clear
- [ ] Quality review process exists

## Output Structure

All planning artifacts go in the context network:

```
context-network/
├── planning/
│   └── $ARGUMENTS/
│       ├── README.md              # Planning overview
│       ├── research-question.md   # What we're investigating
│       ├── methodology.md         # How we'll research it
│       ├── research-breakdown.md  # Research task breakdown
│       ├── dependencies.md        # What depends on what
│       ├── research-risks.md      # What could go wrong
│       └── readiness-checklist.md # Are we ready?
├── analysis/frameworks/
│   └── $ARGUMENTS/
│       ├── overview.md           # Framework design
│       ├── components.md         # Detailed components
│       └── validation.md         # How to validate
└── research/
    └── $ARGUMENTS/
        ├── sources.md           # Source evaluation
        └── gaps.md              # Knowledge gaps
```

## Success Criteria

This planning session is successful when:

1. **Complete Understanding**: The research domain is thoroughly explored
2. **Clear Framework**: Design decisions are documented and justified
3. **Actionable Research**: Work is broken into independent, answerable questions
4. **Identified Risks**: Potential issues are documented with mitigations
5. **No Premature Research**: Zero investigation has occurred without proper planning
6. **Team Alignment**: Plan can be understood by any researcher

## Remember

> "Weeks of research can save you hours of planning" - Adapted

Take the time to understand deeply, design thoughtfully, and plan comprehensively. The goal is to create a research plan so clear that investigation becomes systematic and findings become reliable.

**Now, let's plan research for: $ARGUMENTS**