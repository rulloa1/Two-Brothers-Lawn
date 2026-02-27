# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-file static landing page for a local lawn care business. No build step, no package manager, no dependencies to install — everything is loaded via CDN. The entire site lives in `index.html`.

## Architecture

**Single-file, zero-build architecture:**
- All HTML, Tailwind utility classes, custom CSS, and GSAP animation logic are in `index.html`
- Tailwind CSS loaded via CDN (`cdn.tailwindcss.com`) — no `tailwind.config.js`, no purging
- GSAP 3 + ScrollTrigger loaded via CDN for scroll-based animations
- Google Fonts (`Inter`) loaded via `<link>` in `<head>`

**Animation pattern:** Elements needing scroll-reveal get class `gsap-reveal` (sets `visibility: hidden` via CSS). GSAP immediately sets them to `autoAlpha: 1` on load, then animates them in via `fromTo` with `ScrollTrigger`. This prevents FOUC without needing JavaScript-disabled fallbacks.

## Deployment

Hosted as a static file — GitHub Pages, Vercel, or Netlify. Just upload/push `index.html`. No build command needed.

The CI workflow (`.github/workflows/blank.yml`) is a placeholder stub — it currently only echoes text and has no actual checks.

## Design Constraints

- **Color palette:** Slate/grayscale base (`slate-900`, `slate-50`, `slate-400`) with green accents (`green-500`, `green-600`) for nature/growth associations
- **Icons:** Inline custom SVG paths (no icon library) — keeps HTTP requests zero and allows precise custom shapes
- **Contact CTAs:** Use `tel:` and `sms:` href protocols for direct mobile dialing/texting
- **Phone numbers:** Call = `281-451-9214`, Text = `832-376-1419`
