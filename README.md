# MoveMenu

A no-frills gym reference: pick a plan, see the day's categories and sets/reps, tap a category to see movement options and how to do them. No login, no logging, no app. Just a page to check on your phone at the gym or print out.

Real names are never used anywhere in this repo. Plans are labeled generically (`Plan A`, `Plan B`), not tied to any person.

## Editing content

Everything is hand-written HTML, no build step:

- `index.html`: landing page, links to each plan
- `plan-a.html` / `plan-b.html`: one page per plan
- `styles.css`: shared screen + print styles

To change a workout split, edit the `<table class="split">` rows. To change the movements available for a category, edit the matching `<div class="card">` section further down the same page. Each movement has a `watch demo` link (`class="demo-link"`) pointing to a verified exercise demonstration; swap it out or add an image/GIF alongside it if you have your own media later.

## Printing

Open a plan page in a browser and use Print (or Save as PDF). A print stylesheet strips the navigation, keeps each category on a clean page, and prints the demo link's full URL next to it since it isn't clickable on paper.
