# ATLAS Estimating — Android with ACT Ceiling Takeoff (prototype v2.5)

This complete folder contains the previous ATLAS DXF wall takeoff, plus an independently saved ceiling takeoff overlay. Keep all files together; do not mix them with a separate iPad repository.

## Try it
1. Open index.html on Windows, or host the whole folder over HTTPS and open android.html in Android Chrome.
2. Open a DXF, verify its units and/or calibrate using a known dimension. Wrong scale means wrong ceiling material counts.
3. Tap CEILING ▦ then + NEW CEILING AREA. Tap at least 3 corners around the ceiling boundary (each tap creates a vertex). Tap CLOSE CEILING.
4. Set 2×2 or 2×4, rotation, X/Y offset, and waste percentage. Live blue and orange grid lines appear within the area. Move X/Y by 6 inches using the buttons, and zoom for border cuts. Purple dots show estimated hangers.
5. Add additional ceiling areas. They persist in Save Project / Open Saved and in the downloaded project backup. Use Ceiling CSV for an independent report.
6. To reopen the ceiling controls, press CEILING ▦.

## What counts mean
- Area SF and perimeter LF follow the polygon exactly.
- Tiles: each grid position that touches the polygon counts as a tile; full and cut positions are separated. Cut-tile reuse is not optimized. Waste is applied to the number of touched tiles.
- Typical grid assumption: main runners 4 ft on center, 4 ft cross tee lines every 2 ft, and for 2×2 tiles extra 2 ft tee lines midway between mains.
- Main runners are estimated as 12 ft pieces, wall angle as 10 ft pieces, 4 ft / 2 ft tees by clipped line length, with a separately applied waste factor. Actual tee connector counts and cut reuse can differ.
- Wire points are a *conceptual* maximum 4 ft spacing along each main run, including ends, not a code-compliant hanger layout. Add independent support for lights/HVAC and follow manufacturer/seismic/inspection requirements.
- This first version handles the polygon boundary; it does not subtract columns, soffit holes, lights, penetrations, or use manufacturer-specific hanger/grid rules.
- Calibration or unit changes update the displayed quantities based on current drawing scale. Recheck the results after any scale change.

## Notes
This is a field estimating prototype, **not** a verified construction assembly design. Compare against reflected ceiling plans and product requirements before ordering. Projects with ceiling regions remain backwards-compatible with projects saved before ceilings were introduced.
