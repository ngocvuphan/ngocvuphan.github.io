# AGENTS.md — vphtec.com

Static personal profile site — single HTML page with embedded CSS, no build tooling.

## Stack

- Static HTML/CSS (no framework, no bundler)
- Deployed via GitHub Pages at `ngocvuphan.github.io` (CNAME: `vphtec.com`)
- Font: Poppins via Google Fonts

## Project structure

```
index.html            — all markup and embedded CSS (Poppins, multi-section portfolio)
site.webmanifest      — PWA manifest
favicon-*.png/.ico    — favicon assets
CNAME                 — custom domain for GitHub Pages
```

## Commands

No build, test, lint, or dev server configured. Open `index.html` directly in a browser to view.

## Deploy

```bash
git add -A && git commit -m "message" && git push origin main
```

## Setup notes

- Fixed nav with smooth scroll; scroll-padding-top: 72px for anchor offset
- Sections: Home, About, Experience, Portfolio, Contact
- Responsive: single-column below 768px
- Accent color: #4f7cff
- Favicon assets: favicon-96x96.png, favicon.svg, favicon.ico, apple-touch-icon.png
- AGENTS.md is local-only (not committed)
