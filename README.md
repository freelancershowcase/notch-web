# Notch

A concept online shop for a small UK denim label, made as a portfolio piece.

## What it is

Notch sells three cuts of jeans (Straight, Wide and Taper) plus a few hand-printed one-of-ones. The main idea is the **Fit finder**: instead of measuring your body, you measure a pair of jeans you already like. The site picks your closest size in each cut, draws the Notch outline over yours, and shows the difference in centimetres.

What you can try on the site:

- Pick a size once on Shop all and see stock and fit notes for that size
- Add to bag from Shop all or a product page. A side drawer opens with a fit check
- The bag is kept in your browser across pages; checkout moves it to the order page
- Fit finder with a step-by-step tutorial, which you can reopen from "How it works"
- One-of-one pairs with their own measured numbers and a 15-minute hold message
- The printed brochure as its own page (`brochure/`): flip the bundle cards, open the mailer and try the tracing card

## Notes

- This is a concept, not a real shop. Products, people and prices are made up, and the photos are AI-generated and art-directed.
- Bracketed values like `[£X.XX]` or `[@handle]` are placeholders.
- Only W80 Regular is treated as a measured sample. The other sizes follow a proposed grading.
- Checkout is not real. "Check out" goes straight to the order confirmation.

## How it's built

Plain HTML pages with a small runtime (`js/dc-lite.js`) that renders each page's template, handles state, and keeps the bag in `localStorage`. DOM updates use [morphdom](https://github.com/patrick-steele-idem/morphdom) (MIT). There's no build step and no framework, so it loads fast and runs on any static host. For GitHub Pages, upload these files to the repo root and serve from the main branch.

Fonts: Figtree (SIL Open Font License) and Piscolabis for page titles.

## Rights

© 2026 Notch concept. All rights reserved. The design, copy and images may not be reused without permission. morphdom and Figtree keep their own licences.
