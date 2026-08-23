# kbrovibes.github.io

The project hub — a grid of everything I build on weekends, at
**<https://kbrovibes.github.io/>**.

Each card links out three ways: the **live app**, the project's **landing page**
(GitHub Pages, hosted in that project's own repo), and the **source**.

## Editing

`index.html` is fully self-contained — inline CSS and JS, no build step, no
dependencies beyond Google Fonts. The project list lives in the `PROJECTS`
array near the bottom of the file. `projects.json` mirrors it for anything that
wants to read the list programmatically; update both together.

Card thumbnails live in `media/<id>.jpg` and are optional — a missing image
falls back to an accent-tinted plate with the project's emoji.

Kept in sync by hand with `lib/portfolio-data.ts` in
[kbrovibes/portfolio](https://github.com/kbrovibes/portfolio).
