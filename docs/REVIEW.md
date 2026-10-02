# Repository review

## Confirmed from the supplied materials

- Six exercise folders, two FluidSIM `.ct` files, four complete STEP 7 project directories, two Factory I/O scenes, four OB1 ladder PDFs, one report, and one question paper.
- Report authorship line: Ali Ramezanzadeh. Course: Industrial Control. Institution named in the report: Amirkabir University of Technology. Date: Aban 1403.
- The author confirmed individual work and the two-FluidSIM/four-PLC split.
- The report's six topics agree with the two-pneumatic/four-PLC file grouping.
- STEP 7 metadata records V5.6 + SP2, and Factory I/O scene headers record 2.5.2.
- Four PLC exports contain 10, 11, 18, and 23 OB1 networks respectively.

## Remaining factual details

- Identify which scenes, hardware configurations, or code were supplied as course starter material.
- Confirm FluidSIM version and the PLC simulator and connection driver.
- Confirm the inferred scene-to-project pairing by opening the projects and scenes.
- Supply the videos referenced by the report if available.
- The author plans to supply the PLC question 1 traffic-light scene; it is not yet present in this package.
- Confirm whether the exam paper and course-provided scene files may be shared publicly. Original documents are included only in this local review draft.

## Technical verification still needed

- All six simulations need actual execution checks.
- Exercise 04: confirm whether ID30 is a measured height signal, an emitter/category value, or another signal. The report records 128/192/224, while the original assignment asks for height classification. Avoid claiming height measurement until this is resolved.
- Exercises 04/05: confirm Stop polarity and the intended orderly-stop behavior; do not call normal Stop an emergency stop.
- Exercise 06: confirm actual analog module conversion and output encoding, as well as the comparison boundaries between temperature bands. Numeric valve-current commands in documentation alone do not establish a physical 4-20 mA output.
- Exercise 03: the supplied exercise intentionally specifies three light stages; the report's suggested fourth stage is commentary, not an implemented feature.

## Preparation decisions

One repository groups this single take-home exam and its six related exercises. Native STEP 7 companion files, including existing lock/metadata files, are retained to preserve the received project layout. Only the redundant FluidSIM `.bak` was left out of the curated copy. The source archive remains unchanged.

No simulation code was rewritten, no results were invented, and no public repository was created during preparation.
