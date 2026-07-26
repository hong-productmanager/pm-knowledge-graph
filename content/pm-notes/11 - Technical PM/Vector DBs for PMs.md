---
tags: [technical, data]
type: concept
branch: 11 - Technical PM
related: ["Embeddings & Vector Databases", "RAG (Retrieval Augmented Generation)", "Data Pipelines"]
created: 2026-07-26
---

# Vector DBs for PMs

## Definition
Vector Databases (Vector DBs) are specialized data storage systems that allow for "Semantic Search." Instead of searching for exact words (keyword search), they search for "meaning" by representing data as high-dimensional vectors. For a PM, a Vector DB is the "Long-term Memory" of an AI system. It is where you store your company's documents, user data, and product information so they can be retrieved and provided as context to an LLM via a **RAG (Retrieval Augmented Generation)** architecture.

## How to Apply It
1. **Choose Between "Pure" vs. "Hybrid"**: Decide if you need a dedicated vector database (like Pinecone) or an extension to your existing DB (like pgvector for Postgres).
2. **Define the Embedding Strategy**: Select a model that will turn your text or images into vectors, ensuring it matches the language and domain of your users.
3. **Determine Chunking and Metadata**: Decide how to break up your documents and what "filters" (like date, user_id, or category) you need to store alongside the vectors.
4. **Monitor Retrieval Relevance**: Track "Recall at K" — how often the correct document is among the top few results returned by the database.
5. **Manage Cost and Latency**: As the database grows, work with engineering to implement "Approximate Nearest Neighbor" (ANN) indexing to keep the search fast and cheap.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Embeddings & Vector Databases]] — the technical foundation of this technology.
- [[03 - AI & ML Fundamentals/RAG (Retrieval Augmented Generation)]] — the primary use case for Vector DBs in the product.
- [[04 - Data Strategy/Data Pipelines]] — the systems needed to keep the Vector DB updated with fresh data.
