---
tags: [responsible-ai, compliance]
type: concept
branch: 08 - Responsible AI
related: ["Privacy & Compliance", "Transparency to Users", "Explainability (XAI)"]
created: 2026-05-05
---

# EU AI Act

## Definition
The EU AI Act is the world's first comprehensive legal framework for artificial intelligence, designed to ensure that AI systems used in the EU are safe, transparent, and under human control. It follows a **Risk-based Approach**, categorizing AI systems into four levels: **Unacceptable Risk** (banned), **High Risk** (strictly regulated), **Limited Risk** (transparency obligations), and **Minimal Risk** (no regulation). For PMs, "High Risk" systems (e.g., critical infrastructure, education, employment) face the most intense requirements, including mandatory conformity assessments and human oversight.

## How to Apply It
1. **Classify Your System's Risk**: Determine if your AI falls into the "High Risk" category (e.g., hiring tools, credit scoring, or critical infrastructure).
2. **Implement Data Governance**: Ensure your training and testing data meets the high standards for quality and bias mitigation required by the Act.
3. **Build for Transparency**: Develop "Instructions for Use" and UI patterns that help users understand the system's purpose and limitations.
4. **Ensure Human Oversight**: Design the product so that a human can intervene, override, or shut down the AI system at any time.
5. **Establish a Compliance Registry**: Maintain detailed technical documentation and "logs" of system performance and incidents as required for High-Risk systems.

## Connected Concepts
- [[04 - Data Strategy/Privacy & Compliance]] — the broader regulatory landscape for user data.
- [[08 - Responsible AI/Transparency to Users]] — the specific UX requirements mandated by the "Limited Risk" and "High Risk" tiers.
- [[08 - Responsible AI/Explainability (XAI)]] — the technical capability required to fulfill the Act's transparency mandates.
