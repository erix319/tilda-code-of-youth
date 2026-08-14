# Код молодости

Health and longevity course — a Tilda landing page, exported as a static site.

**Live:** https://erix319.github.io/tilda-code-of-youth/

## About

Course page for a naturopathy-led health and rejuvenation programme — audience fit, curriculum across nutrition, hormonal health and diagnostics, cohort start date, and links to the public offer and privacy policy.

Interface language is Russian.

## Stack

- **Tilda** — Zero Block layout, built from the platform's page builder
- **Static export** — plain HTML, CSS and JavaScript, no build step and no server
- Tilda's runtime bundle: grid, lazy-loading, forms, menu and animation modules

## Running locally

Any static file server works. From the repository root:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

Opening `index.html` straight off the filesystem mostly works too, but a
server is closer to how it is actually deployed.

## Layout

```
index.html   the page itself
assets/      16 files — styles, scripts, images and fonts
```

## Notes

- Archived from https://project8312772.tilda.ws, then repackaged: the saved asset folder was renamed
  to `assets/` and every reference rewritten, so the paths survive being served
  over HTTP instead of only from a local disk.
- This export references Tilda's CDN for every asset, so the page needs an internet connection to render even when served locally.
- Third-party endpoints in the original markup are left untouched. Forms still
  post to Tilda's handler and analytics still call home, so anything submitted
  here goes wherever the original site pointed it — treat this as a display
  copy, not a working intake channel.
