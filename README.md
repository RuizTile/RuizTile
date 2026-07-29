# Ruiz Flooring — website

Tile and hardwood installation, Albuquerque NM. Static site, no build step.

## Publish to GitHub Pages

Commit these to the root of `RuizTile/RuizTile` on `main`:

```
index.html      the whole site (Home, Work, About, Contact)
support.js      runtime the page loads — required
_ds/            design-system stylesheet + bundle — required
photos/         the photo library
```

Then **Settings → Pages → Deploy from a branch → main → / (root)**.
Live at `https://ruiztile.github.io/RuizTile/` a minute later. Every later push
to `main` republishes automatically.

`index.html` is a copy of `Ruiz Flooring.dc.html` — the editable source. After
any change to the source, the copy has to be remade or the published site is stale.

## Photo library

87+ photos, ~9 MB total, one copy each (no thumbnails — the WebP files average
97 KB, small enough to skip a second size). Lazy-loaded, so gallery size barely
affects load time. See `photos/README.md` for folders, naming and export specs.

Counts live in the `SECTIONS` list inside the source file. Add or remove files
and that number must change too.

| Section | Photos |
| --- | --- |
| Wood-look plank | 15 |
| Hardwood | 14 |
| Showers & tubs | 44 |
| Porcelain floors | 13 |
| Kitchens & baths | 16 |
| Patios & entries | 5 |
| Fireplaces | 9 |

Sections may have gaps in their numbering — a `skip` list in `SECTIONS` names
the removed numbers. Renumbering a folder is what corrupted it once; don't.

All seven folders have now been audited photo by photo. Corrections made: 11 of
plank's 24 were misfiled, plus 5 in hardwood/patios and 2 in porcelain — almost
always a room shot filed by what was visible in the background.

## Site facts (confirmed)

- (505) 319-7653 · Eleazar7653@gmail.com
- Albuquerque and surrounding area
- Installing since 2013 · licensed and insured · free estimates · English/Español
- No hours listed, no quote form — calls and email only, by request

## Open items

1. **Showers is 44 of ~116 photos** — over a third of the library in one section.
   Options: split the marble ones (calacatta, black marble, curved panels) into
   their own Marble section, or trim the near-duplicates.
2. **`uploads/` still holds every original.** It is the recovery source if a
   folder gets scrambled — do not delete it, and do not commit it either.

## Working notes for whoever picks this up

- **Never chain renames through `copy_files`.** Moving `a→b, b→c` in one call
  deletes sources mid-chain; it destroyed the plank and porcelain folders once.
  Re-copy from `uploads/` with explicit destinations instead.
- **`run_script` refuses writes that shrink a file by half**, which blocks
  in-folder renumbering. Same fix: copy from `uploads/`.
- **`view_image` caches by path.** After overwriting a file, a re-view may show
  the old image. Verify by comparing byte sizes against the source instead.
