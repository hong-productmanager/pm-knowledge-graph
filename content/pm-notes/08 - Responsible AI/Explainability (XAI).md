---
tags: [responsible-ai, technical]
type: concept
branch: 08 - Responsible AI
related: ["Transparency to Users", "EU AI Act", "Hallucination"]
created: 2026-05-05
---

# Explainability (XAI)

## Definition
Explainable AI (XAI) refers to the suite of techniques and tools used to make the "Black Box" of machine learning models understandable to humans. The goal is to explain **why** a model reached a specific decision or prediction. XAI is divided into **Global Explainability** (how the whole model works) and **Local Explainability** (why it made this specific choice for this user). Common technical methods include **SHAP** and **LIME** (feature importance scores) and "Attention Maps" for visual models.

## How to Apply It
1. **Define the "Explanation Target"**: Determine who needs the explanation — is it the end-user (simple language) or a compliance auditor (technical data)?
2. **Select an XAI Method**: Work with engineering to implement a method like **Feature Importance** (showing the top 3 reasons for a score) or **Counterfactuals** ("If your income was $10K higher, you would have been approved").
3. **Design the "Reasoning UI"**: Create simple, visual ways to show the explanation to the user (e.g., "Why am I seeing this recommendation?").
4. **Test for "Explanation Clarity"**: Conduct usability testing to ensure that the explanations actually help users make better decisions and don't just add confusion.
5. **Monitor for "Plausible but Wrong" Explanations**: Ensure the XAI system isn't just creating "hallucinated" reasons for a model's behavior that aren't technically true.

## Connected Concepts
- [[08 - Responsible AI/Transparency to Users]] — the UX design of how explanations are presented to the user.
- [[08 - Responsible AI/EU AI Act]] — the legal framework that often mandates explainability for high-risk systems.
- [[03 - AI & ML Fundamentals/Hallucination]] — how explainability can help users identify and "catch" AI hallucinations.
