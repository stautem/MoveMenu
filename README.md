# MoveMenu

A no-frills gym reference: pick a plan, see the day's categories and sets/reps, tap a category to see movement options and how to do them. No login, no logging, no app — just a page to check on your phone at the gym or print out.

Real names are never used anywhere in this repo. People are referred to by nickname only (`Glute General`, `Balance Boss`).

## Editing content

Everything is hand-written HTML, no build step:

- `index.html` — landing page, links to each person's plan
- `glute-general.html` / `balance-boss.html` — one page per person
- `styles.css` — shared screen + print styles
- `images/equipment/` — reference photos of available equipment

To change a workout split, edit the `<table class="split">` rows. To change the movements available for a category, edit the matching `<div class="card">` section further down the same page. Each movement has an HTML comment (`<!-- image: none yet -->`) marking where a future image/GIF can be added.

## Printing

Open a plan page in a browser and use Print (or Save as PDF) — a print stylesheet strips the navigation and keeps each category on a clean page.
