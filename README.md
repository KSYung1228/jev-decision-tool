# Jev Decision Tool

A static GitHub Pages interface for making structured decisions with TypeSafe Jev.

## GitHub Pages

The site is served from `docs/index.html`. It provides Choice, Score, and Noul decision modes, presets, probability bars, and confidence / review guidance.

Each user enters their own TypeSafe API key in the page. The key is kept in page memory only and is not written to this repository.

## Important limitation

TypeSafe's HTTP API currently requires an Authorization header, and its browser CORS preflight is not enabled for GitHub Pages origins. As a result, the pure static version may be blocked when it tries to call Jev directly from a browser. A small HTTPS backend relay is required for a fully working public deployment. Do not put a shared API key in this repository or in browser JavaScript.

## Local preview

Open `docs/index.html` directly in a browser, or serve the repository with a static HTTP server.
