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
└── media/          # Performance photos/video for the Music Showcase
```

## Features

**Navigation**
- Tabbed layout (`role="tablist"` / `role="tab"` / `role="tabpanel"`) grouped into three tracks: Professional, Program Journey, Personal
- Keyboard navigation between tabs with the arrow keys
- Active tab reflected in the URL hash, so a link can drop someone directly into a section
- `aria-selected` and `hidden` attributes managed in JS to keep the tab state accessible

**Content sections**
- **Overview** — the career narrative in three parts (main story, current focus, what's next)
- **Resume** — certifications, skills, tools, full work history, education
- **Projects** — case study writeups (currently: the i.c.stars Cycle 60 client consulting project)
- **Skills** — evidence-based skill categories (Security & Risk, Operations, Tools)
- **Leadership / Business / Career Planning / Wellness** — the "Program Journey" story told through i.c.stars
- **About Me** — hobbies, music, family
- **Music Showcase** — photo/video gallery plus an **interactive drum kit** (click or press A/S/D/F to hit kick/snare/hi-hat/crash, with a live hit counter and `aria-live` status updates)

**Accessibility**
- Semantic landmarks (`header`, `nav`, `main`, `footer`)
- ARIA labels on icon-only and interactive elements
- Live region (`aria-live="polite"`) on the drum kit status text
- Keyboard support throughout (tabs and drum pads both work without a mouse)

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
