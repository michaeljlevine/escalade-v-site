# 2023 Cadillac Escalade-V Showcase Website

## Project Overview
Dark, aggressive single-page showcase for the 2023 Cadillac Escalade-V. Focus on raw power and the exhaust note.

## Tech Stack
- Single `index.html` (no frameworks, no build tools)
- Google Fonts: Bebas Neue (headlines), Inter (body), Space Mono (stats)
- GSAP 3 + ScrollTrigger via CDN (scroll animations, counters)
- HTML5 Audio + Web Audio API (exhaust sound with waveform visualizer)
- CSS custom properties for theming

## Sections
Hero (video banner) > Power Stats (animated counters) > Exhaust Note (audio player) > Specs > Gallery > Footer

## Local Dev
```bash
cd ~/escalade-v-site && python3 -m http.server 8080
# Open http://localhost:8080/index.html
```

## Key Files
- `index.html` — entire site
- `audio/escalade-v-exhaust.mp3` — V8 engine sound (CC0, Internet Archive)

## Notes
- Audio won't play from file:// — must serve via HTTP
- Gallery has placeholder divs — swap with real `<img>` tags when photos are ready
- Hero video is commented out — add WebM/MP4 sources when available
