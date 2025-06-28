---
layout: default
title: Welcome to Myceliary
---

# Myceliary

Welcome to Myceliary, a research project dedicated to exploring anti-capitalist frameworks and patterns in AI/ML development. Drawing inspiration from mycelial networks - nature's organic communication and resource-sharing systems - we build interconnected knowledge commons that support community-driven technology development outside of capitalist structures.

## Quick Start Guide

<pre class="mermaid">
graph TD
    A[Start Here] --> B[Research Areas]
    A --> C[Frameworks]
    A --> D[Case Studies]
    B --> E[Current Projects]
    C --> F[Analysis Tools]
    D --> G[Historical Examples]
</pre>

### Key Resources
- 🔬 [Research Dashboard](research/) - Track ongoing research and findings
- 🛠️ [Analysis Frameworks](frameworks/) - Tools for evaluating AI/ML initiatives
- 📚 [Case Studies](case-studies/) - Real-world examples and lessons
- 📊 [Latest Analysis](analysis/) - Current insights and patterns
- 💻 [P2P Platform Development](p2p_platform/) - Peer-to-peer community platform architecture
- 🚀 [High-Leverage Projects](projects/) - Strategic technology project framework
- 🔄 [Community Alternatives](alternatives/) - Replace exploitative apps with community-owned solutions
- 🛡️ [Safety Systems](safety/) - Protect vulnerable users in community platforms

## Latest Research Progress

### Active Projects
{% for task in site.data.research_tasks %}
{% if task.status == "In Progress" %}
- **{{ task.name }}** - {{ task.description }}
  - Due: {{ task.due_date }}
  - [View Details]({{ task.link }})
{% endif %}
{% endfor %}

### Recent Findings
- [P2P Community Platform Architecture](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/p2p_community_platform_architecture.md) - Technical architecture for peer-to-peer platforms
- [AI/ML Landscape Analysis](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/ai_ml_landscape_analysis.md) - Comprehensive overview of current technologies
- [Movement Monitoring Update](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/movement_monitoring_analysis.md) - Latest developments in community initiatives
- [Policy Impact Assessment](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/policy_monitoring_analysis.md) - Recent policy changes affecting community tech

## Core Frameworks

### Anti-Capitalist Framework
Our primary tool for identifying AI applications that serve community needs outside capitalist structures.

<pre class="mermaid">
graph LR
    A[Identify Need] --> B[Analyze Power]
    B --> C[Design Solution]
    C --> D[Test Impact]
    style A fill:#f9f,stroke:#333
    style B fill:#bbf,stroke:#333
    style C fill:#bfb,stroke:#333
    style D fill:#fbf,stroke:#333
</pre>

[Learn More](frameworks/#anti-capitalist-ai-applications-framework)

### Capitalist Trap Detector
Systematic approach to identifying when AI solutions inadvertently serve capitalist interests.

<pre class="mermaid">
graph TD
    A[Solution] --> B{Efficiency Trap}
    A --> C{Platform Dependency}
    A --> D{Data Extraction}
    style A fill:#f9f,stroke:#333
</pre>

[Learn More](frameworks/#capitalist-trap-detector-framework)

### Second Order Effects Framework
Strategic analysis of how AI's reduced technical barriers create cascading opportunities for community-controlled alternatives.

<pre class="mermaid">
graph TD
    A[Technical Democratization] --> B[Community Infrastructure]
    C[Economic Barrier Dissolution] --> D[Platform Alternatives]
    E[Knowledge Transfer] --> F[Resistance Tools]
    style A fill:#f9f,stroke:#333
    style C fill:#bbf,stroke:#333
    style E fill:#bfb,stroke:#333
</pre>

[Learn More](frameworks/#second-order-effects-framework)

## Featured Case Studies

### Historical Examples
- [Project Cybersyn](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/project_cybersyn.md) - Chilean economic planning system
- [Zapatista Networks](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/zapatista_networks.md) - Autonomous communication infrastructure
- [Platform Cooperatives](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/platform_coops.md) - Worker-owned digital platforms

### Current Initiatives
- [Mutual Aid Tech](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/mutual_aid_tech.md) - Technology supporting community resilience
- [Community Tech Centers](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/community_tech_centers.md) - Local technology sovereignty
- [Mesh Networks](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/mesh_networks.md) - Community-controlled infrastructure

## Get Involved

- 📱 [Join Our Community](https://github.com/jwynia/myceliary/discussions) - Participate in discussions
- 📬 [Newsletter](https://myceliary.substack.com/) - Regular updates and analysis
- 🤝 [Contribute](https://github.com/jwynia/myceliary) - Help improve our research and tools

## Deep Dive Resources

For comprehensive documentation and detailed analysis:
- [Full Research Archive](https://github.com/jwynia/myceliary/blob/main/context-network/research_tasks/research_tasks_index.md)
- [Complete Framework Documentation](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/frameworks/)
- [Detailed Case Studies](https://github.com/jwynia/myceliary/blob/main/context-network/analysis/findings/case_studies/)
- [Research Methodology](https://github.com/jwynia/myceliary/blob/main/context-network/processes/research.md)
