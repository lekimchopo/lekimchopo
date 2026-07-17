# NutriSnap — AI-Assisted Nutrition Tracking

[← Back to profile](../../README.md)

## Overview

**NutriSnap** is a mobile-first nutrition application that uses image understanding to help users estimate meals, record nutrition data and follow progress with less manual input.

The product is designed as an assistant rather than a medical authority: AI suggestions are editable, uncertainty matters and the user remains responsible for confirming the final record.

## Problem

Traditional food tracking is accurate only when users consistently search, weigh and enter every ingredient. That friction makes many people abandon the habit.

NutriSnap explores a faster workflow:

1. Take or upload a food photo.
2. Receive an AI-generated estimate.
3. Review and correct the ingredients and quantities.
4. Save the confirmed result.
5. Track progress through visual summaries.

## Product capabilities

- Camera and image-based meal analysis.
- Editable food and quantity estimates.
- Daily nutrition tracking.
- Progress charts and historical views.
- Structured validation of AI output.
- User accounts and cloud-ready data storage.
- Mobile packaging exploration with Capacitor.
- PDF report generation.

## Architecture

```text
React 19 + TypeScript
        │
        ├── Camera / image input
        ├── Structured validation with Zod
        ├── Gemini multimodal analysis
        ├── Supabase-ready persistence
        ├── Recharts analytics
        └── Capacitor mobile layer
```

## Product and safety decisions

- AI-generated nutrition values are presented as estimates, not guaranteed measurements.
- Users can review and correct results before saving.
- Structured schemas reduce malformed model responses.
- The product avoids presenting itself as medical diagnosis or professional dietary advice.
- Personal nutrition data should be minimized and protected before any public release.

## Technologies

`React 19` · `TypeScript` · `Vite` · `Gemini` · `Supabase` · `Zod` · `Recharts` · `Capacitor` · `jsPDF`

## What this project demonstrates

- Designing a useful multimodal AI workflow.
- Handling uncertainty in image-based estimates.
- Turning model output into structured, editable product data.
- Building a mobile-first experience around a high-friction daily habit.

## Status

Private MVP under active development. This case study contains no user nutrition records, API credentials or proprietary source code.
