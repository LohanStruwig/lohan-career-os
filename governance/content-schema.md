---
title: Content Schema
category: Governance
visibility: public
resume_relevance: medium
portfolio_relevance: high
last_updated: 2026-06-21
---

# Content Schema

Most Markdown files in this repository use a small front matter block so they can later be parsed into a portfolio website, case-study system, executive profile builder, or content API.

## Standard Fields

```yaml
title: Human-readable page or block title
category: Master CV | Experience | Capability Block | Skills | Project | Evidence Ledger | Resume Blocks | Portfolio Content | Role Targeting | Governance
visibility: public
resume_relevance: low | medium | high
portfolio_relevance: low | medium | high
last_updated: YYYY-MM-DD
```

## Future Website Use

The front matter can power:

- portfolio cards
- capability pages
- case-study routing
- executive profile snippet selection
- role-family pages
- searchable career evidence
- portfolio publication status

## Rule

Use `visibility` to distinguish polished portfolio material from working notes if future content states are added.
