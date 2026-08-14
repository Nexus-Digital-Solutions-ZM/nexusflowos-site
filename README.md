# Nexus Flow OS — Product Site

Static marketing site for Nexus Flow OS, the real-time control panel for
fuel station money, litres, and shifts. Built by Nexus Digital Solutions.

## Structure

```
index.html              Single-page site (no build step — open directly or serve statically)
assets/
  brand/                 Source-of-truth brand kit assets (logo SVG/PNG, favicon sizes)
  video/
    poster.png           Placeholder poster shown until the real walkthrough video is added
    nexus_flow_os.mp4    ⚠️ NOT YET ADDED — see "Known gaps" below
```

## Running locally

No build tooling required. Either:

- Open `index.html` directly in a browser, or
- Serve it statically, e.g. `python3 -m http.server` from this folder, then visit `http://localhost:8000`

## Brand

Colors, wordmark (Courier New), and logo mark are pulled directly from the
Nexus Flow OS brand kit. Do not recreate these by hand — copy from
`assets/brand/` so the source stays canonical if the kit is updated.

| Token | Value |
|---|---|
| Navy | `#0A1628` |
| Deep blue | `#1A3C6E` |
| Cyan | `#00AACC` |
| Gold | `#E8A020` |
| Gold light | `#F3B94A` |

## Known gaps

- **Demo video missing.** The "See it in action" section references
  `assets/video/nexus_flow_os.mp4`, which does not exist yet. A branded
  placeholder poster is shown in its place so the page doesn't break.
  Drop the real file in at that path (same filename) once it's ready —
  no HTML changes needed.

## Deploying

This is a static site — any static host works (GitHub Pages, Netlify,
Vercel, S3, etc.). No environment variables or server-side code involved.
