# Seitaro Iwama — Personal Website

Landing page for [https://neuroiwm.github.io/](https://neuroiwm.github.io/).

## Architecture

Hybrid: GitHub Pages hosts the bilingual landing page; Notion holds the actual
content (publications, contact, research statement, etc.).

- **Landing page**: `docs/` — static HTML/CSS, no build step, no JS frameworks.
- **Content**: [seitaro-iwama.notion.site](https://seitaro-iwama.notion.site/)

See [`../info/spec.md`](../info/spec.md) for the full specification.

## Local preview

```bash
cd docs && python3 -m http.server 8000
# open http://localhost:8000/
```

## Layout

```
docs/
├── index.html      # Landing page (name, tagline, JA/EN cards, affiliation)
├── style.css       # Single stylesheet (light/dark, responsive)
├── 404.html
└── assets/
    └── icon.png
```

## Updating

- **Landing page text/links**: edit `docs/index.html`, commit, push.
- **Publications, contact, research**: edit on Notion — changes are live immediately.
