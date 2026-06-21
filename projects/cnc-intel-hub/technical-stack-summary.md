---
title: CNC Intel Hub Technical Stack Summary
category: Project
visibility: public
resume_relevance: high
portfolio_relevance: high
last_updated: 2026-06-21
---

# CNC Intel Hub Technical Stack Summary

CNC Intel Hub should be understood as a vertical SaaS-style account-intelligence workspace for CNC/VMC market intelligence, not as a simple marketing website or static application.

The public landing page is only one surface. The more important product work is the private workspace model: approved-access account intelligence, structured company review, market-fit signals, saved filters, exportable account packets, research tooling, data governance, and release discipline.

## Product Architecture

CNC Intel Hub is designed to help approved client teams review territories, dealers, customers, potential customers, and potential dealer candidates in a structured workspace.

The product is not positioned as a CRM or CMS. It focuses on account intelligence:

- filtering company records
- reviewing company cards and detail panels
- checking evidence and fit signals
- understanding Evidence Score, VMC/customer fit, dealer Channel Fit, CNC/Automation relevance, caveats, validation status, confidence, and review priority
- saving useful views
- exporting PDF account packets for internal planning and handoff

## Frontend Application

The online application is built as a Vite React application using:

- React
- TypeScript
- Vite
- CSS
- lucide-react icons

The frontend includes:

- public landing page
- protected workspace request/contact page
- workspace login/access screens
- workspace selector
- private workspace explorer interface
- company cards
- focused detail panels
- filters and search
- Data Stream shortcuts
- Review Priority shortcuts
- saved filters
- PDF export controls
- local URL/session state
- protected workspace access states

## Backend And Contact API

The app includes a Vercel-compatible serverless API route for contact/request submissions.

The API is designed around:

- input validation
- honeypot bot protection
- basic rate limiting
- Cloudflare Turnstile-ready verification
- server-side delivery through configured methods
- fail-closed behavior when verification or delivery is not configured

The contact flow avoids exposing a public email address or mailto link while still giving prospective customers a way to request a custom workspace.

## Supabase And Workspace-Scoped Data Planning

Supabase is part of the planned and partially integrated architecture for authentication, workspace membership, and workspace-scoped data access.

The app uses the Supabase JavaScript client for:

- auth/session handling
- authorized workspace loading
- workspace data loading when a signed-in user has approved access

The intended data model includes tables such as:

- workspaces
- workspace_members
- import_batches
- metro_feed
- company_cards
- company_details

The security model is planned around `workspace_id`, membership checks, and Row Level Security policy design so real client rows can be scoped to approved workspaces.

## PDF Export System

CNC Intel Hub uses `pdf-lib` for browser-generated PDF exports.

The export flow supports professional A4 account packets with:

- cover page
- one company page per company
- workspace/report summary
- company name and location
- Data Stream
- Evidence Score
- VMC/customer fit or Channel Fit
- CNC/Automation relevance
- overview/profile/fit/validation/evidence sections
- website evidence

Exports are capped to prevent oversized output and to keep reports practical for real planning workflows.

## Saved Filters

Saved filters are currently browser/local-storage based and scoped by workspace and, when available, signed-in user identity.

Saved filter behavior includes:

- save current filters
- select a saved filter
- search saved filters
- update an existing saved filter
- delete saved filters
- download a PDF from the current filtered view

Supabase-backed saved filters are a planned improvement that requires migration and RLS planning before implementation.

## Research, Data, And Import Tooling

Python is used heavily for local data preparation, research automation, scoring, import previews, diagnostics, and workbook/feed preparation.

The tooling supports:

- inspecting source files
- extracting product intelligence
- building master workbooks
- preparing research batches
- running research review flows
- building dashboard-ready outputs
- creating territory planning packs
- applying scoring refinements
- preparing Supabase import packages
- building import previews
- running company intelligence scoring dry runs

PowerShell supports local workflow automation and guarded SQL execution wrappers, including validation commands, SQL package preflight scripts, and controlled connection handling when explicitly approved.

## SQL And Import Governance

SQL and import workflows are treated as high-governance areas.

The product work includes planning and tooling for:

- SQL package preflight
- SQL apply validation
- import package review
- expected row-count checks
- workspace targeting checks
- RLS safety checks
- import batch governance
- generated SQL kept under ignored outputs
- explicit confirmation before live database writes

## Hosting, Release, And QA Workflow

CNC Intel Hub uses:

- GitHub for source control and pull requests
- Vercel for preview and production deployments
- preview URLs for QA before merge
- production smoke QA after merge

The QA and release workflow includes:

- local build checks
- `git diff --check`
- GitHub PR review
- Vercel preview QA
- browser testing
- console error checks
- protected-data access checks
- anonymous logout/deep-link safety checks
- PDF export behavior checks
- saved filter behavior checks
- production smoke QA

## AI-Assisted Development Workflow

ChatGPT and Codex support the development workflow for planning, implementation briefs, frontend features, file review, local checks, PR summaries, merge-readiness reviews, preview QA, production smoke QA, project summaries, and handoff notes.

The AI workflow is governed by explicit product scope, data safety, git, deployment, SQL, and approval rules.

## Portfolio Summary

CNC Intel Hub combines frontend engineering, protected workspace access, account-intelligence data modeling, scoring logic, PDF reporting, research automation, Supabase workspace planning, Vercel deployment, GitHub PR workflow, and governed AI-assisted development.

The business goal is to help CNC/VMC sales and leadership teams review the right accounts faster, understand why each company matters, validate evidence before action, and produce clean internal handoff materials without turning the product into an overly complex CRM.
