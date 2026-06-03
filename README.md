# AHA BLS / ACLS — Blended Learning Landing Page (Wireframe)

A single, self-contained HTML wireframe for the American Heart Association
BLS / ACLS blended-learning campaign. One template is designed once and reused
across markets with country-specific content — the course name (BLS or ACLS) is
a variable, so the same page covers both.

> This is a **design wireframe / prototype** intended as a handoff reference for
> a HubSpot + WordPress build, not a production application.

## Highlights

- **One standalone file** — `wireframe.html` contains all markup, CSS, and JS.
  No build step, no framework, no dependencies to install.
- **Bilingual** — English (LTR) and Arabic (RTL) with a top-right language
  switcher. Every section, label, and control mirrors correctly in RTL.
- **Lead-capture pop-up** — the "Find a Training Centre" buttons open a modal
  collecting **name, phone number, and country** (dropdown of campaign markets),
  followed by a thank-you confirmation with a "Go to Training Center" action.
- **Design system** — AHA red (`#C10E21`) used as an accent only, Montserrat /
  Noto Naskh Arabic type, and a self-contained inline SVG icon set.
- **Responsive** — desktop, tablet, and mobile layouts.

## Page sections

Hero → Why blended learning → What you'll learn → How it works (3 steps) →
Who it's for → Trust strip → Primary CTA → FAQ → International Training Centres
(alphabetical list) → Footer.

## Running it locally

It's a static page — just open it. Either:

```bash
# Option A: open the file directly in a browser
open wireframe.html        # macOS
xdg-open wireframe.html    # Linux

# Option B: serve it (recommended, so relative asset paths resolve cleanly)
python3 -m http.server 8000
# then visit http://localhost:8000/wireframe.html
```

## Files

| File | Purpose |
|------|---------|
| `wireframe.html` | The complete wireframe — markup, styles, and scripts |
| `Group 36.png` | AHA logo for light backgrounds (header, trust strip) |
| `Group 10.png` | AHA logo for dark backgrounds (footer) |

External fonts (Montserrat, Noto Naskh Arabic) load from Google Fonts.

## Notes

- The country dropdown lists the campaign's markets. Confirm the exact market
  list against the campaign plan before build.
- For the production build, the lead-capture form is intended to be implemented
  as a HubSpot form; the modal here is a wireframe demonstration of the flow.
