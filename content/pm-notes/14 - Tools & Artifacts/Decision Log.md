---
tags: [artifact, process]
type: artifact
branch: 14 - Tools & Artifacts
related: ["AI PRD", "Trade-off Frameworks", "Stakeholder Communication"]
created: 2026-07-26
---

# Decision Log

## Definition
A Decision Log (also known as an ADR — Architecture Decision Record) is a living document that captures the "Why" behind product and technical decisions, not just the "What" was decided. It is a historical record that includes: **Date**, **Decision Made**, **Context at the time**, **Options considered**, **Rationale chosen**, **Trade-offs accepted**, and **Stakeholders involved**. The goal is to provide a permanent "Institutional Memory" that prevents teams from relitigating the same debates every few months.

## How to Apply It
A standard Decision Log entry should be short (1 page max) and include:
1. **Title**: The specific decision (e.g., "Switching to RAG for Docs").
2. **Status**: Proposed, Accepted, or Superseded.
3. **Context**: What was the problem? What were the constraints (budget, time, accuracy)?
4. **Options**: List at least two alternatives (e.g., "Fine-tuning" vs. "RAG").
5. **Rationale**: Why did you pick the winner? (e.g., "RAG is 10x cheaper and easier to update").
6. **Consequences**: What did we give up? (e.g., "Higher latency for the first query").

## Connected Concepts
- [[06 - Execution & Delivery/AI PRD]] — the document that often triggers a decision log entry.
- [[05 - Prioritization & Roadmapping/Trade-off Frameworks]] — the mental tools used to reach the decisions in the log.
- [[12 - Leadership & Stakeholders/Stakeholder Communication]] — the process of sharing the "Why" with the broader organization.
