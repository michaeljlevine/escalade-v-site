---
topic: static-showcase-site
date: 2026-02-13
tags: [html, css, gsap, audio, dark-theme]
---

# Static Showcase Site Learnings

## Audio playback from file:// protocol
Browsers block audio playback when opening HTML files directly (`file://`). Must serve via HTTP — use `python3 -m http.server 8080` for local dev.

## Audio player UX
Play/pause icons alone aren't obvious enough. Change the button text ("HEAR THE V" / "STOP") AND the visual style (outlined vs filled) for clear state.

## GSAP + ScrollTrigger via CDN
Works great for cinematic single-page sites. Use `defer` on script tags. Add SRI hashes for security. Fully free now including all plugins.

## Dark theme best practices
- Never use pure #000000 — use #0a0a0a
- Never use pure #ffffff — use #f0f0f0
- Use elevation through lightness levels
- Subtle borders: rgba(255,255,255,0.06)

## Free audio assets
Internet Archive (archive.org/details/car-engines) has CC0 engine sounds. Pixabay and Freesound require login for downloads.
