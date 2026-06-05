# Marvels Team 2026 — Web Deck

A self-contained, static web version of `Marvels_Team_2026.pptx`. Every slide is the
original PowerPoint render (pixel-for-pixel), locked to 16:9, with the deck's real
slide transitions reproduced in the browser.

## What's inside
- `index.html` — the viewer (HTML/CSS/JS, no build step, no dependencies)
- `slides/` — the 13 slides rendered straight from PowerPoint (WebP, visually lossless)
- `vercel.json` — static hosting + caching config

## Controls
- **→ / Space / click-right** : next · **← / click-left** : previous
- **Home / End** : first / last slide · **F** : fullscreen · **swipe** on touch

## Transitions (matched to the original .pptx)
| Slides | Effect |
|--------|--------|
| 1, 12, 13 | Fade through black |
| 2–10 | Morph → smooth crossfade (closest web equivalent) |
| 11 | Push (from bottom) |

## Deploy
It's a plain static site — host the folder anywhere.

**Vercel (CLI):**
```bash
npm i -g vercel
vercel            # preview
vercel --prod     # production URL to share
```

**GitHub + Vercel (dashboard):** push this folder to a repo, "Add New Project" on
vercel.com, import the repo, deploy. No framework/build settings needed.
