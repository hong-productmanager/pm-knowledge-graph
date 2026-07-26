---
tags: [data, compliance]
type: concept
branch: 04 - Data Strategy
related: ["Data Quality", "EU AI Act", "Transparency to Users"]
created: 2026-05-05
---

# Privacy & Compliance

## Definition
Privacy & Compliance in AI refers to the legal and ethical frameworks that govern how user data is collected, stored, and used to train machine learning models. Key regulations include **GDPR** (EU), **CCPA** (California), and sector-specific rules like **HIPAA** (Healthcare). A major challenge for AI products is the "Right to Erasure" (the right to be forgotten), which complicates the use of user data in training sets that cannot easily be "unlearned" by a model once it has been trained.

## How to Apply It
1. **Implement Privacy by Design**: Build data minimization and anonymization into the product from the very first architectural diagram.
2. **Get Explicit Consent**: Clearly explain to users how their data will be used (e.g., "to improve the model") and give them a simple "opt-out" mechanism.
3. **Manage PII (Personally Identifiable Information)**: Use "PII Redaction" tools to strip names, emails, and addresses from data before it enters the training pipeline.
4. **Plan for the "Right to Erasure"**: Develop a strategy for how to handle user deletion requests, whether through "Machine Unlearning" or periodic retraining without deleted cohorts.
5. **Audit Third-Party Vendors**: Ensure that any AI APIs you use (like OpenAI or Anthropic) have "Zero Data Retention" (ZDR) policies for your sensitive user data.

## Connected Concepts
- [[04 - Data Strategy/Data Quality]] — ensuring that privacy-compliant data is still accurate and useful for training.
- [[08 - Responsible AI/EU AI Act]] — the emerging legal framework for AI safety and transparency in Europe.
- [[08 - Responsible AI/Transparency to Users]] — the UX requirement to be honest about data usage.
