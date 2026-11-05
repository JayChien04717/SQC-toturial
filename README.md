# SQC-toturial

A learning guide to superconducting quantum circuits: paper discussions, chip design with Qiskit Metal, and quantum simulations with QuTiP.

The course provides official learning resources and exercises. Students learn the tools from the official documentation and develop their own implementations.

## Learning tracks

| Track | Topics | Start here |
|---|---|---|
| Paper reading | Research questions, models, key figures, and discussion; content prepared by the instructor | [Paper reading](01_paper_reading/README.md) |
| Chip design | One TransmonCross system: EC/h = 250 MHz, f01 = 4 GHz, fr = 6 GHz, and loaded linewidth = 2 MHz | [Chip design](02_chip_design/README.md) |
| Quantum simulation | Spectrum, ZZ strength, and time-domain pulses | [QuTiP](03_qutip/README.md) |

## Learning sequence

1. Complete the official installation and introductory tutorials listed in [Preparation](00_setup/README.md).
2. Discuss an instructor-selected paper using the [Paper discussion template](01_paper_reading/paper_template.md).
3. Build a TransmonCross system with a readout resonator, charge line, and CPW feedline. Use the same design through the Metal exercises: layout → EC → eigenmodes → linewidth.
4. Work through the QuTiP exercises: spectrum → ZZ → pulses.

## Suggested schedule

| Session | Topic | Focus |
|---|---|---|
| 1 | Paper reading and prerequisites | Research question, notation, and assumptions |
| 2 | Metal layout | Components, dimensions, and routing |
| 3 | Capacitance and EC | Nodes, boundary conditions, and convergence |
| 4 | Eigenmodes | Field patterns, mode identification, and frequency |
| 5 | S21 and linewidth | Complex data, fitting, and uncertainty |
| 6 | Spectrum and ZZ | Energy levels, state labels, and conditional shifts |
| 7 | Time-domain pulses | Calibration, populations, and leakage |

Allow roughly 2–3 hours per session, plus independent study and electromagnetic solve time. Adjust the pace to the students' background.

## Folders

- `00_setup`: prerequisites, official starting points, and units.
- `01_paper_reading`: instructor-editable discussion and figure reproduction templates.
- `02_chip_design`: four Metal and electromagnetic simulation exercises.
- `03_qutip`: three quantum simulation exercises.
- `references`: official resource index.

The existing thesis PDF remains in the root folder. No thesis summary or chapter selection has been prepared. Official links were checked on November 4, 2026; record the versions used when following them.
