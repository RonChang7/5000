## Cursor Cloud specific instructions

This is a zero-dependency static website (Taiwan 振興5倍券 lottery checker). There is no package manager, no build system, no test framework, and no linter configured.

### Running the app

Serve the project root with any static HTTP server:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html` in a browser. Vue.js 2 is loaded from CDN (`cdn.jsdelivr.net`), so internet access is required.

### Key files

- `index.html` — the entire application (HTML + CSS + inline Vue.js)
- `diamond.svg` — decorative icon

### Notes

- There are no automated tests, linters, or build steps to run.
- All lottery data is hardcoded inside `index.html`.
- External image assets are loaded from `vhpi.5000.gov.tw` (may be unavailable; does not affect core functionality).
