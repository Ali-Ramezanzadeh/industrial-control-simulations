# Industrial Control Simulations

Six industrial-control coursework exercises covering pneumatic sequencing and PLC ladder logic with FluidSIM, Siemens STEP 7, and Factory I/O.

This is individual coursework by Ali Ramezanzadeh. The original Persian report lists the Industrial Control course at Amirkabir University of Technology, Department of Electrical Engineering, in Aban 1403 (2024). This collection preserves the supplied project files and adds English translations, navigation, and technical summaries.

## Exercises

| Exercise | Topic | Environment | Available evidence |
| --- | --- | --- | --- |
| [01](exercises/01-pneumatic-machining/README.md) | Timed clamping, machining, and drilling | FluidSIM | Native circuit, report figure |
| [02](exercises/02-magnetic-part-separation/README.md) | Pneumatic handling of ferrous parts | FluidSIM | Native circuit, report figure |
| [03](exercises/03-traffic-light-control/README.md) | Three-stage traffic-light control | STEP 7 | Native project, 10-network OB1 export |
| [04](exercises/04-box-classification/README.md) | Box classification and counting | STEP 7 + Factory I/O | Native project, scene, 11-network OB1 export |
| [05](exercises/05-palletizing/README.md) | Two-box palletizing | STEP 7 + Factory I/O | Native project, scene, 18-network OB1 export |
| [06](exercises/06-furnace-control/README.md) | Temperature-band valve commands and motor changeover | STEP 7 | Native project, 23-network OB1 export |

The supplied files and report contain **two FluidSIM exercises and four PLC exercises**. Factory I/O scene filenames use local PLC-section numbering: `Q 2.factoryio` corresponds to overall exercise 04 and `Q 3.factoryio` to overall exercise 05. These associations should be confirmed by opening the scenes with their corresponding PLC projects.

## Circuit previews

### Machining sequence

![Machining circuit from the Persian report](exercises/01-pneumatic-machining/preview.png)

### Part separation

![Part-separation circuit from the Persian report](exercises/02-magnetic-part-separation/preview.png)

## Inspecting and running

Start with the exercise summaries and readable ladder PDFs. To edit or simulate the native projects, see [setup notes](docs/SETUP.md).

| Environment | Version evidence in supplied files |
| --- | --- |
| FluidSIM | Exact version not established |
| Siemens STEP 7 | Project metadata records STEP 7 Professional 2017 SR2, V5.6 + SP2 |
| Factory I/O | Both scene headers record version 2.5.2 |
| PLC target | Ladder export headers identify SIMATIC S7-300 CPU 313C |

These are recorded versions and project targets, not a tested compatibility matrix. No physical PLC or machine test is documented here.

## Documentation and provenance

- [English report translation](docs/report-en.md), including network explanations, source figures, and I/O tables.
- [English exam-question translation](docs/exam-questions-en.md), including all six question statements and the furnace-current table.
- [Original Persian report](docs/report-fa.pdf), 39 PDF pages.
- [Original Persian exam questions](docs/exam-questions-fa.pdf), 9 PDF pages.
- [Review and verification notes](docs/REVIEW.md).
- [Attribution](ATTRIBUTION.md).
- [File manifest](docs/file-manifest.json), recording original paths, new paths, and SHA-256 hashes for copied source files.

English translations retain source technical details and identify ambiguous or inconsistent source statements in separate translation notes. Original circuit and ladder screenshots are reproduced with English captions. They are not new simulation outputs.

## Verification status

The archive, report, ladder exports, and available software metadata were inspected. Copied original files were checked for byte-for-byte integrity. The simulations have **not** been independently run. Proposed functional checks are listed in each exercise folder.

The report refers to demonstration videos, but no video files were present in the supplied archive. No performance, reliability, or hardware-validation claim is inferred from the screenshots.

## Publication status

This is a local repository draft. The author has confirmed that the work was individual. The provenance of any starter assets remains to be confirmed. The original exam and any course-provided scenes should be checked for public-sharing permission before uploading them. No open-source license has been assigned to the collection.
