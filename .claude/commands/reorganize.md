# reorganize

Restructure and optimize knowledge organization in the context network

## Usage

When the context network becomes unwieldy, redundant, or poorly structured, use this command to systematically reorganize knowledge for better clarity, accessibility, and maintenance.

## Reorganization Triggers

Consider reorganization when:
- Navigation becomes difficult
- Duplicate information exists across documents
- Concepts blur together without clear boundaries
- New understanding invalidates current structure
- Relationships between concepts have shifted
- Documents exceed recommended size limits (100-300 lines)
- Search becomes ineffective

## Phase 1: Structure Analysis

### Current State Assessment

1. **Map Existing Structure**
   - Document current organization hierarchy
   - Identify all major concept clusters
   - Map cross-references and dependencies
   - Note navigation patterns

2. **Identify Problems**
   - Locate duplicate information
   - Find orphaned documents
   - Identify oversized documents
   - Document broken or circular references
   - Note confusing navigation paths

3. **Usage Pattern Analysis**
   - Which documents are frequently accessed together?
   - What search patterns indicate poor organization?
   - Where do navigation paths break down?
   - Which concepts are consistently mislocated?

## Phase 2: Reorganization Planning

### Design New Structure

1. **Define Organization Principles**
   - Establish consistent categorization scheme
   - Create naming conventions
   - Define document size targets
   - Specify relationship types

2. **Plan Document Changes**
   - **Split**: Large documents into focused pieces
   - **Merge**: Related fragments into coherent wholes
   - **Move**: Misplaced content to proper locations
   - **Delete**: Redundant or obsolete information
   - **Create**: Missing navigation hubs or indexes

3. **Map Transition**
   - Create migration checklist
   - Identify high-risk changes
   - Plan redirect/alias strategy
   - Document rollback approach

## Phase 3: Content Reorganization

### Reorganization Patterns

#### Pattern: Document Splitting
When documents exceed 300 lines or cover multiple concepts:
```
Before: framework_complete.md (500 lines)
After:
  - framework_overview.md (150 lines)
  - framework_components.md (200 lines)  
  - framework_examples.md (150 lines)
  - framework_index.md (navigation hub)
```

#### Pattern: Concept Clarification
When boundaries between concepts blur:
```
Before: Mixed concepts in multiple files
After:
  - concept_a_definition.md (pure concept)
  - concept_b_definition.md (pure concept)
  - concept_comparison.md (relationships)
  - implementation_guidance.md (practical application)
```

#### Pattern: Hierarchy Flattening
When navigation depth impedes discovery:
```
Before: deep/nested/structure/concept.md
After: 
  - domain/concept.md
  - domain/index.md (with logical grouping)
```

#### Pattern: Hub Creation
When related documents lack central navigation:
```
Create: domain_hub.md
  - Overview of domain
  - Key concepts list with links
  - Common workflows
  - Related domains
```

## Phase 4: Implementation

### Execution Steps

1. **Create New Structure**
   - Create new directories as needed
   - Generate navigation hubs
   - Establish index documents

2. **Migrate Content**
   - Copy content to new locations
   - Update internal links
   - Preserve important history
   - Maintain citation integrity

3. **Update References**
   - Fix all cross-references
   - Update navigation paths
   - Modify task references
   - Adjust research citations

4. **Clean Up**
   - Remove empty directories
   - Delete redundant files
   - Archive obsolete content
   - Optimize file names

## Phase 5: Validation

### Quality Checks

1. **Structure Validation**
   - All documents within size limits
   - Clear concept boundaries
   - Logical hierarchy
   - Effective navigation paths

2. **Link Integrity**
   - No broken references
   - No circular dependencies
   - All documents reachable
   - Citations remain valid

3. **Content Completeness**
   - No information lost
   - All concepts represented
   - Relationships preserved
   - Context maintained

## Reorganization Principles

### Single Responsibility
Each document should have one clear purpose:
- Define a concept
- Provide navigation
- Document relationships
- Present examples

### Atomic Notes
Keep documents small and focused:
- 100-300 lines maximum
- One main idea per file
- Extensive linking between related notes
- Clear, descriptive titles

### Progressive Disclosure
Organize from general to specific:
- Overview → Details
- Concept → Implementation
- Theory → Practice
- Abstract → Concrete

### Consistent Naming
Use predictable patterns:
- `concept_name.md` for definitions
- `domain_index.md` for navigation
- `topic_examples.md` for practical applications
- `comparison_x_vs_y.md` for relationships

## Anti-Patterns to Avoid

1. **Big Bang Reorganization**: Changing everything at once
2. **Perfect Structure Paralysis**: Over-planning without executing
3. **Lost History**: Removing valuable context or evolution
4. **Broken Gardens**: Creating areas that quickly decay
5. **Over-Categorization**: Too many categories with few documents

## Metrics for Success

**Before/After Comparison:**
- Average document size reduced
- Navigation depth decreased
- Search effectiveness improved
- Duplicate content eliminated
- Cross-references increased
- Dead links eliminated

## Rollback Strategy

Always maintain ability to reverse changes:
1. Document original structure
2. Keep archive of moved content
3. Maintain redirect mapping
4. Test critical paths first
5. Implement in phases

## Completion Checklist

- [ ] Current structure analyzed and documented
- [ ] Reorganization plan created and reviewed
- [ ] New structure implemented
- [ ] All content successfully migrated
- [ ] References and links updated
- [ ] Navigation paths tested
- [ ] Quality validation completed
- [ ] Old structure archived (not deleted)
- [ ] Team notification sent (if applicable)