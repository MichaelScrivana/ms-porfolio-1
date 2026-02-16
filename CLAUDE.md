# Project Context — AI Lead Application Site

## What This Is
A single-file interactive HTML application site for **Michael Scrivana**, a Senior Brand Designer at Bayer Consumer Health applying for an internal **AI Proficiency & Learning Lead** role within Consumer Health IT (Basel, Switzerland). The file is `michael-scrivana-ai-lead.html`.

## The Candidate
- 6+ years at Bayer Consumer Health, directing creative across 20+ brands (packaging, ecomm, web, social, motion)
- 1 of 5 cross-functional AI team reps, representing Product Experience alongside Product Dev, Regulatory, and Medical
- Self-taught developer building "One A Day" — an orchestrated design review agent on Azure with Claude
- Pioneered GenAI (MidJourney) adoption in the DPX team for photography direction, packaging concepts, and ecomm
- Key win: MiraFAST brand identity — 3rd fastest scaling launch in Digestive Health, $14MM retail sales in 9 months, designed in a 3-week sprint

## The Role (Req ID 860868)
**AI Proficiency & Learning Lead** — Consumer Health IT, Basel (or EU major site), VS 2 grade

Key responsibilities:
- Build a practical AI proficiency program people love to use
- Enable peer-to-peer learning at scale (clinics, office hours, meetups, flow-of-work guides)
- Create role-based learning paths across marketing, ecomm, supply, manufacturing, medical, support
- Embed safety/compliance (EU AI Act, GDPR, PV, GxP) as practical guardrails
- Partner with Focus Area Leads, Product, Governance, BU leaders
- Track adoption via dashboards (usage, time saved, accuracy, compliant content rate)

## Site Architecture
Single HTML file with embedded CSS/JS. Sections in order:

1. **Nav** — fixed top bar, dark mode toggle (dark is CSS default), name links home
2. **Hero** — headline, description, stats (6+ years, 20+ brands, 700+ renders, 1 of 5 AI reps)
3. **About Me** — photo placeholder + bio
4. **AI Projects** — 3 deep-dive project cards (One A Day agent, AI Strategy Consulting, GenAI in Creative)
5. **Role Fit** — 2-column table mapping job requirements → Michael's experience
6. **Design Portfolio** — Featured projects (MiraFAST, PX Platform) + 4-item carousel (OAD, Age Factor, Iberogast, Bold) with click-to-modal detail views
7. **Career Timeline** — Experience + education + references (Chris Padain, Beth Harlor)
8. **Brand Runner Game** — endless runner that auto-starts after education. Player is Bayer cross shape, obstacles are brand-name boxes. Space/tap to jump.
9. **Footer** — contact info, "built with Claude" credit

## Design System
- **Fonts:** Outfit (display), DM Sans (body), IBM Plex Mono (labels/mono)
- **Colors:** Dark default. Accent blue `#4D8FE8` (dark) / `#0047AB` (light)
- **Theme:** `[data-theme="light"]` overrides `:root` dark defaults
- **Animations:** IntersectionObserver-based fade-in on scroll

## Image Placeholders
14 placeholders need real images. They're marked with `[ Description ]` text:
1. Profile photo
2. One A Day agent screenshot
3. AI Team / presentation photo
4. MidJourney style guide examples
5. MiraFAST pack design
6. MiraFAST brand world
7. PX Platform homepage
8. PX Platform project detail
9. OAD Brand Platform
10. Age Factor launch
11. Iberogast
12. Bold Breakthrough Tour
13-14. Modal gallery images per project (4 each)

## Technical Notes
- Dark mode is the CSS default (`:root` = dark, `[data-theme="light"]` = override)
- Footer uses hardcoded `#18181B` background to avoid variable resolution issues
- Game canvas uses `_displayWidth`/`_displayHeight` for logic (separate from pixel dimensions for retina)
- Game reduces particles and skips glow on mobile (`window.innerWidth < 600`)
- Carousel supports touch/swipe, responsive item count (3 → 2 → 1)
- Portfolio modals close via ✕, click-outside, or Escape
- External links: `michaelscrivana.com`, `michaelscrivana.com/marketingexcellence`, GitHub placeholder on project 1

## Contact Info in Footer
- michael.scrivana@bayer.com
- 973.919.7414
- michaelscrivana.com

## How Michael Works
- Learning JS/React/Node/Azure — explain the "why" behind decisions, use clear code comments
- Thinks visually — diagrams and flow descriptions help
- Prefers overview first, then zoom in
- Be direct, skip design/branding over-explanations, go deep on technical concepts
- Flag architectural decisions that are hard to undo
