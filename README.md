# Bonnie&Frame

A made-to-measure interior textile atelier in Dubai. Custom upholstered headboards, cushions, bed skirts, benches and textile details.

This repository contains the brand's landing page — a single-file `index.html` with no build step.

---

## Structure

```
.
├── index.html              # The landing page
├── logo-system.html        # Brand & logo system overview
├── BonnieAndFrame.jsx      # Same site as a standalone React component
├── logo/
│   ├── bonnie-frame-logo.svg               # Primary stacked wordmark
│   ├── bonnie-frame-wordmark.svg           # Single-line wordmark
│   ├── bonnie-frame-wordmark-tagline.svg   # Wordmark + tagline
│   ├── bonnie-frame-stacked.svg            # Stacked variant
│   └── bonnie-frame-monogram.svg           # B&F monogram
└── images/                 # Drop your photographs here
```

## Local preview

Open `index.html` directly in a browser — no server needed. Everything is loaded from CDN (Tailwind, React, Google Fonts).

## Replacing the placeholder photographs

Each image area in the page is a numbered placeholder (1–16) marked clearly in the HTML:

```html
<!-- IMAGE 7 — Atelier feature -->
<div class="placeholder absolute inset-0" data-num="7"></div>
```

To swap a placeholder for a real photograph, replace the `<div>` with an `<img>`:

```html
<img src="images/your-photo.jpg"
     alt="Description"
     class="absolute inset-0 w-full h-full object-cover" />
```

For the hero accent (image 1) the page already references `images/hero-accent.jpg` with the placeholder as a fallback — just save your photograph at that path.

## Typography

- **Headlines** — Playfair Display (closest free alternative to Noe Display)
- **Body** — Inter

Both loaded from Google Fonts.

## Palette

| Name      | Hex       |
| --------- | --------- |
| Ivory     | `#F5F0E8` |
| Cream     | `#EDE5D7` |
| Beige     | `#E2D5C0` |
| Sand      | `#C9B79C` |
| Taupe     | `#A48A6E` |
| Brown     | `#7A5E47` |
| Espresso  | `#3B2A1F` |
| Ink       | `#1A1410` |

## Deployment — GitHub Pages

1. Push this repository to GitHub.
2. In the repo on github.com, open **Settings → Pages**.
3. Under **Source**, select **Deploy from a branch**.
4. Choose **main** branch, **/ (root)** folder. Save.
5. After ~1 minute, the site is live at `https://<your-username>.github.io/<repo-name>/`.

---

© Bonnie&Frame · Dubai
