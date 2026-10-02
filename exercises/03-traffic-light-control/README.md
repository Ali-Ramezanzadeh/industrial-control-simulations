# 03. Traffic-light sequence

**Tools:** STEP 7

## Objective

Implement the prescribed three-stage repeating traffic-light exercise in ladder logic.

## Documented implementation

OB1 contains 10 networks for Start/Stop memory, indicator outputs, a stage counter, three on-delay timers, and the traffic-light outputs. The prescribed states are green 1/red 2 for 20 s, yellow 1/yellow 2 for 7 s, and red 1/green 2 for 20 s. The original report comments that another yellow stage could be useful, but the supplied implementation follows the three-stage exercise.

## Files

- [native/Q3/Q3.s7p](native/Q3/Q3.s7p): original STEP 7 project entry point. Keep its complete companion folder.
- [ladder-logic.pdf](ladder-logic.pdf): readable original OB1 ladder export.

## Source documentation

[English report translation](../../docs/report-en.md) and [Persian report](../../docs/report-fa.pdf), PDF pages 16-19 (PDF page positions, not printed page numbers). The [English question paper](../../docs/exam-questions-en.md) preserves the assignment requirements. The original native files and ladder exports are preserved; this exercise README is a portfolio summary, not a new implementation.

## Running and checking

See [setup notes](../../docs/SETUP.md). Open `native/Q3/Q3.s7p` with the appropriate software.

Monitor the counter, timers, six lamp outputs, Start, and Stop over several complete cycles. The specified stage durations sum to 47 s; no measured cycle-time result is supplied.

**Verification status:** files inspected; simulation execution and functional results not independently verified.
