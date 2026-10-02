# 05. Two-box palletizing sequence

**Tools:** STEP 7 + Factory I/O

## Objective

Coordinate conveyors and a pick-and-place mechanism to load two boxes onto each pallet.

## Documented implementation

OB1 contains 18 networks for Start/Stop/reset controls, pallet and box sensing, conveyor memory, box/cycle/rotation counters, X/Z movement, gripping, clockwise/counterclockwise rotation, and a count display. The supplied scene is Q 3.factoryio, using PLC-section numbering. A separate Force stop input is visible in the ladder export.

## Files

- [native/Q5/Q5.s7p](native/Q5/Q5.s7p): original STEP 7 project entry point. Keep its complete companion folder.
- [ladder-logic.pdf](ladder-logic.pdf): readable original OB1 ladder export.
- [Factory I/O scene](scene/Q%203.factoryio): original scene, inferred association from assignment numbering and exercise content.

## Source documentation

[English report translation](../../docs/report-en.md) and [Persian report](../../docs/report-fa.pdf), PDF pages 26-32 (PDF page positions, not printed page numbers). The [English question paper](../../docs/exam-questions-en.md) preserves the assignment requirements. The original native files and ladder exports are preserved; this exercise README is a portfolio summary, not a new implementation.

## Running and checking

See [setup notes](../../docs/SETUP.md). Open `native/Q5/Q5.s7p` with the appropriate software.

Observe at least two complete pallets, confirm two boxes per pallet and the displayed count, test counter reset, and check normal Stop and Force stop. PLC/scene communication settings need confirmation.

**Verification status:** files inspected; simulation execution and functional results not independently verified.
