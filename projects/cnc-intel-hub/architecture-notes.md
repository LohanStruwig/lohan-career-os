---
title: CNC Intel Hub Architecture Notes
category: Project
visibility: public
resume_relevance: medium
portfolio_relevance: high
last_updated: 2026-06-21
---

# CNC Intel Hub Architecture Notes

## Portfolio-Level Architecture

This file keeps the architecture discussion at product and workflow level. CNC Intel Hub should be understood as a vertical SaaS-style account-intelligence workspace, not a simple public website.

## Conceptual Components

- public landing and request/contact surface
- protected workspace access screens
- workspace selector and approved-access state handling
- private account-intelligence explorer
- company cards and focused detail panels
- search, filters, Data Stream shortcuts, and Review Priority shortcuts
- saved filters scoped by workspace and available user identity
- evidence-backed company context
- account-intelligence signals: Evidence Score, VMC/customer fit, dealer Channel Fit, CNC/Automation relevance, confidence, caveats, validation status, and review priority
- browser-generated PDF account packets with export caps
- Vercel-compatible contact/request API with validation, honeypot, rate limiting, and Cloudflare Turnstile-ready verification
- Supabase auth/session handling and authorized workspace loading
- planned workspace membership, workspace-scoped data model, and RLS policy design
- Python research, scoring, diagnostics, workbook/feed, import preview, and territory planning tooling
- PowerShell validation and guarded SQL execution wrappers
- SQL/import governance with preflight, row-count, workspace-targeting, RLS, and apply-confirmation checks
- data governance and QA review
- GitHub PR, Vercel preview, production smoke, browser, protected-access, PDF export, saved-filter, and console-error QA workflow

## Technical Fluency Represented

- React
- TypeScript
- Vite
- CSS
- lucide-react
- Supabase
- Vercel
- GitHub
- pdf-lib
- Python
- PowerShell
- PostgreSQL
- Cloudflare Turnstile-ready verification
- SQL governance
- AI-assisted implementation support
- human approval gates
