# Block Nine — Streetwear Brand and Shopify Product System

[← Back to profile](../../README.md)

## Overview

**Block Nine** is a streetwear and e-commerce project that combines brand development, product validation and a native Shopify Online Store 2.0 implementation.

The project separates visual experimentation from the real commerce system: React is used as a design laboratory, while Shopify remains the source of truth for products, variants, inventory, cart and checkout.

## Problem

A visually impressive prototype is not automatically a safe or operational online store. Real e-commerce requires inventory, payments, product data, legal content, logistics, accessibility and a reliable publishing workflow.

Block Nine was structured to avoid treating a client-side demo as production commerce.

## Product system

- Editorial storefront direction and campaign modules.
- Native Shopify theme using Liquid and Online Store 2.0.
- Responsive navigation and mobile menu.
- Collection filtering, sorting and pagination.
- Product gallery, variants, quantity selection and native forms.
- Cart, search, pages, contact and 404 templates.
- Spanish and English translations.
- SEO fundamentals, Open Graph and canonical URLs.
- Editable sections through the Shopify visual editor.
- Isolated pre-production theme and draft product collection.

## Architecture

```text
Shopify Admin — source of truth
        │
        ├── Products, variants and inventory
        ├── Customers, discounts and orders
        ├── Secure cart and checkout
        └── Native Liquid theme

React / AI Studio prototype
        └── Visual direction and interaction experiments only
```

## Risk and governance decisions

- Checkout and payment data are never handled by the React prototype.
- Products remain drafts until samples, pricing, stock and legal content are confirmed.
- Themes are uploaded as unpublished versions before review.
- Assets with franchise or recognizable character references are excluded.
- Commercial-use rights must be confirmed before publishing generated imagery.
- Secrets, customer exports and Shopify access tokens are excluded from Git.

## Technologies

`Shopify Liquid` · `Online Store 2.0` · `React` · `Vite` · `Shopify CLI` · `GitHub` · `Theme Check`

## What this project demonstrates

- Separating a visual prototype from production commerce architecture.
- Treating operational readiness as part of product development.
- Managing intellectual-property and asset risks.
- Building a controlled GitHub-to-Shopify release process.

## Status

Private pre-production project. The store and products are not represented as commercially launched until manufacturing, legal, logistics and checkout validation are complete.
