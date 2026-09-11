# Training Table Run Configurator

Build 2026.09.11‑5

A single-page configurator for daisy-chained power on training-table runs. Lay out one or more runs of tables, and the app draws the layout (plan or isometric), routes the trunk with real cord lengths, enforces the run limit, and produces a bill of materials.

## Parts

| Part | Description | Quantity rule |
| --- | --- | --- |
| 5CDDCSTART | Starter cord: NEMA 5‑15P, 70.9 in 14 AWG, inline module with RESET breaker and one 5‑15R, 3.9 in tail to GST female | 1 per run (one trunk) |
| 5CDDCCONN | GST connector, 4‑port: trunk in/out below, two clamp‑socket outputs above; mounted to the underside on the spine | 1 per surface (straight run) · 1 per pair (face to face) |
| 5CDDCEXT | GST extension, 70.9 in, male ↔ female | positions − 1 per run |
| 5CDPWR2WH‑GST | Clamp socket: 2 × TR 5‑15R, USB‑A, USB‑C 65 W, 70.9 in lead with GST male | 1 per surface |

## Rules built in

- Cord run per trunk = 70.9 in + 3.9 in (starter) + 70.9 in per extension. Maximum 614 in (15.6 m) and 8 surfaces per run — the table counter stops there.
- One 15 A / 120 V circuit per run, behind the starter's RESET breaker. The starter plugs into a wall outlet only.
- Cords route straight along the underside spine; slack is coiled at true length and reported in the legend.
- Face to face: two mirrored rows sharing the socket edge on one trunk (paired connectors). A 0 in aisle between runs also puts them face to face, each with its own trunk.
- Runs stack away from the wall corner: Run 1 is at the bottom of the drawing.

## Using it

- **Feed** — which end the wall feed enters from. **Socket** — clamp position on the back edge, from the seated user's view (default Right).
- **Runs** — add runs; per run set surfaces (1–8), surface size, straight run or face to face, table spacing, aisle width to the next run (0 = face to face with its own trunk) and distance to the wall. All measurements are inches.
- **Plan / Isometric** — scroll to zoom, drag to pan, Fit to reset.
- **New / Save / Load / Undo / Redo** — Save downloads a JSON layout; Load restores one.
- **Bill of materials** — totals plus a per‑run breakdown; copy to clipboard or download the CSV spreadsheet.

