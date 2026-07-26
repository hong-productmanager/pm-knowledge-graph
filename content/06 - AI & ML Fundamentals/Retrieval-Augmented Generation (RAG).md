---
tags: [ai, ml, rag]
type: concept
branch: AI & ML Fundamentals
related: []
created: 2026-07-26
---

# Retrieval-Augmented Generation (RAG)

## Definition
RAG is a pattern where an LLM's response is grounded by first retrieving relevant documents or data (typically via vector similarity search) and inserting them into the prompt context, rather than relying purely on what the model memorized during training. It's the standard way to get an LLM to answer accurately about private, current, or domain-specific data.

## Why It Matters for PMs
RAG changes what's feasible to scope: instead of fine-tuning a model (expensive, slow to update) to "know" your company's data, you can often stand up a retrieval pipeline much faster. PMs scoping AI features need to know RAG's failure modes too — retrieval can miss the right document, or the model can still hallucinate on top of correct retrieved context — so "we used RAG" doesn't automatically mean "the answer is accurate."

## How I've Applied It
*(Placeholder — replace with a real example: a feature you scoped or evaluated that used RAG, and a tradeoff you had to navigate.)*

## Real-World Example
*(Placeholder — replace with a real example of a RAG-based product or feature you've used or researched.)*

## Connected Concepts
- [[Data Moats]]
- [[Model Bias & Fairness]]
