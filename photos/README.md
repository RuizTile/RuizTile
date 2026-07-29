# Photos

**One copy of each photo — no thumbnails.** The uploaded WebP files average
~97 KB, which is already small enough to load a full gallery fast. A separate
`thumbs/` tree would save bandwidth but double the file count for no visible gain.

```
photos/
  featured/
    hero.webp     ← home page hero (portrait reads best)
    about.webp    ← About page (portrait)
  plank/          plank-01.webp … plank-13.webp
  hardwood/       hardwood-01.webp … -15
  showers/        showers-01.webp … -24
  porcelain/      porcelain-01.webp … -12
  kitchens/       kitchens-01.webp … -11
  patios/         patios-01.webp … -07
  fireplaces/     fireplaces-01.webp … -05
```

Numbering starts at 01 with no gaps. Each folder's count is declared in the
`SECTIONS` list inside `Ruiz Flooring.dc.html` — if you add or remove files,
that number has to change too.

## Adding more

Export WebP (or JPEG) at **1600px on the long edge, quality 80** — lands around
100–300 KB. Drop them in the right folder, numbered after the last existing file.
Send them and I'll place and renumber them.

Current total is about 9 MB across 87 photos. GitHub Pages allows 1 GB, so there
is room for several hundred more.

## Sorting

File each photo by what the shot is actually *about*, not by what happens to be
visible in the background — a bathroom photographed from the doorway with plank
floor in the foreground is still a shower photo.
