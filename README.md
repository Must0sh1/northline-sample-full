# Northline Sports Management — Static Site Sample

A clean, modern, responsive single-page website for a fictional boutique sports management agency. Built as a **self-initiated portfolio sample** to demonstrate the kind of small static-site work I take on.

> **Note:** This is a personal sample project. "Northline Sports Management" is a fictional brand created for this demo. **It is not real client work** and does not represent a real agency, real athletes, or any existing business.

---

## Project Overview

A responsive single-page static website built around a premium, restrained visual style: dark theme with a black / white / gold palette, generous spacing, and modern card layouts. The goal was to produce something that looks like it could plausibly be used by a real small business — not a flashy concept piece.

### Sections

- **Hero** — agency name, positioning statement, primary CTA, stats row, and a right-side visual panel
- **About** — short description of the agency
- **Services** — Athlete Management, Scouting Support, Race & Event Placement, Sponsorship Support
- **Athletes** — three fictional athlete cards, each with its own sport-themed visual panel
- **Contact** — simple email-based call to action
- **Footer**

---

## What I Built

- Designed the visual style from scratch: dark theme, restrained gold accent, clear typographic hierarchy
- Wrote semantic HTML with proper landmarks (`header`, `main`, `section`, `footer`) and logical heading order
- Built a custom responsive layout using CSS Grid and Flexbox (no UI framework)
- Created lightweight SVG visuals for the hero panel and athlete cards (no image files, no external assets)
- Implemented a mobile navigation menu with a small amount of vanilla JavaScript and proper ARIA attributes
- Tuned spacing, color contrast, and focus states for readability and basic accessibility
- Kept the markup and CSS organized so a client can edit copy or swap content without help

---

## Technologies Used

- **HTML5** — semantic markup
- **CSS3** — custom properties (CSS variables), Grid, Flexbox, `clamp()` for fluid typography, media queries, `aspect-ratio`
- **Vanilla JavaScript** — small script for the mobile menu and the footer year (no frameworks, no build step)
- **Inline SVG** — for the hero and athlete card visuals (resolution-independent, no image requests)

No frameworks, no preprocessors, no external paid assets, no CDN dependencies.

---

## Responsive Design Notes

Tested and tuned across four breakpoints:

- **Desktop** (960px+): full two-column hero, three-column athlete grid, two-column services
- **Tablet** (≤ 960px): hero stacks into a single column, athletes go to a two-column grid
- **Mobile** (≤ 720px): single-column layout, collapsible menu, stats stack vertically, hero panel resizes
- **Small mobile** (≤ 420px): tighter padding, full-width buttons, smaller heading scale

Other responsive details:

- Fluid type scaling using `clamp()` so headings adapt smoothly between breakpoints
- `prefers-reduced-motion` is respected (transitions are reduced for users who request it)
- All interactive elements have visible focus states
- Color contrast meets readable levels for body text against the dark background
- Mobile menu auto-closes on link tap and on resize back to desktop

---

## File Structure

```
.
├── index.html      # Markup
├── styles.css      # All styles
├── script.js       # Mobile menu + footer year
└── README.md       # This file
```

---

## How to Run Locally

No build step is required.

1. Download or clone the project folder.
2. Open `index.html` directly in a browser, **or** serve it locally:
   ```bash
   # Option A: Python
   python3 -m http.server 8080

   # Option B: Node
   npx serve .
   ```
3. Visit `http://localhost:8080` in your browser.

---

## How to Deploy

### GitHub Pages

1. Create a new GitHub repository (e.g. `northline-sports-sample`).
2. Push the project files to the `main` branch.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
5. Wait ~30–60 seconds. GitHub will publish the site at:
   `https://<your-username>.github.io/northline-sports-sample/`

### Netlify (drag & drop)

1. Sign in at [netlify.com](https://www.netlify.com/).
2. From the dashboard, drag the project folder into the **"Want to deploy a new site"** drop zone.
3. Netlify will assign a public URL like `https://your-site-name.netlify.app`.
4. Optional: rename the site or connect a custom domain in **Site settings**.

Both options are free for this kind of static project.

---

## What This Sample Represents

This is the type of work I take on for small clients on Upwork:

- Building or refreshing a small static marketing site
- Implementing responsive layouts from a brief or a rough design
- Fixing HTML/CSS issues, layout bugs, and mobile responsiveness problems
- Updating WordPress-style page templates and content sections
- Deploying static sites to GitHub Pages or Netlify
- Small front-end improvements: typography, spacing, accessibility basics, performance

If you'd like a similar site for your business, or help cleaning up an existing one, feel free to reach out through my Upwork profile.

---

## License

This sample project is free to use for learning or as a starting point. Brand name and copy are fictional.
