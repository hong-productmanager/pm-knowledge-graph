---
tags: [artifact, safety]
type: artifact
branch: 14 - Tools & Artifacts
related: ["AI Safety & Guardrails", "Model Card", "Hallucination"]
created: 2026-05-05
---

# Red Team Report

## Definition
A Red Team Report is a technical document that summarizes the results of "Adversarial Testing" on an AI system. "Red Teaming" involves a group of security researchers or developers (the "Red Team") attempting to "break" the AI by finding jailbreaks, prompt injections, data extraction vulnerabilities, or bias elicitation paths. The report documents: **Attack Types tested**, **Success Rate per attack**, **Severity of successful exploits**, **Mitigations applied**, and **Residual Risk accepted**.

## How to Apply It
1. **Scope the Attacks**: Determine what "Harm" you are testing for (e.g., "Medical advice," "Hate speech," "PII extraction").
2. **Run the Attacks**: Use a mix of "Automated Red Teaming" (using other LLMs to attack yours) and "Manual Red Teaming" (expert human hackers).
3. **Analyze & Mitigate**: For every successful exploit, the engineering team must either "Fix" the model weights or add a "Guardrail" filter.
4. **Final Sign-off**: The PM and the Safety Lead must review the "Residual Risk" (the attacks that still work) and decide if it’s "Safe enough" to launch.

## Connected Concepts
- [[08 - Responsible AI/AI Safety & Guardrails]] — the technical defenses that the red team report aims to test.
- [[14 - Tools & Artifacts/Model Card]] — the high-level summary where the results of the red team are often referenced.
- [[03 - AI & ML Fundamentals/Hallucination]] — one of the many failure modes that a red team attempts to trigger.
