---
tags: [prioritization, framework]
type: framework
branch: 05 - Prioritization & Roadmapping
related: ["Product Roadmap", "Trade-off Frameworks", "RICE Prioritization"]
created: 2026-07-26
---

# MoSCoW

## Definition
MoSCoW, developed by Dai Clegg in 1994 as part of the Dynamic Systems Development Method (DSDM), is a prioritization technique used in management, business analysis, and software development to reach a common understanding with stakeholders on the importance they place on the delivery of each requirement. The acronym stands for: **Must have** (critical for launch), **Should have** (important but can be deferred), **Could have** (desirable but not necessary), and **Won't have (this time)** (deliberately excluded from the current release). It is particularly effective for managing scope and preventing "feature creep" during a development cycle.

## How to Apply It
1. **List All Requirements**: Gather all the potential features, bugs, and tasks for the next release or sprint.
2. **Categorize by Criticality**:
    - **Must**: If this isn't included, the product is a failure or legally non-compliant.
    - **Should**: Important features that add significant value but aren't vital for day one.
    - **Could**: Small improvements or "delighters" that can be cut if time runs out.
    - **Won't**: Ideas that the team has agreed are out of scope for this specific cycle.
3. **Review with Stakeholders**: Get buy-in from engineering, design, and business owners on the categorization.
4. **Enforce the "Won't" List**: Use the list as a defensive tool during the build phase to prevent new requests from derailing the timeline.
5. **Re-evaluate Every Cycle**: Move items between categories as the project progresses and new information becomes available.

## Connected Concepts
- [[05 - Prioritization & Roadmapping/Product Roadmap]] — the high-level plan that MoSCoW helps detail.
- [[05 - Prioritization & Roadmapping/Trade-off Frameworks]] — the logic used to decide which category a feature falls into.
- [[13 - Frameworks & Models/RICE Prioritization]] — a more quantitative scoring method that can be used alongside MoSCoW.
