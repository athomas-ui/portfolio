# Andrew Thomas — Portfolio Site

A personal portfolio site built as an interactive "newspaper" — **The Andrew Thomas Daily** — positioning Andrew Thomas as a Cybersecurity & GRC Analyst (Security+ certified, i.c.stars Cycle 60, Computer Science/Cybersecurity). The site pairs a professional resume/projects/skills track with a "Program Journey" track (Leadership, Business, Career Planning, Wellness) and a personal track (About Me, Music Showcase featuring an interactive drum kit).

**Live concept:** Andrew Thomas Daily — Vol. 01 / No. 01 — Cybersecurity Edition
**Repo:** [athomas-ui/portfolio](https://github.com/athomas-ui/portfolio)

## Tech Stack

No frameworks, no build step — everything runs straight from the browser:

- **HTML5** — semantic sectioning, ARIA roles/states
- **CSS3** — custom properties (`:root` design tokens for the newspaper color palette), responsive layout with a mobile breakpoint (`max-width: 520px`)
- **Vanilla JavaScript** — tab navigation, keyboard controls, URL hash routing, and the interactive drum kit

## Project Structure

```
portfolio/
├── index.html      # All page content and markup
├── style.css       # All styling, design tokens, responsive rules
├── resume.txt       # Plain-text resume source
└── media/          # Profile photo, performance photos (web-sized JPGs), and video
```

## Features

**Navigation**
- Newspaper masthead plus a sticky, always-visible section bar (scrolls sideways on phones)
- Every section has its own URL hash (`#leadership`, `#technology`, ...), so links open straight to a desk and the browser Back button works
- Old links from v1 (`#overview`, `#projects`, `#skills`) still land on the right section
- Without JavaScript, every section simply shows on one long page

**Content sections**
- **Front Page** — lead story, featured project, an index of the five C60 desks, and a "Position Wanted" classified with contact links
- **Leadership / Business / Technology / Career Planning / Wellness** — the five required C60 desks
- **Technology Desk** — project case studies (Cyber//Breach, Encourage), skills, and tools
- **Career Desk** — career timeline and certification roadmap (earned / in progress / planned)
- **Resume** — certifications, skills, tools, full work history, education
- **About Me** and **Music Showcase** — photo/video gallery plus an **interactive drum kit** (click or press A/S/D/F; sound is synthesized with the Web Audio API and stays off until the visitor turns it on)

**Accessibility**
- Semantic landmarks, one `h1`, and no skipped heading levels
- Skip link, visible focus outlines, and `aria-current` on the active section
- Expandable stories use native `<details>`, so they work with keyboard and screen readers
- Respects `prefers-reduced-motion`

## Running Locally

No install or build required:

1. Clone the repo
2. Open `index.html` directly in a browser, or serve the folder with a local server (e.g. VS Code's Live Server extension) for the cleanest experience

## Build Log

A running record of what's shipped, pulled from the commit history:

**Sept 15, 2026 — Foundation**
Cloned the repo and stood up the initial page structure and styling. Built out the HTML/CSS skeleton, then layered in resume and profile info across several passes.

**Sept 17, 2026 — Resume & About Me**
Added the full Resume section and About Me content, then went back and corrected the About Me copy. Extended the stylesheet to support the new sections.

**Sept 18, 2026 — Content Expansion**
Added a large batch of new content and incorporated feedback/direction from an AI-assisted planning pass.

**Sept 19, 2026 — Presentation Polish**
Added sections required by the i.c.stars presentation guide (Brandie's feedback), fixed font issues, and toned down the visual styling for better balance.

## Roadmap — Portfolio v2

Based on a full audit of the site (Sept 18, 2026), the next round of work is prioritized as:

1. **Build a real Projects section** — replace any remaining placeholder cards with real, detailed case studies
2. **NIST CSF 2.0 risk assessment / GRC project** — an independent project demonstrating Identify, Protect, Detect, Respond, Recover, Govern
3. **Medline OPN 2026 case study** — a public-safe writeup of the i.c.stars Cycle 60 client project
4. **Homepage positioning** — lead immediately with Cybersecurity & GRC Analyst identity and certifications
5. **Evidence-based Skills section** — tie skills directly to projects
6. **Clear CTAs** — GitHub, LinkedIn, Resume download, all explicit
7. **Rewrite generic About Me content** — replace filler with authentic differentiators (teaching, program management, music)
8. **SEO & accessibility polish** — meta description, Open Graph tags, favicon, contrast checks
9. **Move image assets fully into the repo** for asset control
10. **Polish the newspaper/drum visual system** once the content architecture is locked in

## Author

**Andrew Thomas**
[GitHub](https://github.com/athomas-ui) · [LinkedIn](https://www.linkedin.com/in/andrew-thomas-83564259) · athomas@icstars.org
