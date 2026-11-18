# Daedalus Fashion Industries — Garment Pattern Drafter

A browser-based pattern drafting studio for drafting, grading and exporting industry-standard garment patterns, in the spirit of Marvelous Designer, CLO3D and Tailornova. It runs entirely in the browser as a single HTML file, with no install or server.

## Garment categories

The app opens on a launcher with one card per garment. Each card has its own drafting area:

- T-shirt
- Polo T-shirt
- Hoodie
- Knit Dress
- Shirt
- Bodice Block
- Skirt Block
- Trousers
- Shorts
- Track Pants
- Trunks

Every card supports men's, women's and children's (boys' and girls', by age) size charts.

## Drafting features

- Industry-standard drafting with seam allowances, notches, grading and mirrored hem corners
- Sleeve options on knit tops: short or long, set-in or raglan
- Body measurements with a **?** help button on each, showing a diagram of where to measure
- Measurement profiles: save and load as JSON, including design settings, seam allowances, fit and fabric
- Distance measuring tool that snaps to seams
- Per-card Reset that asks twice before resetting, can be undone, and keeps the selected size chart
- Drafting warnings that appear only when a draft has a real problem (for example, a sleeve cap that doesn't fit the armhole)

## Views

| View | What it shows |
|---|---|
| Pattern | The drafted pattern pieces |
| Grade nest | All sizes nested over each other |
| Marker | Pieces laid out for cutting |
| Tech flat | Flat technical drawing of the garment |
| Spec sheet | Measurements and construction details |
| 3D | Interactive 3D model of the assembled garment, with fabric textures and studio lighting (built with three.js) |

## Export

- **PDF 1:1:** true-scale vector PDF
  - Tiled on A4, US Letter or A0, with a cover page, printing instructions, a page map, labelled pages (A1, A2, B1…), corner crosses and trim lines for taping
  - Or full size on one sheet, for a plotter or print shop
  - Includes a **10 × 10 cm calibration square**, on the cover and next to the pieces
- **SVG:** vector pattern with the calibration square
- **DXF:** for CAD, plotters and cutters (saved as `.dxf.txt`; rename to `.dxf`)
- **CSV:** cutting and measurement data

### Printing at true scale

1. Print at **Actual size / 100 %**, and turn off "Fit to page".
2. Measure the calibration square. It must be exactly 10 cm × 10 cm.
3. Only cut once the square measures correctly.

## Getting started

1. Open the HTML file in a modern browser (Chrome, Edge, Firefox or Safari).
2. Choose a garment on the launcher.
3. Choose a size chart and size, or enter your own measurements.
4. Adjust design, fit, fabric and seam allowance settings.
5. Review the views, then export.

## Tech

- Plain HTML, CSS and JavaScript in one self-contained file
- three.js for the 3D view
- Soft neumorphic cream-and-teal UI (Plus Jakarta Sans)

## Related apps

- **Daedalus Leather Goods:** pattern drafter for bags, wallets, card holders and belts
- **Daedalus Footwear Lab:** sneaker pattern drafter

## Author

Steffan Mendis
