---
tags: [ai, technical]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["Build vs Buy vs Fine-tune", "Cost Metrics", "AI Metrics"]
created: 2026-05-05
---

# Inference & Latency

## Definition
**Inference** is the process of a trained model making a real-time prediction or generation based on new input. **Latency** is the time it takes for that process to complete and return a result to the user. In AI products, latency is often the primary bottleneck for user experience. Key factors influencing latency include model size (parameters), hardware (GPU/CPU), quantization (compressing the model), and batching. For PMs, managing the "Latency Budget" is a critical architectural decision that often requires trading off accuracy for speed.

## How to Apply It
1. **Set a Latency SLA**: Define the maximum acceptable time for each user action (e.g., "Search results must appear in <500ms").
2. **Benchmark Different Models**: Test the trade-off between a "Large" model (higher accuracy, higher latency) and a "Small" model (lower accuracy, lower latency).
3. **Implement "Streaming"**: For LLMs, show the output token-by-token so the user *perceives* the system as fast even if the total generation takes several seconds.
4. **Optimize the Stack**: Work with engineering to explore techniques like **Quantization** (reducing precision to gain speed) or using specialized inference engines (like vLLM).
5. **Monitor Latency at P99**: Look beyond the "Average" latency to see the "Worst-case" (99th percentile) experience, which is often where users actually churn.

## Connected Concepts
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — how latency influences the decision to build your own model vs. use an API.
- [[07 - Metrics & Analytics/Cost Metrics]] — the direct relationship between inference speed and infrastructure cost.
- [[07 - Metrics & Analytics/AI Metrics]] — tracking how latency affects product-level success metrics like activation and retention.
