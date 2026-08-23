# kbrovibes.github.io

The project hub — a grid of everything I build on weekends, at
**<https://kbrovibes.github.io/>**.

Each card links out three ways: the **live app**, the project's **landing page**
(GitHub Pages, hosted in that project's own repo), and the **source**.

## Editing

`index.html` is fully self-contained — inline CSS and JS, no build step, no
dependencies beyond Google Fonts. The project list lives in the `PROJECTS`
array near the bottom of the file — that array is the single source of truth.

Each project draws a purpose-made monoline glyph from the `GLYPH` map (24×24
viewBox, `currentColor`, tinted by the card's `accent`). Add a new glyph there
rather than reaching for an emoji.

Card thumbnails live in `media/<id>.jpg` and are optional — a missing image
leaves the accent-tinted glyph plate showing. Portrait/mobile captures should
set `fit:"contain"` so they letterbox instead of cropping to an unreadable zoom.

Projects whose repo is private set `private:true` and omit `page`; they render
with a "Private" badge and no project-page link.

Kept in sync by hand with `lib/portfolio-data.ts` in
[kbrovibes/portfolio](https://github.com/kbrovibes/portfolio).
