---
tags: [ai, technical]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["Hallucination", "Embeddings & Vector Databases", "Data Pipelines"]
created: 2026-07-26
---

# RAG (Retrieval Augmented Generation)

## Definition
Retrieval Augmented Generation (RAG) is an architecture that combines the reasoning capabilities of a Large Language Model with the accuracy of a retrieval system. It works by first "retrieving" relevant documents or data from an external source (like a vector database) and then providing that context to the LLM to "generate" an answer. This allows the model to answer questions about proprietary data or current events that were not included in its original training set, significantly reducing hallucinations and improving factual accuracy.

## How to Apply It
1. **Identify the Data Source**: Determine which proprietary documents or databases contain the "ground truth" the AI needs.
2. **Develop a Chunking Strategy**: Break large documents into smaller, semantically meaningful "chunks" that can be easily retrieved.
3. **Select a Retriever**: Choose an embedding model and a vector database that can quickly find the most relevant chunks based on a user's query.
4. **Draft the "System Prompt"**: Instruct the LLM to *only* use the provided context to answer the question and to cite its sources.
5. **Monitor and Tune**: Track retrieval quality (did we find the right docs?) separately from generation quality (did the LLM summarize them correctly?).

## Connected Concepts
- [[03 - AI & ML Fundamentals/Hallucination]] — the primary problem that RAG is designed to solve.
- [[03 - AI & ML Fundamentals/Embeddings & Vector Databases]] — the technical infrastructure that makes RAG retrieval possible.
- [[04 - Data Strategy/Data Pipelines]] — the systems required to keep the RAG database up-to-date.
