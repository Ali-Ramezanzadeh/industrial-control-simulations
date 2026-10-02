# 06. Furnace control and motor changeover

**Tools:** STEP 7

## Objective

Implement the coursework furnace exercise with analog signal conversion, a tabulated valve command, and main/reserve conveyor motors.

## Documented implementation

OB1 contains 23 networks. The report describes a 4-20 mA temperature-transmitter signal corresponding to -100 to 1000 degrees C, FC106/FC105 conversion, integer conversion for comparisons, and temperature-band selection of valve commands. The main motor starts first; the exercise requests reserve-motor activation after a 10 s delay following Stop, and shutdown after another Stop. When both motors are off, the documented command is 4 mA. This is a table-based coursework implementation; the archive contains no identified PID controller or physical furnace test.

## Files

- [native/Q6/Q6.s7p](native/Q6/Q6.s7p): original STEP 7 project entry point. Keep its complete companion folder.
- [ladder-logic.pdf](ladder-logic.pdf): readable original OB1 ladder export.

## Source documentation

[English report translation](../../docs/report-en.md) and [Persian report](../../docs/report-fa.pdf), PDF pages 33-39 (PDF page positions, not printed page numbers). The [English question paper](../../docs/exam-questions-en.md) preserves the assignment requirements. The original native files and ladder exports are preserved; this exercise README is a portfolio summary, not a new implementation.

## Running and checking

See [setup notes](../../docs/SETUP.md). Open `native/Q6/Q6.s7p` with the appropriate software.

Confirm analog input/output scaling and module configuration; test values within each temperature band and at every boundary; inspect the 10 s motor changeover and the inactive-state valve command. Functional verification is pending.

**Verification status:** files inspected; simulation execution and functional results not independently verified.
