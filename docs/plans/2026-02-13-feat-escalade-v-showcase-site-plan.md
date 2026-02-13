---
title: 2023 Cadillac Escalade-V Showcase Website
type: feat
date: 2026-02-13
---

# 2023 Cadillac Escalade-V Showcase Website

## Overview

A dark, aggressive single-page showcase website for the 2023 Cadillac Escalade-V. Built as a single `index.html` with embedded CSS and JS — no frameworks, no build tools. Focus: raw power and the exhaust note.

## Tech Stack

- **Structure:** Single `index.html`
- **Typography:** Google Fonts (Bebas Neue for headlines, Inter for body)
- **Animations:** GSAP 3 + ScrollTrigger (via CDN, free)
- **Audio:** HTML5 `<audio>` + Web Audio API for waveform visualization
- **Video:** `<video autoplay muted loop playsinline>` with poster fallback
- **Gallery:** CSS Grid + vanilla JS lightbox
- **Colors:** CSS custom properties — near-black backgrounds, off-white text, Cadillac gold (#c4a962) accent

## Sections (Scroll Order)

### 1. Hero — Video Banner
- Full-viewport video background (muted, looping, autoplay)
- Dark gradient overlay fading to black at bottom
- Title: "ESCALADE-V" in massive Bebas Neue
- Subtitle: "THE FIRST-EVER" in gold accent
- Tagline: "682 HP of Supercharged Defiance"
- Animated scroll indicator at bottom
- Mobile: static poster image fallback (no video)

### 2. Power Stats — Animated Numbers
- Key stats animate/count up on scroll into view:
  - **682 HP** | **653 lb-ft** | **0-60 in 4.4s** | **6,217 lbs**
- Tagline: "Three tons. Under 4.4 seconds. No compromises."
- GSAP ScrollTrigger counter animation

### 3. Exhaust Note — Audio Experience
- "HEAR THE V" button with gold border styling
- Plays a short exhaust clip (cold start → rev → idle)
- Audio waveform visualization on canvas (gold bars)
- Description of the 3 exhaust modes: Stealth, Tour, Sport
- Note about the deleted center resonator / straight-pipe approach

### 4. Specs Breakdown — Technical Details
- Engine: Supercharged 6.2L V8 (LT4), hand-built
- Transmission: 10-speed automatic
- Drivetrain: Full-time AWD
- Brakes: Brembo with Edge Red calipers
- Suspension: Magnetic Ride Control 4.0 + Air Ride Adaptive
- Interior: 38" curved OLED, 36-speaker AKG audio, massaging seats
- Starting at ~$149,990

### 5. Gallery — Photo Grid with Lightbox
- CSS Grid layout (mixed sizes: wide, tall, standard)
- Hover zoom effect on images
- Click opens fullscreen lightbox with prev/next navigation
- Keyboard support (arrows, escape)
- Lazy loading on all images

### 6. Footer
- Cadillac V-Series branding
- Disclaimer text
- Minimal, dark

## Implementation Steps

1. **Scaffold `index.html`** — HTML structure with all sections, CDN links (GSAP, Google Fonts), CSS custom properties, base dark theme styles
2. **Build Hero section** — Video element, overlay, title/subtitle, scroll indicator animation
3. **Build Power Stats section** — Stat cards, GSAP counter animation on scroll
4. **Build Exhaust Note section** — Audio player button, Web Audio API waveform visualization, exhaust mode descriptions
5. **Build Specs section** — Styled spec grid/cards with scroll-triggered fade-in animations
6. **Build Gallery section** — CSS Grid image layout + vanilla JS lightbox with keyboard navigation
7. **Build Footer** — Branding, disclaimer
8. **Add placeholder assets** — Placeholder images/video/audio with comments noting where to add real assets
9. **Mobile responsiveness** — Media queries for all sections, video → poster fallback, touch-friendly gallery
10. **Polish** — Smooth scroll, reduced-motion support, final animation timing tweaks

## Asset Notes

The site will use **placeholder images and a placeholder audio file** initially. Real assets to source later:
- Escalade-V photos (Cadillac media library or stock)
- Exhaust note audio clip (~10 seconds, MP3 format)
- Hero video (~15 seconds, muted, MP4 + WebM)
