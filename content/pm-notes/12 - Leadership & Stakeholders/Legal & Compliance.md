---
tags: [leadership, compliance]
type: concept
branch: 12 - Leadership & Stakeholders
related: ["Privacy & Compliance", "EU AI Act", "Responsible AI"]
created: 2026-05-05
---

# Legal & Compliance

## Definition
Legal & Compliance for PMs refers to the partnership with the legal team to ensure the product meets all regulatory, contractual, and ethical obligations. In AI, this is exceptionally complex, involving **Intellectual Property** (who owns the AI's output?), **Data Privacy** (GDPR/CCPA), **Liability** (who is responsible if the AI fails?), and **Ethics** (avoiding bias and harmful content). The PM's role is to ensure these "constraints" are built into the product architecture rather than being added as an afterthought.

## How to Apply It
1. **Engage Legal "Early and Often"**: Don't wait until the day before launch to show the legal team your AI feature; bring them into the PRD phase.
2. **Map Your "Data Rights"**: Clearly document where every piece of training data came from and confirm that your "Terms of Service" allow for model training.
3. **Build for "Auditability"**: Ensure the system keeps logs of AI decisions and data usage so you can provide "proof of compliance" to regulators.
4. **Implement "Terms of Use" Prompts**: Work with legal to design UI patterns that clearly explain the AI's limitations and the user's responsibilities.
5. **Establish a "Risk Threshold"**: Agree with legal on what constitutes an "acceptable" level of risk for a specific AI feature (e.g., a "creative" bot has more leeway than a "medical" bot).

## Connected Concepts
- [[04 - Data Strategy/Privacy & Compliance]] — the technical side of the legal partnership.
- [[08 - Responsible AI/EU AI Act]] — the primary upcoming legal framework for AI products.
- [[08 - Responsible AI/Responsible AI MOC|Responsible AI]] — the ethical dimension that often goes beyond strict legal requirements.
