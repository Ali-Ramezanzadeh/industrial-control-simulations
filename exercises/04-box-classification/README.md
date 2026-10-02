# 04. Box classification and counting

**Tools:** STEP 7 + Factory I/O

## Objective

Classify boxes into Palletizing Box, Box(M), and Box(L) categories, actuate pushers, and display counts.

## Documented implementation

OB1 contains 11 networks covering Start/Stop memory, conveyor control, button indicators, three classification paths, delayed pusher activation, and resettable counters. The report records numeric values 128, 192, and 224 for the three categories and the ladder export compares ID30. The assignment describes height-based sorting; the physical meaning and driver mapping of this numeric input need confirmation before claiming independent height measurement. The supplied scene is Q 2.factoryio, which uses PLC-section numbering.

## Files

- [native/Q4/Q4.s7p](native/Q4/Q4.s7p): original STEP 7 project entry point. Keep its complete companion folder.
- [ladder-logic.pdf](ladder-logic.pdf): readable original OB1 ladder export.
- [Factory I/O scene](scene/Q%202.factoryio): original scene, inferred association from assignment numbering and exercise content.

## Source documentation

[English report translation](../../docs/report-en.md) and [Persian report](../../docs/report-fa.pdf), PDF pages 20-25 (PDF page positions, not printed page numbers). The [English question paper](../../docs/exam-questions-en.md) preserves the assignment requirements. The original native files and ladder exports are preserved; this exercise README is a portfolio summary, not a new implementation.

## Running and checking

See [setup notes](../../docs/SETUP.md). Open `native/Q4/Q4.s7p` with the appropriate software.

Confirm the scene input mapped to ID30, test all three categories and counter reset, and check Stop during pusher operation. The report describes an orderly stop that can allow the current handling action to finish.

**Verification status:** files inspected; simulation execution and functional results not independently verified.
