# Lumonic Marketing Website Redesign

## Project Context
Redesigning Lumonic's marketing website (lumonic.com). Lumonic is a PitchBook company — a portfolio monitoring platform for private credit and private equity. Serves institutional asset managers monitoring 3,000+ companies. Has an AI conversational agent called "Lu."

Current site is built in Framer. We're rebuilding with a completely new design language.

## Design Direction

### Aesthetic
- **Light mode**, warm off-white background (#FAFAF8)
- AI-forward but grounded in financial services credibility — NOT startup-y or consumer app-y
- Inspired by microsoft.ai and claura.framer.ai visual language
- Subtle noise/grain texture overlay for depth
- Generous whitespace, editorial feel
- Soft blue accent (#2B5CE6)
- Frosted glass / glassmorphism nav on scroll

### Typography
- **Headlines:** Sans-serif — DM Sans, bold weight (700), tight letter-spacing (-2px to -2.5px)
- **Body:** Sans-serif — DM Sans (available on Google Fonts)
- **Accent/secondary:** "Office Times Round" (custom serif font, loaded via local @font-face from project font files) — used for feature card titles, stat numbers, cross-asset headings, and editorial moments. NOT for the main hero headline.
- Office Times Round adds warmth and distinction without dominating — it's a supporting typeface, not the lead.

### Animation & Motion
- Scroll-triggered fade-up reveals with stagger delays (IntersectionObserver)
- Hover lifts on cards with subtle shadow transitions
- Animated chart bars on scroll into view
- Document type marquee
- Frosted glass nav that appears on scroll
- **NO** cursor-follow animations or anything too flashy
- **NO** overwhelming effects — restraint is key for financial software
- Think: polished micro-interactions, not spectacle

### Color Palette
- Background: #FAFAF8 (warm off-white)
- Primary accent: #2B5CE6 (soft blue)
- Text: dark grays, not pure black
- Cards: white with subtle borders and soft shadows
- Dark section for "Meet Lu" AI feature (inverted treatment for contrast)

## Content Rules
- ALL content must be accurate to what Lumonic actually does — reference lumonic.com for real copy
- Should read like a professional copywriter wrote it — no filler, no generic SaaS language
- Key sections: Hero, trust bar (client logos), document type marquee, platform features (data collection, extraction/benchmarking, auditability/source tracing, Lu AI agent, multi-asset support), stats, CTA, footer
- Keep real links to lumonic.com pages
- Don't invent features or stats that don't exist

### Customer Logo Bar
- **Tile grid layout** (4-column grid with 1px borders, like Cursor/Rogo) — NOT a scrolling carousel
- Logos centered in each tile, grayscale with hover reveal
- Only use logos that visually fit the light-mode aesthetic — clean, single-color logos that work on a light background
- **DO NOT** use inverted-color logos or logos that look jarring against the warm off-white background
- If a logo doesn't look right in this context, skip it rather than force it in

## Technical Requirements
- Clean HTML/CSS/JS or React components (Framer-portable)
- Single-file when possible — inline CSS and JS
- Fully responsive
- Use CSS variables for all colors, spacing, and typography
- Prefer CSS-only animations where possible, JS IntersectionObserver for scroll triggers
- Office Times Round: load via @font-face from local font files (woff2/woff). DM Sans: load via Google Fonts.
- Semantic HTML, accessible

## Frontend Quality Bar
- Follow `/mnt/skills/public/frontend-design/SKILL.md` for all frontend work
- Production-grade — this should look like a real shipped website, not a prototype
- Every detail matters: border-radius consistency, shadow uniformity, spacing rhythm, animation easing curves
- Square/minimal-radius CTAs (4px border-radius, NOT pill-shaped), consistent border treatments
- Mock UI illustrations in feature cards should feel realistic and detailed
- No generic AI aesthetics — no Inter font, no purple gradients, no cookie-cutter layouts

## What "Done" Looks Like
A landing page that a visitor would believe was designed by a top-tier agency for a Series B+ fintech company. Polished, credible, distinctive, and accurate.
