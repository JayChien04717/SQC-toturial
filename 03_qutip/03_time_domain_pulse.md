# Q3 | Time-Domain Pulses, Leakage, and Dissipation

## Where to learn

- [Lindblad Master Equation Solver](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html): initial states, dynamics, and expectation values.
- [Time-dependent Hamiltonians](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-time.html): time-dependent drives.
- [Solver API](https://qutip.readthedocs.io/en/stable/apidoc/solver.html): tolerances, internal step sizes, and result storage.

## Teaching parameters

Use one transmon with f01 = 5.0 GHz and alpha = −0.25 GHz. Begin with three levels and the initial state |0〉. You may use a rotating frame and RWA, but define the frame, detuning, and drive-amplitude convention.

For the dissipative comparison, use T1 = 30 μs and Tphi = 50 μs. Express time in ns. Derive suitable collapse operators and verify the 0–1 coherence decay convention.

## Exercises

1. Apply a resonant square pulse. Sweep duration or amplitude to observe Rabi oscillations.
2. Use a Gaussian pulse with sigma = 10 ns, center = 40 ns, and simulation interval 0–80 ns. Estimate an initial amplitude and calibrate it with an amplitude sweep.
3. Plot the envelope and P0, P1, and P2. Compare maximum transient P2 with residual P2 after the pulse.
4. Compare sigma = 5, 10, and 20 ns. Adapt the time window to contain each pulse and recalibrate each case.
5. Compare ideal evolution with the specified T1 and Tphi. Explain relaxation and pure dephasing separately.
6. Compare N = 3, 4, and 5, then tighten ODE tolerances and maximum step size. Increasing only the plotted sample count is not an integration convergence test.
7. Can the highest final P1 establish full single-qubit gate fidelity? What additional tests are needed?

## Learning checks and discussion

Check population normalization and any nonphysical negative values. Understand the differences among pulse calibration, population transfer, leakage, and gate fidelity.

Extension: use the official documentation to investigate DRAG, Ramsey / echo, or a conditional two-qubit pulse. Explain the additional physics.
