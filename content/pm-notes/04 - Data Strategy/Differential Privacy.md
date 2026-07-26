---
tags: [data, privacy]
type: concept
branch: 04 - Data Strategy
related: ["Privacy & Compliance", "Data Collection & Labeling", "Responsible AI"]
created: 2026-07-26
---

# Differential Privacy

## Definition
Differential Privacy is a mathematical framework for sharing information about a dataset by describing the patterns of groups within the dataset while withholding information about individuals in the dataset. It works by adding "calibrated noise" to the data before it is analyzed or used for training. This ensures that even if an attacker has access to the model or the aggregate data, they cannot determine whether any specific individual was included in the original dataset. The key parameter is **Epsilon** (the "privacy budget"), which controls the trade-off between privacy and accuracy.

## How to Apply It
1. **Identify High-Risk Data**: Determine which datasets contain information that could harm users if it were ever leaked or re-identified.
2. **Set the Privacy Budget (Epsilon)**: Work with data scientists to find the "Sweet Spot" where the added noise protects users without destroying the model's utility.
3. **Implement Noise at the Source**: Add the noise during the data collection or aggregation phase, rather than trying to "anonymize" the data after it is stored.
4. **Monitor the "Budget Spend"**: Track how much privacy budget is being used by different queries or training runs to ensure the overall dataset doesn't become vulnerable over time.
5. **Communicate the Benefit**: Use the fact that you use differential privacy in your marketing to build trust with privacy-conscious users and enterprise buyers.

## Connected Concepts
- [[04 - Data Strategy/Privacy & Compliance]] — the broader legal and ethical context for using differential privacy.
- [[04 - Data Strategy/Data Collection & Labeling]] — how differential privacy can be integrated into the data gathering process.
- [[08 - Responsible AI/Bias & Fairness]] — ensuring that the added noise doesn't disproportionately degrade performance for certain user groups.
