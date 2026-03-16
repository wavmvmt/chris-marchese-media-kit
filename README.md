# Chris Marchese — Creator Media Kit

A luxury single-page media kit for creator and entrepreneur **Chris Marchese** (@thechrismarchese).  
Built to be shared with hotels, resorts, and luxury lifestyle brands as a partnership pitch.

---

## 🌐 Live Site
> Deploy to Vercel — link will go here once live.

---

## 🎯 Project Brief

**Who:** Chris Marchese — Canadian entrepreneur, creative director, founder of SET Enterprises.  
**What:** A cinematic digital media kit designed to pitch luxury brand collaborations.  
**Vibe:** Hollywood-Miami. Dark luxury. Cinematic. High-class. Engaging and interactive.  
**Audience:** Hotel GMs, resort marketing teams, luxury lifestyle brand directors.  
**Goal:** Brands open this link, feel the quality immediately, and want to collaborate.

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary Gold | `#C8A96E` |
| Gold Light | `#E8CFA0` |
| Black | `#080808` |
| Surface | `#111111` |
| White | `#F5F2EE` |
| Display Font | Cormorant Garamond (Google Fonts) |
| UI Font | Barlow Condensed (Google Fonts) |
| Body Font | Barlow (Google Fonts) |

**Aesthetic rules:**
- Film grain overlay always present (subtle, ~3% opacity)
- Custom animated gold cursor — scales on hover
- Scroll-reveal animations on all sections (translateY fade-in)
- Animated counters trigger on scroll entry
- Gold accent lines, borders, and dividers throughout
- NO generic design patterns. NO purple gradients. NO Inter/Roboto fonts.
- All backgrounds dark unless a section break requires contrast

---

## 📄 Page Structure

```
/ Hero          — Full-screen cinematic bg, name, tagline, scroll cue
/ Ticker        — Scrolling gold stats bar (360K, 1.5M views, etc.)
/ About         — Two-column: copy left, overlapping photos right
/ Metrics       — 4-card dark grid with animated counters
/ Gallery       — Editorial masonry photo grid (6 images)
/ Reel          — Video reel placeholder + 3 stat callouts
/ Audience      — Demographics bars + interest tags
/ Packages      — 2 collaboration package cards + production note
/ Brand Fit     — 4-cell grid for brand alignment categories
/ Contact       — Full-bleed bg overlay, links, CTA button
/ Footer        — Minimal: name, kit label, social links
```

---

## 📸 Asset Replacement Guide

All placeholder images are from Unsplash. Replace with Chris's actual content:

### Photos
Drop real photos into `/assets/images/` and update these sections in `index.html`:

| Section | Element | Replace With |
|---|---|---|
| Hero background | `.hero-img` background-image | Best wide landscape/resort shot |
| About — main | `.about-img-main` background | Portrait or editorial lifestyle shot |
| About — float | `.about-img-float` background | Travel or destination shot |
| Gallery g1 | `<img src="...">` | Wide resort/hotel exterior |
| Gallery g2 | `<img src="...">` | Portrait or vertical lifestyle |
| Gallery g3 | `<img src="...">` | Travel/destination wide |
| Gallery g4 | `<img src="...">` | Vertical lifestyle/fashion |
| Gallery g5 | `<img src="...">` | Wide landscape or experience shot |
| Gallery g6 | `<img src="...">` | Interior/luxury detail |
| Contact bg | `.contact-bg` background | Dramatic landscape or resort aerial |

### Video
Drop showreel into `/assets/video/` then replace the reel section:

```html
<!-- Replace the .reel-placeholder div and .reel-play div with: -->
<video
  class="reel-video"
  src="/assets/video/reel.mp4"
  poster="/assets/images/reel-poster.jpg"
  controls
  playsinline
></video>
```

---

## 📊 Chris's Stats (Source of Truth)

| Metric | Value |
|---|---|
| Instagram | @thechrismarchese — 360K followers |
| LinkedIn | Chris Marchese — 8.2K followers |
| Total Reach | 368K+ |
| Monthly Views | 1.5M |
| Monthly Interactions | 142K |
| Avg Reel Views | 160K |
| Top Reel Record | 700K+ views |
| Based | Toronto / Miami |
| Website | thechrismarchese.com |
| IMDb | Listed |

---

## 💼 Collaboration Packages

### Option A — Hosted Stay
- In exchange for complimentary accommodation
- 1 Instagram collab post
- 1–2 story posts per day
- Short-form video/reel coverage
- Cross-platform exposure
- **Est. value: $10,000 USD**

### Option B — Content Production
- Up to 30 pieces of professional content per stay
- High-res videos, photos, reels
- Full usage rights for marketing
- Creative team available
- **Value: $7,500–$12,000+ USD**

### Production Notes
- May require: videographer/photographer, creative assistant
- Team accommodation discussed per-project

---

## 🔒 Optional Features (Future)

- **Password gate** — Add a PIN entry screen before the kit loads (for exclusive outreach)
- **PDF export** — Printable version for email attachments
- **Analytics** — Add Vercel Analytics or Plausible to track views and time-on-page
- **Contact form** — Replace the mailto CTA with a real form (Formspree or similar)
- **Dark/Light toggle** — Offer a light luxury variant for certain brand preferences

---

## 🛠 Claude Code Instructions

When working on this project, Claude Code should:

1. **Preserve the design system** — Never change fonts, colors, or core aesthetic
2. **Keep it a single file** (`index.html`) unless assets require `/assets/` folder
3. **No frameworks** — Pure HTML, CSS, JS only. No React, no bundlers.
4. **Performance matters** — Lazy-load images, keep animations GPU-accelerated (transform/opacity only)
5. **Mobile-first on edits** — Always check the responsive breakpoint at 900px
6. **Film grain stays** — The `.grain` overlay is intentional, do not remove it
7. **Cursor stays** — The custom cursor is part of the luxury UX, preserve it

### Common Tasks for Claude Code
```
"Replace all placeholder images with the files in /assets/images/"
"Add a password gate that shows before the page loads — PIN: 2025"
"Add a mobile hamburger menu for the nav"
"Make the gallery a horizontal scroll carousel on mobile"
"Add a Formspree contact form replacing the mailto button"
"Add Vercel Analytics tracking"
"Create a /assets/ folder structure and update all image paths"
```

---

## 🚀 Deployment

**Local development:**
```bash
# Just open index.html in browser, or use a simple server:
npx serve .
# or
python3 -m http.server 8080
```

**Deploy:**
```bash
git add .
git commit -m "your message"
git push origin main
# Vercel auto-deploys on every push
```

---

## 👤 Contact Info (For Page Updates)

| Field | Value |
|---|---|
| Name | Chris Marchese |
| Email | *(add real email)* |
| Instagram | @thechrismarchese |
| LinkedIn | Chris Marchese |
| Website | thechrismarchese.com |
| IMDb | Chris Marchese |
| Location | Toronto / Miami |
| Company | SET Enterprises |

---

*Built by WAVMVMT · Powered by Claude*
