# Solo &amp; Proud — The Art of Living Beautifully on Your Own

A cozy, illustrated single-page guide to living happily on your own — cooking for one, home safety, money for solo life, and gentle self-care. **Filter the stories by how you feel right now.**

> Live site: **https://palakpeshwani69428-del.github.io/solo-proud/**

---

## What it is

**Solo &amp; Proud** is a warm, editorial-style landing page for people who live alone and want to do it beautifully. Instead of the usual "here's how to survive being single" framing, it treats solo living as an art form — small meals cooked with care, a home that feels like yours, money handled quietly on autopilot, and rituals that make an empty evening feel full.

Everything is a **single self-contained `index.html`** (plus six illustrations). No build step, no framework, no backend — open the file and it runs.

---

## Features

- **Mood-based story filter** — five moods (Hungry, Anxious, Broke, Lonely, Content) re-sort nine real stories about solo life; click a mood chip and the cards fade, reorder and animate.
- **Nine illustrated stories** with an in-page **article reader modal** — each story opens into a full readable piece with a hero image, category tag, read-time and mood label. Escape or click-outside closes it.
- **Four life pillars** — Cooking for One, Home Safety, Solo Money, Self-Care.
- **Daily ritual checklist** — a five-item interactive checklist with a live progress bar and a rotating gentle message as you tick things off.
- **Cozy Club newsletter** — a friendly, client-side sign-up form with inline confirmation (no data leaves the page).
- **Warm, custom design system** — a cream / peach / terracotta / rose / sage palette, Fraunces + Nunito typography, dotted paper texture, floating hero cards, hover-lift cards, soft shadows and scroll-reveal animations.
- **Fully responsive** — a collapsible mobile nav and single-column layouts on small screens.

---

## Tech

| | |
|---|---|
| Structure | One `index.html` (HTML + embedded CSS + vanilla JS) |
| Styling | Hand-written CSS — custom properties, Grid, Flexbox, keyframe animations |
| Scripting | Vanilla JavaScript (no dependencies, no framework) |
| Fonts | Fraunces &amp; Nunito via Google Fonts |
| Illustrations | Six images in `images/` |
| Backend | None — 100% static |
| Data at rest | None — the newsletter form is client-side only |

---

## Project structure

```
solo-proud/
├── index.html      # the entire site — markup, styles and behaviour
├── README.md       # this file
└── images/
    ├── hero.png         # hero illustration
    ├── cooking.png      # "Cooking for One" pillar / stories
    ├── cozy-home.png    # "Home Safety" pillar / stories
    ├── finance.png      # "Solo Money" pillar / stories
    ├── lonely.png       # "Loneliness" / connection stories
    └── self-care.png    # "Self-Care" pillar / ritual art
```

---

## Run it locally

No build tools required.

```bash
git clone https://github.com/palakpeshwani69428-del/solo-proud.git
cd solo-proud
# just open the file…
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
```

Or serve it (recommended, so the relative `images/` paths resolve cleanly):

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

## Deploying

The repo is published with **GitHub Pages** from the `main` branch root — no workflow needed. Any commit to `main` updates the live site at:

**https://palakpeshwani69428-del.github.io/solo-proud/**

---

## Notes

- The page contains **no analytics, no trackers, no external requests** other than the Google Fonts stylesheet.
- The newsletter form deliberately does **not** transmit anything — it confirms in the UI only. Wire it to a real list before using it publicly.
- Illustrations are illustrations, not photographs of real people.

---

## License

Content and code released for personal and educational use.
