# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A zero-build personal portfolio: a single static `index.html` + `style.css` (plus `assets/`). No package manager, no build step, no tests, no framework. Edit the files directly and open `index.html` in a browser to preview.

## Deploy

Deployed to GitHub Pages at `https://barry-mir.github.io/portfolio/`. **Pushing to `main` publishes the live site** — there is no staging environment. Deploy is `git push`; there is no build to run.

## Gotchas

- **Canonical / absolute URLs keep the `/portfolio/` path.** This is a GitHub Pages *project* site, so `<link rel="canonical">`, the JSON-LD `url` fields, and `og:`/Twitter URLs all point at `.../portfolio/`, not the bare domain. Don't "simplify" these.
- **Keep JSON-LD structured data in sync with visible content.** The `<script type="application/ld+json">` blocks (Person + WebSite schemas) in `index.html` duplicate on-page facts. When editing name, links, or profile info, update the structured data too.
- `googlebc588cf56be78771.html` is a Google Search Console verification file — leave it in place.

## Style conventions

- CSS is themed via custom properties in `:root` (`--accent`, `--ink`, `--bg`, `--radius`, `--maxw`, etc.). Reuse these tokens rather than hardcoding colors/spacing.
- Dark mode is a full second palette under `@media (prefers-color-scheme: dark)`. Any new color must be defined for both light and dark.
- Fonts: `--sans` is Inter, `--serif` is Fraunces (loaded from Google Fonts).
- Keep the accessibility scaffolding: skip link, semantic HTML5 landmarks, and proper heading hierarchy.
