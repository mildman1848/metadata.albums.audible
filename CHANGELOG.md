# Changelog

Deutsch: [CHANGELOG.DE.md](CHANGELOG.DE.md)

All notable changes to this project will be documented in this file.

## 1.0.7 - 2026-03-15

- Restricted album artist extraction to the first Audible author only, matching the Mp3tag `Add single album artist only` behavior.
- Kept narrators out of album artist metadata so Kodi interpreters stay author-only.

## 1.0.6 - 2026-03-15

- Fixed Audible search result parsing so album matches no longer mix fields across adjacent products.
- Fixed album detail extraction to keep the actual audiobook title instead of occasionally taking a nested series title.
- Switched review extraction to the extended product description so Kodi no longer shows truncated `p` plot text.

## 1.0.5 - 2026-02-21

- Added a `500` image-size fallback for cover extraction when larger Audible product images are unavailable.

## 1.0.4 - 2026-02-21

- Aligned the scraper with ASIN-tagged STRM export workflows and republished the package metadata.

## 1.0.3 - 2026-02-21

- Switched scraper settings to Kodi legacy format to restore editable settings dialogs.

## 1.0.2 - 2026-02-21

- Fixed Kodi settings parsing by adding explicit `<control>` definitions for all scraper settings.

## 1.0.1 - 2026-02-21

- Simplified the debug workflow with `tools/debug_audible_scraper.py` in the original monorepo.
- Added addon settings scaffolding.
- Added German and English language files.
- Prepared community translation interfaces with `strings.pot` and `resources/i18n/README.md`.

## 1.0.0 - 2026-02-21

- Added the first installable Audible album scraper based on the Audible API mapping from the Mp3tag source package.
- Added repository packaging and index integration for the Kodi repo.
