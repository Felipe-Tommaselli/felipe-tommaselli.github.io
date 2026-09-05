# Local development

Static site — no build step. Serve the repo root and open the printed URL.

```bash
python3 -m http.server 8000
# http://localhost:8000
```

Any static server works, e.g.:

```bash
npx serve .
```

Hard-refresh (Ctrl+Shift+R) after editing `stylesheet.css` or replacing images, since
`index.html` pins cache-busting query strings (e.g. `?v=20260830`) on assets.
