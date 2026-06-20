# TK Olymp – Legal Documents

Static GitHub Pages site hosting the Privacy Policy and Terms of Use for the **TK Olymp** mobile app.

**Live site:** https://toby-gamez.github.io/tkolymp-docs.github.io/

## Pages

| Path | Content |
|------|---------|
| `/` | Landing page with links to both documents |
| `/privacy/` | Privacy Policy |
| `/terms/` | Terms of Use |

## Languages

All documents are available in 7 languages, selectable via the in-page switcher or the `?lang=` URL parameter:

| Code | Language |
|------|----------|
| `en` | English |
| `cs` | Česky |
| `de` | Deutsch |
| `sk` | Slovensky |
| `sl` | Slovenščina |
| `uk` | Українська |
| `vi` | Tiếng Việt |

The selected language is persisted in `localStorage` and propagated across pages via the `?lang=` query param. The app opens these pages with the current in-app language pre-selected.

## Structure

```
tkolymp-docs.github.io/
├── index.html          # Landing page
├── privacy/
│   └── index.html      # Privacy Policy
├── terms/
│   └── index.html      # Terms of Use
└── assets/
    ├── style.css        # Shared stylesheet
    └── icon.svg         # App icon (dancer couple)
```

## Updating content

All language content is embedded directly in each HTML file as a JavaScript object. To update a document:

1. Open `privacy/index.html` or `terms/index.html`
2. Find the `const CONTENT = { ... }` block in the `<script>` tag
3. Edit the relevant language key
4. Commit and push — GitHub Pages redeploys automatically

> **Note:** Avoid unescaped ASCII double quotes (`"`) inside JS string values that already use `"` as delimiters. Use `\"` or replace with typographic quotes.

## Effective date

Current effective date: **June 16, 2026**
