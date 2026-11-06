# 01 | Paper Reading

## Recommended Reading Order

Start with selected sections of the Engineer's Guide for the basic concepts. Read Long Nguyen first among the two experimental theses, then move on to Leon Ding. If you already know the basics of qubit control and readout, start directly with Long.

### 1. A Quantum Engineer's Guide to Superconducting Qubits

Use the review to answer three questions about a superconducting qubit. [Read the Engineer's Guide (PDF)](1904.06560v5.pdf)

- **What is a qubit?** Read §II.A to see how Josephson nonlinearity produces unequal level spacings and lets us address the two lowest states. Skim §II.B.2 for the contrast between transmon and fluxonium circuits.
- **What should we measure?** Identify the transition frequency and anharmonicity for selective control, the drive strength for pulse calibration, and the relaxation and coherence times that limit experiments. Read §III.B and Fig. 5 for the distinction between energy relaxation $T_1$, Ramsey decay, and echo decay.
- **How do we measure it?** Read §IV.D for microwave control and §§V.A–B for dispersive readout. Follow Fig. 13 from pulse envelope to qubit drive, then Figs. 19 and 22 from the resonator response to the measured I/Q signal.

### 2. Long Bao Nguyen, Toward the Fluxonium Quantum Processor

Start with §6.5.2 and Figs. 6.27–6.30. Each example pairs a pulse sequence with measured data. Follow which pulse prepares the state, which variable is swept, and what the fit reveals. In Fig. 6.27, the Rabi scan varies the qubit pulse width and measures the readout phase. The next three figures show how Ramsey fringes, relaxation, and echo give different information about the qubit. [Read Long's thesis (PDF)](LongNguyen_thesis_final.pdf)

Use Fig. 6.25 for a two-tone spectrum and §5.3 for the microwave control and readout hardware. For a bridge to two-qubit gates, skim §6.4.5 and Fig. 6.20, which show driven transitions used in a microwave-activated CZ experiment.

### 3. Leon Ding, Novel Gates with Superconducting Fluxonium Qubits

Read Chapter 5 for the MIT experiment on two fluxonium qubits coupled through a tunable transmon. Start with Fig. 5-1 for the circuit and gate principle, then read §5.1.2 and Fig. 5-3 to see how the design suppresses static ZZ and how the measured interaction compares with simulation. [Read Ding's thesis (PDF)](<ding-leonding-phd-physics-2023-thesis (1).pdf>)

Continue with §5.3.2 and Figs. 5-7–5-9. Follow the progression from spectroscopy to driven oscillations and CZ calibration. Fig. 5-9 shows how leakage, conditional phase, and single-qubit phases are calibrated separately. Read §5.3.3 and Fig. 5-10 for the interleaved randomized benchmarking results.

## Suggested approach

1. Copy [paper_template.md](paper_template.md) for each topic and fill in the research question, main conclusions, and supporting evidence.
2. Focus each discussion on one model or one to two figures.
3. Use the optional [Figure reproduction notes](figure_reproduction_template.md) to distinguish author data, digitized data, and independent simulations.
4. Explain the chain “assumptions → equations → figures → testable predictions,” then connect it to a Metal or QuTiP exercise.

## Discussion checks

Can students identify the source of each key number, explain the approximations, and distinguish quantities obtained from electromagnetics from those requiring nonlinear quantum models or experiments?

If a figure cannot be reproduced, identify the missing parameters or data rather than inventing values.
