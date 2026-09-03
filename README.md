# Код молодости

Health and longevity course — a Tilda landing page.

**Live:** https://pafuluofu-dev.github.io/tilda-code-of-youth/

## About

Course page for a naturopathy-led health and rejuvenation programme — audience fit, curriculum across nutrition, hormonal health and diagnostics, cohort start date, and links to the public offer and privacy policy.

Interface language is Russian.

## Stack

- **Tilda** — Zero Block layout, built from the platform's page builder
- **Static site** — plain HTML, CSS and JavaScript, no build step and no server
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

- Assets load from Tilda's CDN, so the page needs an internet connection to render even when served locally.
