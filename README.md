# PM Knowledge Graph

A personal product management digital garden — concepts, frameworks, and applied notes across 14 domains, published with [Quartz](https://quartz.jzhao.xyz/) and Obsidian.

🔗 Live site: https://hong-productmanager.github.io/pm-knowledge-graph

## Structure

All content lives in `content/pm-notes/`, organized into 14 numbered domains (Strategy & Vision, Research & Discovery, AI & ML Fundamentals, Data Strategy, Prioritization & Roadmapping, Execution & Delivery, Metrics & Analytics, Responsible AI, AI UX Patterns, GTM & Growth, Technical PM, Leadership & Stakeholders, Frameworks & Models, Tools & Artifacts). Each domain has a MOC (Map of Content) index linking to its notes. Every note follows the same template:

```
---
tags: []
type: concept
branch: <domain name>
related: []
created: <date>
---

# Title
## Definition
## How to Apply It
## Connected Concepts
```

Open `content/` as an Obsidian vault to edit notes with full wiki-link/graph support. Run `npx quartz build --serve` to preview the site locally.

## Using This With Claude Code

This vault is written in Claude Code and designed to be used by it, not just published as a static site. A few ways to put it to work:

**As grounding context for PM work in any project.** Point Claude Code at `content/pm-notes/` (or paste a specific note) when scoping a feature, writing a PRD, or making a prioritization call, so its suggestions are grounded in your own definitions and applied notes instead of generic training knowledge. This matters most for the notes you've personalized with real project outcomes rather than the generic definitions alone.

**As source material for custom Claude Code skills.** Individual notes — especially in `13 - Frameworks & Models` and `14 - Tools & Artifacts` — map directly onto reusable slash-command skills:
- `RICE Prioritization.md` → a `/prioritize` skill that walks through Reach/Impact/Confidence/Effort scoring for a real backlog
- `PRD Template.md` → a `/write-prd` skill that drafts a PRD from a one-line problem statement using this exact structure
- `Bias & Fairness.md` + `EU AI Act.md` → an `/ai-risk-check` skill that audits a described AI feature against this vault's Responsible AI notes

Claude Code's `skill-creator` skill can scaffold any of these from a note's content directly — the note becomes the skill's instructions, kept in sync as you refine it here.

**As a portable reference across projects.** Since it's a plain Git repo, clone or reference specific notes from any other project's `CLAUDE.md` to carry the same PM vocabulary and frameworks across your work, rather than re-explaining them per project.
