# MiHucha — Personal Finance PWA with Secure AI

[← Back to profile](../../README.md)

## Overview

**MiHucha** is a mobile-first personal finance application designed to help users understand income, expenses, subscriptions, budgets and savings goals in one place.

The project goes beyond a dashboard prototype: it explores secure AI integration, multi-user cloud synchronization, recoverable data snapshots and resilient offline-first behavior.

## Problem

Personal finance tools often fall into one of two extremes:

- simple spreadsheets with limited automation; or
- complex platforms that require users to surrender a large amount of sensitive financial data.

MiHucha aims for a middle ground: useful automation and intelligent assistance while keeping the user in control of what is imported, stored and analyzed.

## Product capabilities

- Multiple independent financial profiles.
- Fixed and variable expense tracking.
- Annual balance and savings views.
- Budgeting by category.
- CSV and spreadsheet imports processed locally.
- Duplicate detection with explicit user confirmation.
- AI-assisted natural-language entry and financial summaries.
- Installable PWA with temporary offline operation.
- Exportable backups and recoverable cloud snapshots.

## Architecture

```text
React + TypeScript PWA
        │
        ├── Local browser cache for resilience
        ├── Supabase Auth for identity
        ├── PostgreSQL + Row Level Security
        ├── Versioned financial snapshots
        └── Secure server-side AI proxy
                    │
                    └── Google Gemini
```

## Security and privacy decisions

- AI provider keys remain on the server and are never bundled into the browser.
- Every cloud query is constrained by Supabase Row Level Security.
- AI usage is tracked and limited per authenticated user.
- Original bank files are not retained in the cloud after processing.
- Duplicate resolution creates a recovery point before destructive changes.
- Diagnostic exports avoid concepts, notes, credentials and concrete financial values.

## Technologies

`React` · `TypeScript` · `Vite` · `Supabase` · `PostgreSQL` · `RLS` · `Gemini` · `Vercel` · `Vitest` · `PWA`

## What this project demonstrates

- Designing for sensitive personal data.
- Moving an AI integration from client-side experimentation to a protected server-side architecture.
- Combining local-first UX with authenticated synchronization.
- Treating recovery, observability and data integrity as product features.

## Status

Private development project. The public case study intentionally excludes source code, credentials, schemas containing sensitive implementation details and user data.
