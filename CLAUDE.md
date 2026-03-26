# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Usolia Network player-facing documentation site, built with **Docsify** (no build step). Content is written in Simplified Chinese. Hosted on GitHub Pages at `docs.usolia.net`.

## Architecture

- **`index.html`** — Docsify entry point and configuration (theme color, plugins, search settings)
- **`sidebar.md`** / **`navbar.md`** — Navigation structure; edit these when adding/removing pages
- **`docs/`** — All documentation content as Markdown files, organized by server:
  - `docs/server/` — Main server docs (economy, ranks, guides, mechanisms)
  - `docs/server/m01b/` — Cozzy Journey server
  - `docs/server/cl02/` — Creative Land II server
  - `docs/server/pl01/` — Planet server
  - `docs/server/archived/` — Deprecated content (old servers, removed features)
  - `docs/guides/` — General user guides (password reset, network troubleshooting)
  - `docs/forum/` — Forum-related docs
- **`assets/`**, **`plugins/`**, **`css/`** — Static resources (Docsify core, plugins, stylesheets) — all self-hosted, no CDN

## Deployment

Push to `main` triggers `.github/workflows/static.yml` which deploys to GitHub Pages automatically. No build/compile step — the repo is served as-is.

## Local Preview

Serve the root directory with any static HTTP server, e.g.:

```bash
npx docsify-cli serve .
```

## Content Conventions

- Docsify callout syntax: `?>` for info boxes
- Inline HTML is used freely for formatting (`<br>`, styled spans, etc.)
- When updating server versions, check `sidebar.md` and the relevant server introduction page
- New pages must be linked in `sidebar.md` to appear in navigation
