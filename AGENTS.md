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

- Fixed nav with smooth scroll + shrink effect on scroll; scroll-padding-top: 72px
- Sections: Home, About, Experience, Portfolio, Contact
- Responsive: single-column below 768px
- Accent color: #4f7cff
- Favicon assets: favicon-96x96.png, favicon.svg, favicon.ico, apple-touch-icon.png
- Dark mode toggle (persisted in localStorage)
- Typing effect in hero tagline (cycles through 5 phrases)
- Scroll-triggered fade-up animations (IntersectionObserver, no library)
- Vertical timeline with connector line + dot markers in Experience section
- Project cards with tech tags in Portfolio section
- Mailto CTA button in Contact section
- Back-to-top button (appears after 400px scroll)
- Social icon row in footer
- Gradient hero background with subtle circuit-grid pattern overlay
- AGENTS.md is local-only (not committed)
