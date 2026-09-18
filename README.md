# BUDT748 Fall 2026 — Client Side Technologies Project

A three page responsive website designed in **Figma** and rebuilt with
**HTML, CSS, and Bootstrap 5**.

**Student:** Nandini Sinha
**UID:** 122157217
**Email:** nsinha11@umd.edu
**Course:** BUDT748 — Client Side Technologies, Fall 2026
**Professor:** Paul T. Shapiro
**Institution:** Robert H. Smith School of Business, University of Maryland

---

## Live Site

<!-- Paste your GitHub Pages URL here once it is deployed -->
https://github.com/nandinisinha-rvce-umd/nandini-budt748-website

---

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero banner, call-to-action buttons, three category cards |
| About | `about.html` | Course heading, professor / semester / TA details, profile card, course write-up |
| Contact | `contact.html` | Course team contacts, profile card, and a Bootstrap contact form |

---

## Project Structure

```
budt748-website/
├── index.html          Home page
├── about.html          About page
├── contact.html        Contact page
├── css/
│   └── styles.css      Custom stylesheet (loaded after Bootstrap)
├── images/             Figma exports and screenshots
└── README.md
```

---

## Design System

Colors were chosen in Figma and carried into CSS as custom properties
in `:root`.

| Token | Hex | Used for |
|-------|-----|----------|
| `--cream` | `#FDF4EB` | Page background |
| `--ink` | `#222B36` | Headings and dark text |
| `--muted` | `#6E7681` | Secondary text |
| `--coral` | `#F2645A` | Primary accent, buttons, brand underline |
| `--teal` | `#4EC5B0` | Secondary accent and buttons |
| `--amber` | `#F0A93C` | Pill accent and data card |
| `--mint` | `#CFE7DC` | Large decorative circle, top right |
| `--blush` | `#F9DDD4` | Large decorative circle, bottom left |

**Typography:** Montserrat (400, 500, 600, 700) loaded from Google Fonts.

---

## Bootstrap Components Used

- **Navbar** — `navbar navbar-expand-lg` collapses into a hamburger menu below 992px
- **Grid system** — `container` / `row` / `col-md-4`, `col-lg-3`, `col-lg-5`, `col-lg-7`, `col-sm-6`
- **Buttons** — `btn` base class extended by custom `.btn-coral` and `.btn-teal`
- **Forms** — `form-label`, `form-control`, and an alert for the confirmation message
- **Utilities** — `g-3`, `g-5`, `mb-3`, `w-100`, `text-center`, `d-flex`, `justify-content-end`

Bootstrap is loaded from the CDN, so there are no files to install:

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

---

## Custom CSS Beyond Bootstrap

- CSS custom properties for the whole color palette
- Two soft decorative circles that bleed off the edges of each hero section
- The amber capsule accent above every page heading
- A coral underline on the brand mark, drawn with a `::after` pseudo-element
- Hover lift and colored glow on the buttons and category cards
- A flexbox sticky footer so short pages still fill the window
- Light theme restyling of the Bootstrap form controls
- Media queries at 991px and 767px for tablet and phone layouts

---

## Running Locally

1. Clone or download this repository.
2. Open the folder in **VS Code**.
3. Install the **Live Server** extension.
4. Right click `index.html` and choose **Open with Live Server**.

An internet connection is required the first time so the Bootstrap and
Montserrat CDN files can load.

---

## Deployment

Published with **GitHub Pages** from the `main` branch, root folder.
