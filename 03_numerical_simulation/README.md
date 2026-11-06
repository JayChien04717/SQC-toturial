# 03 | Numerical Simulation

Learn QuTiP and scqubits from their official documentation, then build your own models using the questions and parameters below.

## Simulation Tools

- **QuTiP** provides general tools for building Hamiltonians and simulating time-dependent drives and dissipation. [QuTiP documentation](https://qutip.readthedocs.io/en/stable/)
- **scqubits** provides superconducting circuit models for computing transmon and fluxonium spectra, parameter sweeps, and matrix elements. Use it to cross-check the fluxonium spectrum and charge and phase matrix elements in Q2. [scqubits documentation](https://scqubits.readthedocs.io/en/latest/)

## QuTiP Reading

1. [Basic Operations on Quantum Objects](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): Qobj, states, operators, eigenstates, and expectation values.
2. [Tensor Products and Partial Traces](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): composite Hilbert spaces.
3. [Lindblad Master Equation Solver](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html): closed and open system dynamics.
4. [Time-dependent Hamiltonians](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-time.html): pulses and time-dependent coefficients.

| Exercise | Goal |
|---|---|
| [Q1: Spectrum](01_spectrum.md) | Build a Hamiltonian, identify levels, and understand avoided crossings |
| [Q2: Fluxonium spectrum vs. flux](02_fluxonium_spectrum.md) | Sweep external flux and plot the spectrum and charge and phase transition matrix elements |
| [Q3: ZZ strength](03_zz_strength.md) | Calculate conditional frequency shifts and connect them to the FTF architecture |
| [Q4: Time-domain pulses](04_time_domain_pulse.md) | Observe Rabi oscillations, calibrate pulses, and study leakage and dissipation |

Q1, Q3, and Q4 use weakly anharmonic transmon models. Q2 introduces the fluxonium Hamiltonian and an LC oscillator basis.

For each calculation, understand the equations, parameters, units, initial state, basis, truncation, and numerical settings. The exercise parameters are teaching assumptions. When modeling the Metal design, replace them consistently with extracted device parameters.
