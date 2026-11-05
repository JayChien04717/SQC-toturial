# 03 | Quantum Simulation with QuTiP

Learn the tools from the official documentation and build your own models. These exercises define questions and teaching parameters.

## Shared reading

1. [Basic Operations on Quantum Objects](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): Qobj, states, operators, eigenstates, and expectation values.
2. [Tensor Products and Partial Traces](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): composite Hilbert spaces.
3. [Lindblad Master Equation Solver](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html): closed and open system dynamics.
4. [Time-dependent Hamiltonians](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-time.html): pulses and time-dependent coefficients.

| Exercise | Goal |
|---|---|
| [Q1: Spectrum](01_spectrum.md) | Build a Hamiltonian, identify levels, and understand avoided crossings |
| [Q2: ZZ strength](02_zz_strength.md) | Calculate conditional shifts, label dressed states, and test approximations |
| [Q3: Time-domain pulses](03_time_domain_pulse.md) | Observe Rabi oscillations, calibrate pulses, and study leakage and dissipation |

Start with a weakly anharmonic transmon model. If a paper uses fluxonium or another device, choose an appropriate Hamiltonian and basis.

For each calculation, understand the equations, parameters, units, initial state, basis, truncation, and numerical settings. The initial QuTiP parameters are independent teaching assumptions. When modeling the Metal design, replace them consistently with extracted device parameters.
