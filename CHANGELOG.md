# Changelog

All notable changes to this theme are documented here.

## [Unreleased]

### Added
- Initial public portfolio release.
- Custom Online Store 2.0 sections on a Dawn 14 base:
  - **Custom Slideshow** (`funiroslider`) — split-panel Swiper hero.
  - **General Banner** (`genral-banner`) — configurable promo banner.
  - **Custom Grid Section** (`custom-grid`) — flexible image/content grid.
  - **Custom Tabs** (`custom-tabs`) — metafield-driven product tabs.
- Furniro furniture-storefront theme settings, color schemes, and typography.

### Changed
- Modernized image output in the custom sections: replaced the deprecated `img_url` filter
  with `image_url` + `image_tag` (adds responsive `srcset`/`sizes`, `width`/`height`, and
  lazy loading) in `custom-grid`, `custom-tabs`, and `funiroslider`.
- Deferred the Swiper library in `funiroslider` and moved initialization to `DOMContentLoaded`
  so it no longer blocks page parsing.

### Fixed
- Repaired a broken `<style>` block in `custom-grid` (Liquid tags had been split across lines
  by a formatter, so the CSS rendered literally) and aligned the heading markup with its CSS.

### Notes
- Authored by a single developer (Sole Shopify Developer). Base theme: Shopify Dawn 14.0.0;
  Dawn stock files are unmodified except where noted.
- Demo content only — no client store data included.

---

_Format based on [Keep a Changelog](https://keepachangelog.com/)._
