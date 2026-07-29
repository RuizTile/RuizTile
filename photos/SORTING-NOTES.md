# Sorting notes — from reviewing the uploaded batch

Observations from the photos in `uploads/` (~115 files). Use this to sort next
session without re-viewing everything.

## What the library actually contains

Heavy on **plank** — wood-look porcelain and LVP in grey, greige and warm oak,
plus real **hardwood** (acacia, white oak). This is the biggest category by far,
probably 40% of the set.

Strong second: **large-format grey porcelain floors** — new-construction slabs,
laundry rooms, entries, patios. Many are near-duplicates of the same job.

Also present, in useful numbers:
- **Showers** — subway-tile surrounds, pebble pans, marble-look slabs, benches,
  niches, glass-block wall, a curbless double-shower with arched niche
- **Backsplashes** — herringbone (white and grey gloss), hex mosaic, picket,
  travertine subway, patterned cement-look
- **Fireplaces** — split-face travertine, dark large-format slab, concrete-look
  full-height wall
- **Countertops** — tile-top vanity with metal edge, quartz with tile backsplash
- **Stairs** — one hardwood step-up landing with wrapped nosing (thin here)
- **Patios / outdoor** — covered patio in large-format grey, gravel-and-slab
  walkways, an outdoor kitchen wall

Thin categories: **marble** (mostly marble-*look* porcelain — label carefully),
**glass/mosaic** (a few accent bands), **ceramic**, **natural stone** (the
travertine fireplace, pebble pans).

Some photos are **carpet only** — not tile or hardwood. Skip those, or ask
whether carpet should become its own service.

## Recommended change to the site

The twelve equal folders don't match this library. Suggested weighting:

| Section | Photos |
| --- | --- |
| Plank & hardwood | 15 |
| Porcelain floors | 15 |
| Showers | 12 |
| Backsplashes | 10 |
| Fireplaces | 5 |
| Patios & outdoor | 6 |
| Countertops | 4 |
| Stairs | 3 |
| Marble & stone | 5 |
| Glass & mosaic | 4 |

That's ~79 strong photos — close to the curated ~100 target once the rest of the
drive is added. Per-folder counts need the DC's single `photosPerSection` prop
replaced with a per-section number.

## Next session

1. Confirm the weighting above (or adjust)
2. Sort + rename `uploads/` into `photos/<section>/<section>-NN.jpg`
3. Generate `thumbs/` at 600px from each
4. Update the DC's MATERIALS/SPACES lists and per-section counts
5. Re-bundle `index.html`
