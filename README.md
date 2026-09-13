# Anoop Kumar — Portfolio

A single-file, dark-themed developer portfolio. No build step, no framework, no dependencies to install — open `index.html` and it runs.

**Live:** [anoop-kumar.com](https://anoop-kumar.com) <!-- EDIT ME: remove this line if not deployed yet -->

---

## What's in it

- **Hero** — animated intro loader, full-bleed portrait, gradient name treatment
- **Signal / Metrics** — scroll-triggered animated counters (experience, commits, platforms shipped, articles published)
- **Selected Work** — case studies for TokenPulse, AI Dev Roundup, Velra, and Personal AI Notebook, each with problem/build breakdown, live tech-stack tags, and working GitHub/site links
- **Currently Learning** — an honest stand-in for a certifications wall: what's actually in progress right now, no filler
- **Toolkit** — languages, frameworks, data layers, AI APIs
- **Trajectory** — work experience and education timeline
- **Methodology** — Build → Break → Fix → Write
- **Transmissions** — latest technical write-ups, pulled from dev.to
- **Ground Control** — contact card with a one-click Gmail compose button and a custom-built LinkedIn-style profile card (no dependency on LinkedIn's embeddable badge, which is being deprecated)
- **Resume** — opens directly from the nav, embedded in the page itself
- A generative three.js starfield/nebula background that reacts to scroll and mouse position

## Tech

- Plain HTML, CSS, and JavaScript — no React, no bundler, no `npm install`
- [three.js r128](https://threejs.org/) (loaded via CDN) for the background scene
- Google Fonts: Space Grotesk, Manrope, JetBrains Mono
- All images, the resume PDF, and the logo are embedded directly in `index.html` as base64 — the file is fully self-contained and portable

## Getting started

```bash
git clone https://github.com/anu-ship-it/My-Personal-Portfolio.git
cd My-Personal-Portfolio
```

Then just open `index.html` in a browser. That's the whole setup.

## Editing content

Everything is plain text inside `index.html` — no components, no data files to hunt through. A few spots are marked `<!-- EDIT ME -->` for things that need a personal touch (email, LinkedIn URL, location). Otherwise:

- **Projects** live in the `#work` section — each is a `.proj` block with a title, status, problem/build copy, and tech tags
- **Blog posts** are in the `BLOG_POSTS` array near the bottom of the file — add an entry and it renders automatically
- **Stats** are in `#stats` — each `<span data-target="…">` counts up to that number on scroll
- **Colors, fonts, spacing** are all CSS custom properties at the top of the `<style>` block (`--bg`, `--purple`, `--cyan`, etc.)

## Deploying

Since it's a single static file, any static host works:

- **GitHub Pages** — Settings → Pages → deploy from the branch root (rename `index.html` if needed, or just point Pages at this repo)
- **Vercel / Netlify** — drag-and-drop the file or connect the repo; no build command needed
- **Custom domain** — point your DNS at whichever host you choose

## Contact

- Email: anup17508@gmail.com
- GitHub: [@anu-ship-it](https://github.com/anu-ship-it)
- LinkedIn: [anoop-kumar-a49815262](https://www.linkedin.com/in/anoop-kumar-a49815262)
- Writing: [dev.to/anoop_kumar_63925e275ea06](https://dev.to/anoop_kumar_63925e275ea06)