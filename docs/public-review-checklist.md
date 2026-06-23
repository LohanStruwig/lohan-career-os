---
title: Public Review Checklist
category: Documentation
visibility: public
resume_relevance: medium
portfolio_relevance: high
last_updated: 2026-06-23
---

# Public Review Checklist

Use this checklist before sharing the repository more widely, linking new files from the README, adding visuals, or publishing material into a website, proposal, or public profile.

The review should stay lightweight and manual unless a later pass explicitly scopes tooling. The goal is to preserve a professional public proof layer without exposing private material or turning partial evidence into unsupported claims.

Removing a link is not enough. Any file that remains in a public repository must be safe for direct URL access, GitHub search, clone, and indexing.

## Review Cadence

Recommended cadence:

- quarterly public-safety review;
- before adding any new README-linked file;
- before adding screenshots, diagrams, or visual proof;
- before using repository material in a public website, proposal, or profile update.

## Link And Navigation Check

- Confirm README links resolve.
- Confirm newly linked files are intended for public reading.
- Confirm reader paths only point to curated public files.
- Confirm external links are still accurate and intentional.
- Confirm no deeper source folder remains in the public tree unless every file has been sanitized to public standard.

## Public-Safety Scan

Check for:

- credentials, deployment secrets, `.env` values, tokens, or private keys;
- local machine paths, usernames, prompts, handoff notes, branch names, or workflow details that reveal private process;
- private customer, employer, partner, or contact data;
- street addresses, phone numbers, identity documents, or sensitive personal identifiers;
- exact locality beyond the intentionally public regional location;
- compensation, tax, medical, legal, insurance, or role-application materials;
- raw exports, private datasets, unreviewed research files, or internal screenshots;
- non-public dashboards, analytics, admin panels, or system access views.
- table names, data models, security-control status, implementation architecture, rate-limit/bot-check details, access-control internals, or QA probe details.

## Claim And Evidence Check

- Keep claims grounded in reviewed source material, public-safe summaries, or clearly framed professional context.
- Do not invent missing proof.
- Do not imply unavailable artifacts have been reviewed.
- Avoid precise metrics or counts unless they are already reviewed and intentionally public.
- Avoid precise delivery claims unless they remain useful, supportable, and intentionally public.
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
- planned or partially integrated controls;
- implementation-level architecture.

## GitHub Surface Check

Also review non-file GitHub surfaces:

- repo descriptions and topics;
- pinned repositories;
- branch names;
- release titles and descriptions;
- issue and pull request titles, descriptions, and comments;
- Actions logs and artifacts;
- Pages, Packages, Deployments, and environment names.

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
