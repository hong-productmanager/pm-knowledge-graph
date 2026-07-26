---
tags: [prioritization, execution]
type: concept
branch: 05 - Prioritization & Roadmapping
related: ["Product Roadmap", "AI PRD", "Data Pipelines"]
created: 2026-07-26
---

# Dependency Mapping

## Definition
Dependency Mapping is the process of identifying and visualizing the relationships between different tasks, teams, data sources, and technologies within a product project. In AI development, dependencies are often more complex than in standard software, involving **Technical Dependencies** (e.g., Team A must build the API before Team B can use it), **Data Dependencies** (e.g., the pipeline must be active before the model can train), and **External Dependencies** (e.g., waiting for a third-party model provider to grant API access).

## How to Apply It
1. **Host a Cross-functional Sync**: Bring engineering, data science, and infrastructure leads together to brainstorm all the pieces needed for a feature.
2. **Identify the "Critical Path"**: Determine the sequence of tasks that dictates the minimum time needed to complete the project.
3. **Use a Visual Tool**: Map the dependencies in a tool like Lucidchart, Miro, or a simple Gantt chart to show the flow of work.
4. **Explicitly Name Data Dependencies**: For AI, specifically document when training data, annotation pipelines, and evaluation sets will be ready.
5. **Review Dependencies Weekly**: Check in during sprint planning to see if any new dependencies have emerged or if any "upstream" delays will impact the timeline.

## Connected Concepts
- [[05 - Prioritization & Roadmapping/Product Roadmap]] — the high-level plan that dependency mapping makes realistic.
- [[06 - Execution & Delivery/AI PRD]] — the document where dependencies should be explicitly listed during scoping.
- [[04 - Data Strategy/Data Pipelines]] — the primary source of technical dependencies for AI products.
