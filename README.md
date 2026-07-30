# Ruiz Flooring — website

Tile and hardwood installation, Albuquerque NM. Static site, no build step.
`index.html` is the whole site (Home, Work, About, Contact) and the file you edit —
`support.js` renders it in the browser. English/Spanish toggle lives in the header.

## Publish (GitHub Pages)

Commit `index.html`, `support.js`, `_ds/` and `photos/` to `main`, then
**Settings → Pages → Deploy from a branch → main → / (root)**.
Live at https://ruiztile.github.io/RuizTile/ a minute after each push.

## Photos

~160 WebP files (~17 MB), lazy-loaded, one copy each. Folders and counts live in
the `SECTIONS` list inside `index.html`; when you add or remove photos, update that
section's `n` (and its `skip` list). Don't renumber a folder — that corrupts it.

## Site facts

- (505) 319-7653 · Eleazar7653@gmail.com
- Albuquerque and surrounding area · installing since 2013 · insured · free estimates · English/Español
