# Furniro — Shopify Furniture Storefront (Dawn-based)

A complete, installable **Shopify Online Store 2.0 theme** that implements the popular *Furniro* furniture e-commerce design as a customization of Shopify's **Dawn** reference theme. It ships with several hand-built custom sections on top of a clean Dawn 14 base.

> **This is a self-initiated demo/portfolio theme.** It contains **no client data, no store domain, no analytics IDs, and no confidential information** — the settings ship with empty demo content.

---

## Overview

| | |
|---|---|
| **Type** | Shopify Online Store 2.0 theme (Liquid) |
| **Base theme** | Shopify **Dawn 14.0.0** (see [Licensing & attribution](#licensing--attribution)) |
| **Design** | *Furniro* furniture-store UI concept |
| **Custom sections** | 4 (see below) |
| **External runtime deps** | Swiper (loaded from public jsDelivr CDN) |

The goal of this build was to reproduce a modern furniture-storefront design end‑to‑end on Dawn — theme settings, color schemes, typography, and reusable merchant-editable sections — while keeping the theme upgrade-friendly and free of hard-coded content.

---

## Custom sections built on top of Dawn

All four are standard Online Store 2.0 sections with a `{% schema %}`, merchant-editable blocks, and no hard-coded content (images come from the theme editor via `image_picker`):

| Section file | Editor name | What it does |
|---|---|---|
| [`sections/funiroslider.liquid`](sections/funiroslider.liquid) | **Custom Slideshow** | Split-panel hero: a text/CTA column beside a Swiper slide carousel with per-slide image, link, and overlay text. |
| [`sections/genral-banner.liquid`](sections/genral-banner.liquid) | **General Banner** | Configurable promotional banner section. |
| [`sections/custom-grid.liquid`](sections/custom-grid.liquid) | **Custom Grid Section** | Flexible image/content grid for category or lookbook layouts. |
| [`sections/custom-tabs.liquid`](sections/custom-tabs.liquid) | **Custom Tabs** | Product-page tabbed panel (Description / Additional Information / Reviews) that pulls extra imagery from a `product.metafields.custom.product_description_images` metafield. |

The remaining sections, snippets, templates, and assets are Shopify **Dawn** stock (lightly themed via settings).

---

## Technology

- **Shopify Liquid**, Online Store 2.0 (JSON templates, section groups)
- **Dawn** design system (CSS custom properties, color schemes, `card-product` rendering)
- **Vanilla JavaScript** for section interactions
- **Swiper** carousel library (loaded from the public jsDelivr CDN)
- **Shopify CLI** + **Theme Check** for local development and linting

---

## Run it locally

Requires the [Shopify CLI](https://shopify.dev/docs/themes/tools/cli) and a development store.

```bash
# Preview against a dev store (hot reload)
shopify theme dev --store your-dev-store.myshopify.com

# Lint the theme
shopify theme check
```

---

## Screenshots

See [`screenshots/`](screenshots/). _(Add rendered screenshots of the storefront — see the note in that folder.)_

---

## My role

**Role:** Sole Shopify Developer

I independently implemented and customized this Shopify storefront using Shopify Dawn as the
foundation. My work included developing and configuring custom theme sections, adapting the
storefront layout, implementing responsive behavior, and preparing the theme as a functional
Shopify demonstration project.

### Authorship — what is mine vs. what is not

| Layer | Authorship |
|---|---|
| Shopify **Dawn** base theme | Shopify — not my work |
| Original **Furniro** visual design concept | Original Furniro design — design inspiration, **not my concept** |
| **Shopify implementation** of that design | **My work** |
| **Custom sections** — Custom Slideshow, General Banner, Custom Grid, Custom Tabs | **My work** |
| Theme settings, color schemes, typography, responsive behavior | **My work** |
| Third-party libraries (e.g. Swiper) | Respective authors — not my work |

_Project duration: to be added. No performance, conversion, revenue, or speed metrics are
claimed._

---

## Licensing & attribution

- **Base theme:** built on Shopify **Dawn**. Dawn is distributed under Shopify's theme license (see [`LICENSE.md`](LICENSE.md)), which permits developing, modifying, and distributing themes that integrate with Shopify. The original Shopify copyright notice is preserved in `LICENSE.md`.
- **Design concept:** the visual design is based on the community *Furniro* furniture e-commerce concept. _(Add the original design source/credit link here.)_
- **Swiper** is used under its own MIT license, loaded at runtime from a public CDN.

---

## Confidentiality

This repository is a portfolio/demo theme. It intentionally contains **no** merchant store domain, customer data, API keys, tracking/pixel IDs, or client-confidential assets.
