---
title: Public Review Checklist
category: Documentation
visibility: public
resume_relevance: medium
portfolio_relevance: high
last_updated: 2026-06-22
---

# Public Review Checklist

Use this checklist before sharing the repository more widely, linking new files from the README, adding visuals, or publishing material into a website, proposal, or public profile.

The review should stay lightweight and manual unless a later pass explicitly scopes tooling. The goal is to preserve a professional public proof layer without exposing private material or turning partial evidence into unsupported claims.

## Review Cadence

Recommended cadence:

- quarterly public-safety review;
- before adding any new README-linked file;
- before adding screenshots, diagrams, or visual proof;
- before using repository material in a public website, proposal, or profile update.

## Link And Navigation Check

- Confirm README links resolve.
- Confirm newly linked files are intended for public reading.
- Confirm reader paths still start with curated files before deeper source folders.
- Confirm external links are still accurate and intentional.

## Public-Safety Scan

Check for:

- credentials, deployment secrets, `.env` values, tokens, or private keys;
- private customer, employer, partner, or contact data;
- street addresses, phone numbers, identity documents, or sensitive personal identifiers;
- compensation, tax, medical, legal, insurance, or role-application materials;
- raw exports, private datasets, unreviewed research files, or internal screenshots;
- non-public dashboards, analytics, admin panels, or system access views.

## Claim And Evidence Check

- Keep claims grounded in reviewed source material, public-safe summaries, or clearly framed professional context.
- Do not invent missing proof.
- Do not imply unavailable artifacts have been reviewed.
- Avoid precise metrics or counts unless they are already reviewed and intentionally public.
- Keep evidence-basis language visible on case studies.
- Prefer responsible summaries over stronger claims that cannot be supported.

## Wording Check

Prefer restrained public language:

- selected proof;
- public-safe summaries;
- governed workflow;
- structured market and account research;
- evidence basis;
- operating patterns;
- curated credibility layer.

Avoid wording that sounds private, automated, or overly internal:

- non-public research profiles;
- unreviewed company intelligence;
- confidential evidence;
- unreviewed archives;
- automated role-application system;
- unsupported performance claims.

## Visual And Screenshot Check

Before adding an image, screenshot, diagram, or visual:

- read [Public Visual Proof Guidelines](public-visual-proof-guidelines.md);
- confirm no private names, emails, accounts, analytics, credentials, or internal dashboards are visible;
- prefer public website screenshots, sanitized diagrams, or purpose-built public visuals;
- confirm the visual supports the narrative rather than compensating for missing proof.

## Release And Issue Hygiene

- Use small PRs for public-facing changes where practical.
- Link PRs to issues when the work closes a defined improvement.
- Keep issue wording public-safe and professional.
- Use releases only for meaningful public milestones.
- Keep the repo clean after merge by deleting merged branches and syncing local `main`.

## Review Outcome

After review, decide one of:

- Ready for public linking.
- Ready after minor wording cleanup.
- Keep as reviewed source material, not public navigation.
- Keep private or omit from the public proof layer.
