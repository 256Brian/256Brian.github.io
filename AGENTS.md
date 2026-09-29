# Base44 Dev Environment

## Project type
Static HTML website built with Mobirise (GitHub Pages). No backend, no build step, no package manager.

## Running
- Served by `nginx:alpine` via `docker-compose.base44.yml`, bind-mounted at repo root, exposed on host port 3000.
- Start: `docker compose -f docker-compose.base44.yml up -d`
- Health: `curl -f http://localhost:3000/`
- Pages: `index.html` (Home), `page1.html`, `page3.html`, `page4.html`. Assets in `assets/`.

## Edits
Static files are served directly by nginx — changes appear on browser refresh (or call `reload_preview`). No live-reload dev server is needed.

## Secrets
None required.
