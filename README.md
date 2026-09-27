# Web3 Carnival — Website Redesign

A ground-up redesign of the Web3 Carnival website — a global Blockchain & Web3 event platform — with a modern, premium, immersive visual identity. Built as a single self-contained HTML file: no framework, no build step, no dependencies to install.

**Team:** TIRAMISU
**Members:** Riya Kangle, Ananya Raut, Ananya Gupta

## The deliverable

Everything is in **[`web3carnival.html`](./web3carnival.html)**. Open that file and you have the complete site.

## Running it

**Simplest:** double-click `web3carnival.html` (or drag it into a browser tab).

**With a local server** (recommended, so relative asset paths behave exactly as intended):
```bash
python3 -m http.server 8000
# then open http://localhost:8000/web3carnival.html
```

**Hosting it live:** this repo works as-is on GitHub Pages, Netlify, Vercel, or any static host — point them at the repo root (`web3carnival.html` is the site, `_blob/` holds the imagery). If you're using GitHub Pages specifically and want it to load at the site's root URL rather than `/web3carnival.html`, either rename the file to `index.html` before enabling Pages, or add a one-line `index.html` that redirects to it.

## What's covered

- **Homepage** — hero (with ambient background video), a five-scene scroll story, live event stats
- **Upcoming Event / Conference info** — format, cadence, live countdown
- **Event themes / tracks** — a scroll-scrubbed explorer across all seven "Cons"
- **Past Speakers** — 69 speakers, filterable by role, with a full profile lightbox (swipe/keyboard navigable)
- **Past events / editions** — a photo reel and a year-filterable timeline
- **Attendees / ecosystem** — who attends and why
- **Sponsors & Partners** — tiered logo rows, sponsorship deck request flow
- **Get Involved / Registration** — a nine-path role picker feeding a four-step pass builder with a live pass preview and a generated entry code
- **Contact / CTA**, **Footer & social links**
- Full **desktop and mobile** responsive layouts
- A **dark/light theme toggle**, a `/` command palette for site-wide search, and reduced-motion support throughout

## Structure

```
web3carnival.html   → the entire site (markup, CSS, and JS in one file)
_blob/               → imagery referenced by web3carnival.html (hero
                        photography, speaker photos, partner logos)
```

## Tech notes

- Semantic HTML, CSS custom properties for the whole theming system (including the dark/light toggle), and vanilla JavaScript — no framework, no bundler.
- `_blob/` includes a representative set of the site's imagery (all hero photography, a sample of speaker photos and partner logos). A handful of secondary/decorative images beyond that sample degrade to a clean placeholder tile rather than a broken-image icon, by design — see the small inline script at the top of `<body>` in `web3carnival.html`.
