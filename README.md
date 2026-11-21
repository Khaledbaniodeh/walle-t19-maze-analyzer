# WALL·E T19 — Maze Analyzer

[**Open the Maze Analyzer (GitHub Pages)**](https://khaledbaniodeh.github.io/walle-t19-maze-analyzer/)

A standalone, browser-based Micromouse simulation log analyzer developed as a supplementary visualization and debugging tool for **WALL·E · Team T19**, ENCS4380 Interfacing Techniques, Birzeit University.

## What it does

- Visualizes discovered maze walls, confirmed-open passages, and unknown sides from HAL map dumps.
- Displays **Explore, Return and Race** routes and recorded movement replay.
- Inspects individual cells and changes between map snapshots.
- Compares discovered walls with a reference MMS ASCII maze, highlighting conflicts and mismatches.
- Checks the integrity of `@MAP / @C / @END` dumps, including CRC.
- Exports visualizations and an analysis report.
- Includes a **Try demo run** option with clearly identified *synthetic* data.

## How to use

1. [Open the website](https://khaledbaniodeh.github.io/walle-t19-maze-analyzer/).
2. Click **Try demo run** to explore the interface without a log, or load an MMS run log as `.txt` or `.log` (pasting text also works).
3. Switch between Explore, Return, and Race to inspect phases and recorded paths.
4. Optionally import the matching MMS maze `.txt` and `.goal` files to compare your discovered map against the reference.
5. Use **Export** for an image or Markdown analysis report.

**Important:** A real log needs `@MAP`, `@C`, and `@END` records for discovered-map visualization. A log containing only movement messages may still show its recorded route. Missing data is never fabricated.

## Local development & deployment

Everything is contained in `index.html`: no build, dependencies, backend or accounts required. You can open it directly in a browser or host it as a static site.

To publish or maintain the live URL, use GitHub **Settings → Pages → Deploy from a branch → main → /(root)**.

- The analyzer runs locally in your browser; imported logs are not sent to a server.
- The app itself is publicly available, but robot firmware and the main course repository are **not published here**.
- This is an **optional supporting tool**, not the WALL·E solver itself.
- The **Try demo run** displays synthetic data; do not treat it as an actual robot test.
- Actual MMS runs containing map dumps should be tested before presenting results.

## Main robotics project

[WALL·E T19 — Micromouse Robotics](https://github.com/Khaledbaniodeh/micromouse-robotics) — private GitHub repository (accessible only to approved collaborators).

## Team

**Team T19 · Birzeit University · ENCS4380**

Jibreel Haddar · Khaled Bani Oudeh · Mohammad Khaleel · Waad Melhem
