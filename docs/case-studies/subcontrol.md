# SubControl — Subscription Management and Savings Simulator

[← Back to profile](../../README.md)

## Overview

**SubControl** is an installable personal-finance PWA focused on recurring expenses. It helps users understand the real monthly and annual impact of subscriptions, simulate cancellations and identify potential savings.

## Problem

Small recurring charges are easy to ignore individually but can become a significant annual expense. Existing banking views show transactions, yet often fail to answer practical questions such as:

- What do I spend every month on subscriptions?
- Which services are the most expensive?
- How much would I save by cancelling one or more services?
- Which expenses appear redundant or non-essential?

## Product capabilities

- Subscription CRUD and categorization.
- Monthly and annual cost projections.
- Interactive charts and spending rankings.
- Non-destructive cancellation simulations.
- Monthly spending targets.
- Multi-currency formatting.
- Local browser persistence.
- Installable offline-capable PWA.
- AI-generated portfolio analysis and contextual chat.
- Automated tests for calculations, persistence and user flows.

## Architecture

```text
React + TypeScript PWA
        │
        ├── Context + reducers
        ├── Reusable calculation hooks
        ├── Local browser persistence
        ├── Recharts visualizations
        ├── Gemini-powered analysis
        └── Vitest + Testing Library
```

## Product decisions

- Simulations do not delete the original subscription.
- Monthly and annual totals are calculated from normalized recurrence data.
- AI recommendations supplement deterministic calculations rather than replacing them.
- The application can remain useful without an AI connection.
- Local persistence keeps the MVP simple and privacy-conscious while the cloud architecture is evaluated.

## Technologies

`React` · `TypeScript` · `Vite` · `Recharts` · `Gemini` · `Vitest` · `Testing Library` · `PWA`

## What this project demonstrates

- Translating a clear financial problem into an understandable product flow.
- Separating deterministic financial logic from generative AI features.
- Building reusable calculations and automated UI tests.
- Designing a PWA that remains useful offline.

## Status

Private MVP. A future public release would require a final security review, deployment configuration and documentation of data-handling boundaries.
