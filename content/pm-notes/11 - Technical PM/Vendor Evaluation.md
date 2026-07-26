---
tags: [technical, strategy]
type: concept
branch: 11 - Technical PM
related: ["Build vs Buy vs Fine-tune", "Model Selection Criteria", 
          "LLM Architecture for PMs"]
created: 2026-05-06
---

# Vendor Evaluation

## Definition
Vendor Evaluation is the structured process by which a Product Manager assesses third-party AI/ML providers, API platforms, and tooling vendors before committing to a build or integration decision. It covers technical capability, pricing model, reliability guarantees, data privacy terms, and strategic lock-in risk.

## How to Apply It
1. **Define Evaluation Criteria**: Score vendors on: accuracy on your task, latency (P50/P99), cost per inference, data privacy terms, uptime SLA, and deprecation policy.
2. **Run a Bake-off**: Test 2-3 vendors on your actual production data sample — not vendor benchmarks.
3. **Model the Cost Curve**: Project cost at 10x current volume; many vendors look cheap at low scale but become the largest COGS line at growth.
4. **Audit the Contract**: Check model deprecation clauses, data retention policies, and whether your input data is used for training.
5. **Assess Switching Cost**: Before signing, prototype what a migration to an alternative would take — this gives you genuine negotiating leverage.

## Connected Concepts
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — the strategic decision this evaluation informs
- [[11 - Technical PM/Model Selection Criteria]] — technical criteria for evaluating model performance
- [[10 - GTM & Growth/Cost-to-Serve]] — how vendor cost feeds into unit economics
