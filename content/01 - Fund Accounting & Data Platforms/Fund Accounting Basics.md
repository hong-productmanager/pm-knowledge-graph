---
tags: [fund-accounting, data-platforms, example]
type: concept
branch: Fund Accounting & Data Platforms
related: []
created: 2026-07-26
---

# Fund Accounting Basics

## Definition
Fund accounting is a system for tracking assets, liabilities, and cash flows on a per-fund basis rather than a single consolidated ledger. Each fund is treated as its own accounting entity, which lets a firm (e.g., an asset manager or fintech platform) report performance, fees, and positions independently for every fund it administers.

## Why It Matters for PMs
Any product touching NAV calculation, investor statements, or reconciliation workflows inherits the constraints of the fund accounting system underneath it. PMs need to understand the data model (funds, share classes, ledgers, positions) well enough to scope features accurately, spot when a "simple" UI request actually requires a non-trivial accounting change, and speak credibly with accounting/ops stakeholders.

## How I've Applied It
*(Placeholder — replace with a real example: e.g., "Scoped a NAV-per-share reporting feature by first mapping how the fund accounting engine calculates daily NAV, which surfaced an edge case with same-day subscriptions/redemptions.")*

## Real-World Example
*(Placeholder — replace with a real example from your work, e.g. a specific reconciliation bug, a data platform migration, or a vendor integration.)*

## Connected Concepts
- [[Stakeholder Mapping]]
- [[Payment Rails Overview]]
