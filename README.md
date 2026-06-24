# Ohm Studio — Prompt Engineering Showcase

## Student Information
|         |                                               |
|---------|-----------------------------------------------| 
| Nombre  | Andrea Maccan                                 |
| Materia | Desarrollo de Sistemas Web (Front End) - 2° E |
| Módulo  | PFO2 — Prompt Engineering in AI Agents        |
| Año     | 2026                                          |

## Live Deploy
[Vercel Deploy Link](TBD)

## Project Structure
```
ohm-studio/
├── agent1/
│   └── index.html
├── agent2/
│   └── index.html
├── screenshots/
│   ├── agent1.png
│   └── agent2.png
├── index.html
├── prompt.txt
└── README.md
```

## Prompt Used
```
You are an expert front-end developer working autonomously. Do not ask for confirmation at any point. Inspect the project structure first, then execute the corresponding role based on what you find.

## Step 1 — Detect your role

Check whether the directory `agent1/` exists and contains an `index.html` file.

- If it does NOT exist → you are **Agent 1**. Follow the Agent 1 instructions below.
- If it DOES exist → you are **Agent 2**. Follow the Agent 2 instructions below.

---

## Agent 1 Instructions

Create the file `agent1/index.html`.

### What to build
A complete, self-contained landing page for **Ohm Studio**, a professional music production studio offering recording, mixing, mastering, and music production services for independent artists, bands, and content creators.

### Language
All text, headings, and labels must be in Spanish.
Code names, class names, and IDs must be in English.

### Required sections
1. **Header** — Fixed nav bar with logo "Ohm Studio", links (Servicios, Acerca de, Testimonios, Contacto), CTA button "Reservar una sesión". Functional hamburger menu for mobile.
2. **Hero** — Full-viewport section, headline "Donde el sonido se convierte en arte", subheadline, CTA button "Reservar una sesión". Dark cinematic aesthetic.
3. **About Us** — Studio philosophy, experience, differentiators.
4. **Services** — CSS grid, 4 cards: Recording, Mixing, Mastering, Music Production. Each with inline SVG icon, title, description.
5. **Testimonials** — 3 quote cards: client name, artist type, 5-star rating (Unicode ★).
6. **Contact Form** — Fields: Name, Email, Phone (optional), Service of Interest (select with all 4 services), Message, Submit. Visual only, no backend.
7. **Footer** — "Ohm Studio", copyright 2026, inline SVG icon links: Instagram, YouTube, Spotify.

### Design
- Palette: background `#0a0a0f`, accent `#7c3aed`, text `#f8f8f8`, secondary `#a0a0b0`.
- Fonts via Google Fonts CDN: "Montserrat" (headings, 700/900), "Inter" (body, 400/500).
- Smooth scroll. Fade-in on scroll via Intersection Observer API.
- Mobile-first. Breakpoints: 768px, 1024px.
- No CSS frameworks. CSS gradients and inline SVG only — no external images.

---

## Agent 2 Instructions

`agent1/index.html` already exists. Do not touch it.

Create the file `agent2/index.html` using the same brand, content, and sections as Agent 1, but with a visually distinct implementation: different layout direction, typographic style, and color palette.

### Required sections
Same 7 sections as Agent 1 (Header, Hero, About Us, Services, Testimonials, Contact Form, Footer) with identical content and copy.

### Design — must differ from Agent 1
- Palette: background `#0d0d0d`, accent `#00e5ff`, text `#ffffff`, secondary `#888899`.
- Fonts via Google Fonts CDN: "Space Grotesk" (headings, 600/700), "DM Sans" (body, 400/500).
- Services section: use a layout other than a standard grid (e.g. alternating rows, horizontal scroll).
- Hero: asymmetric or typographic-forward layout.
- Animations via CSS transitions and/or Intersection Observer API.
- Mobile-first. Breakpoints: 768px, 1024px.
- No CSS frameworks. CSS gradients and inline SVG only — no external images.

Then, once `agent2/index.html` is complete, also create the following shared files:

### index.html (root — access portal)
A self-contained entry point to the project. Requirements:
- Title: "Ohm Studio — Prompt Engineering Showcase".
- Dark background `#0a0a0f`, accent `#7c3aed`, Google Fonts "Inter".
- Three card-style links:
  1. "View Prompt" → `./prompt.txt` (new tab). Subtitle: "The exact prompt used with both agents."
  2. "Agent 1 — GitHub Copilot · Claude Sonnet 4.6" → `./agent1/index.html` (new tab). Subtitle: "Landing page generated autonomously by Copilot in VS Code."
  3. "Agent 2 — Cursor · Composer 2.5 Fast" → `./agent2/index.html` (new tab). Subtitle: "Landing page generated autonomously by Cursor."
- Footer with literal placeholder text: `Andrea Maccan — Desarrollo de Sistemas Web (Front End) - 2° E · 2026`.
- Fully responsive. No frameworks. No JavaScript. Embedded CSS only.

### README.md
```markdown
# Ohm Studio — Prompt Engineering Showcase

## Student Information
|         |                                               |
|---------|-----------------------------------------------| 
| Nombre  | Andrea Maccan                                 |
| Materia | Desarrollo de Sistemas Web (Front End) - 2° E |
| Módulo  | PFO2 — Prompt Engineering in AI Agents        |
| Año     | 2026                                          |

## Live Deploy
[Vercel Deploy Link](TBD)

## Project Structure
(generate a markdown file tree reflecting the actual project files)

## Prompt Used
(insert the full prompt verbatim)

## Agents Used
|  Agente  | Herramienta | Modelo                             |
|----------|-------------|------------------------------------|
| Agente 1 | VSCode      | Claude Sonnet 4.6 (GitHub Copilot) |
| Agente 2 | Cursor      | Composer 2.5 Fast                  |

## Screenshots
### Agente 1 — GitHub Copilot
![Agente 1](screenshots/agent1.png)

### Agente 2 — Cursor
![Agente 2](screenshots/agent2.png)

## Notes
Space for observations about differences in agent behavior and output quality.
```

---

## Technical requirements (both agents)
- Single HTML file per agent: all CSS in `<style>` in `<head>`, all JS in `<script>` before `</body>`.
- Semantic HTML5: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`.
- HTML section comments.
- Accessibility: heading hierarchy h1→h2→h3, `alt` attributes, `aria-label` on interactive elements, sufficient color contrast.
- Must render correctly opening the file directly in a browser. Only allowed external dependency: Google Fonts CDN.

## Hard constraints (both agents)
- No Bootstrap, Tailwind, or any CSS/JS framework.
- No external images. No `<img>` with external URLs.
- No TODO comments or incomplete sections.
- No questions. Act immediately and completely.
- All content in English.
- Agent 2 must never modify `agent1/index.html`.
```

## Agents Used
|  Agente  | Herramienta | Modelo                             |
|----------|-------------|------------------------------------|
| Agente 1 | VSCode      | Claude Sonnet 4.6 (GitHub Copilot) |
| Agente 2 | Cursor      | Composer 2.5 Fast                  |

## Screenshots
### Agente 1 — GitHub Copilot
![Agente 1](screenshots/agent1.png)

### Agente 2 — Cursor
![Agente 2](screenshots/agent2.png)

## Notes
Space for observations about differences in agent behavior and output quality.
