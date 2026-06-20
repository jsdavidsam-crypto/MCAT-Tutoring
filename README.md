# Medvance Prep — Landing Page

A high-converting, single-page marketing site for **Medvance Prep**, an elite MCAT
tutoring matchmaking agency. Built as one self-contained `index.html` using
**Tailwind CSS (CDN)** and **vanilla JavaScript** — no build step required.

## Stack

- HTML5 (semantic, accessible)
- Tailwind CSS via CDN, with brand theme extended inline
- Vanilla JS (smooth scroll, sticky-navbar shadow, mobile menu)
- Inter font (Google Fonts)
- Calendly inline embed for booking

## Before you go live — edit these placeholders

All are clearly commented in `index.html`:

| What | How to find it | Action |
| --- | --- | --- |
| **Stripe links (×3)** | search `STRIPE: Replace` | Replace each `href="#"` on the **Enroll Now** buttons (5h / 10h / 20h tiers) with your Stripe Payment Link |
| **Calendly slug** | search `YOUR_LINK` | Replace `https://calendly.com/YOUR_LINK` with your real scheduling URL |
| **Prices (×3)** | search `PRICE:` / `$X,XXX` | Set the price for each tier |

## Deploy to Vercel

This is a static site — no framework, no build command.

### Option A: Git import (recommended)
1. Push this repo to GitHub.
2. In Vercel: **Add New → Project → Import** this repository.
3. Framework Preset: **Other**. Build Command: *(leave empty)*. Output Directory: *(leave empty / root)*.
4. **Deploy.** Vercel serves `index.html` at the root.

### Option B: Vercel CLI
```bash
npm i -g vercel
vercel          # preview deploy
vercel --prod   # production deploy
```

`vercel.json` is already included with clean URLs and sensible cache/security headers.

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
