# SQC-toturial

A learning guide to superconducting quantum circuits covering paper discussions, chip design with Qiskit Metal, numerical simulation with QuTiP and scqubits, and qubit measurements with QICK.

The course provides official learning resources and exercises. Students learn the tools from the official documentation and develop their own implementations.

## Learning tracks

| Track | Topics | Start here |
|---|---|---|
| Paper reading | Research questions, models, key figures, and discussion; content prepared by the instructor | [Paper reading](01_paper_reading/README.md) |
| Chip design | One TransmonCross system: EC/h = 250 MHz, f01 = 4 GHz, fr = 6 GHz, and loaded linewidth = 2 MHz | [Chip design](02_chip_design/README.md) |
| Numerical simulation | Transmon and fluxonium spectra, charge and phase matrix elements, ZZ strength, and time-domain pulses | [Numerical simulation](03_numerical_simulation/README.md) |
| Qubit measurement | FPGA pulse control, readout acquisition, and lab scripts | [QICK](04_qick/README.md) |

## Learning sequence

1. Complete the official installation and introductory tutorials listed in [Preparation](00_setup/README.md).
2. Read the Engineer's Guide, then Long Nguyen and Leon Ding, following the [recommended reading order](01_paper_reading/README.md).
3. Build a TransmonCross system with a readout resonator, charge line, and CPW feedline. Use the same design through the Metal exercises: layout → EC → eigenmodes → linewidth.
4. Work through the numerical simulation exercises, from transmon and fluxonium spectra to static ZZ and time-domain pulses.
5. Learn how the lab runs pulse sequences and acquires readout data with [FPGA and QICK](04_qick/README.md).

## Suggested schedule

| Session | Topic | Focus |
|---|---|---|
| 1 | Paper reading and prerequisites | Research question, notation, and assumptions |
| 2 | Metal layout | Components, dimensions, and routing |
| 3 | Capacitance and EC | Nodes, boundary conditions, and convergence |
| 4 | Eigenmodes | Field patterns, mode identification, and frequency |
| 5 | S21 and linewidth | Complex data, fitting, and uncertainty |
| 6 | Transmon and fluxonium spectra, and ZZ | Flux sweeps, matrix elements, and conditional shifts |
| 7 | Time-domain pulses | Calibration, populations, and leakage |

Allow roughly 2–3 hours per session, plus independent study and electromagnetic solve time. Adjust the pace to the students' background.

## Folders

- `00_setup`: prerequisites, official starting points, and units.
- `01_paper_reading`: three readings, a recommended reading order, and discussion templates.
- `02_chip_design`: four Metal and electromagnetic simulation exercises.
- `03_numerical_simulation`: four simulation exercises using QuTiP and scqubits.
- `04_qick`: FPGA measurement basics, official QICK demos, and lab scripts.
- `references`: official resource index.

Official software links were checked on November 4, 2026. Record the versions used when following them.
