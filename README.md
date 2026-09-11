# Training Table Run Configurator

A single-page, offline configurator for daisy-chained power on training-table runs. Lay out one or more runs of 24 × 60 in surfaces, and the app draws the run (plan or isometric), routes the trunk with real cord lengths, and produces a bill of materials.

Live: open `index.html` (GitHub Pages serves it at the repository URL).

## Parts

| Part | Description | Quantity rule |
| --- | --- | --- |
| 5CDDCSTART | Starter cord: NEMA 5‑15P, 70.9 in 14 AWG, inline module with RESET breaker and one 5‑15R, 3.9 in tail to GST female | 1 per trunk |
| 5CDDCCONN | 3‑way GST connector, 1 male in / 2 female out, mounted to the underside on the centre spine | 1 per table |
| 5CDDCEXT | GST extension, 70.9 in, male ↔ female | tables − 1 per trunk |
| 5CDPWR2WH‑GST | Clamp socket: 2 × TR 5‑15R, USB‑A, USB‑C 65 W, 70.9 in lead with GST male | 1 per table |

## Rules built in

- Cord run per trunk = 70.9 in + 3.9 in (starter) + 70.9 in per extension. Maximum run 614 in (15.6 m) → up to 8 tables per trunk.
- One 15 A / 120 V circuit per trunk, behind the starter's RESET breaker. The starter plugs into a wall outlet only.
- Cords route orthogonally along the underside spine; slack is coiled and its length is reported in the legend.
- A face‑to‑face run is two mirrored rows meeting at the socket edge, each with its own starter and trunk.

## Using it

- **Runs** — add runs, set tables per run (1–8), surface size, straight run or face to face, table spacing and aisle width.
- **Feed** — which end the wall feed enters from; **Socket** — clamp position on the back edge.
- **Plan / Isometric** — scroll to zoom, drag to pan, Fit to reset.
- **New / Save / Load / Undo / Redo** — Save downloads a JSON layout; Load restores one.
- **Copy bill of materials** — copies part numbers, quantities and per‑run cord lengths to the clipboard.

## Deploy to GitHub Pages

1. Put `index.html` and this `README.md` in the repository root.
2. Settings → Pages → Deploy from a branch → `main` / root.
3. The app is fully self‑contained (no build step, no external requests).
