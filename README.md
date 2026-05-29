# BetNinja — Player Guide (static site)

Independent, international (non-UK-targeted) informational page.
Dark / neon-green theme, fully responsive (desktop + mobile).

## Files
```
index.html      → main page (links logo.svg + favicon.png + style.css)
style.css       → all styles
logo.svg        → vector logo (used in header / hero)
logo.png        → raster logo (apple-touch-icon)
favicon.png     → browser tab icon
go/index.html   → cloaked redirect; /go → partner URL
```

## The /go redirect
- In-page buttons/links pointing to `/go` are intercepted by JS in `index.html`.
- Direct hits to `yoursite/go` are handled by `go/index.html` (JS replace + meta-refresh fallback, `noindex`).
- To change the destination, edit the URL in **both** places: the `PARTNER_URL` constant in `index.html` and all three occurrences in `go/index.html`.

## Deploy on GitHub Pages
1. Create a repo and upload all files (keep the `go/` folder).
2. Settings → Pages → Source: branch `main`, folder `/ (root)` → Save.
3. (Optional) Add a `CNAME` file with your domain + DNS records, then enable "Enforce HTTPS".

## Notes
- 18+ and "check your local law" disclaimers are intentional — keep them.
- Offshore (Anjouan) licence is stated accurately; do not relabel it as UKGC/MGA/GamStop.
