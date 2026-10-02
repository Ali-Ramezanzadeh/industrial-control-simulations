# Setup notes

## Software evidence

The native STEP 7 projects record `STEP 7 Professional 2017 SR2`, `V5.6 + SP2`. The ladder PDFs identify `SIMATIC 300` / `CPU 313C`. The Factory I/O scene headers record `2.5.2`. The FluidSIM version, PLC simulation tool, and PLC/Factory I/O connection driver are not established from the supplied files.

## FluidSIM exercises

Open the `.ct` file in each exercise's `native/` directory using a compatible FluidSIM installation. Review the circuit against the report, confirm initial actuator positions, and use its Start control to observe the documented sequence. Record the software version and outcomes when verifying it.

## STEP 7 exercises

Keep each complete `native/Qn/` directory together. Open its `Qn.s7p` project entry in SIMATIC Manager. Inspect the configured station, OB1, symbols, and hardware configuration. The included ladder PDF supports read-only review without STEP 7.

The STEP 7 companion database and metadata files are retained without renaming or pruning. The small `.s7p` file alone is not the full supplied project. Simulator configuration and download/run steps need to be documented from the author's working environment.

## Factory I/O exercises

The original exam places saved scenes under `Documents/Factory IO/My Scenes`; use that location if required by the installation, or its supported scene-opening workflow. The `Q 2.factoryio` scene is associated with exercise 04, and `Q 3.factoryio` with exercise 05, based on assignment numbering.

Before running, identify the PLC connection driver, confirm the input/output address map against the corresponding project, and verify the Stop input polarity. The original exam notes that its Factory I/O Stop input is normally 1 and changes to 0 when pressed. Do not assume a fresh installation already has the matching connection settings.

## Record a reproducible verification

For each exercise, record software versions, simulator/driver configuration, initial conditions, the inputs applied, expected behavior, observed behavior, and any discrepancies. Attach a short video or screenshots after actual execution. No execution outcome is supplied by this repository preparation.
