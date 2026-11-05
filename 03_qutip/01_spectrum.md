# Q1 | Spectrum and Avoided Crossings

## Where to learn

- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): eigenenergies, eigenstates, and state projections.
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): composite systems.
- Extension: [Metal Transmon Analytics](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.32-Transmon-analytics-HCPB.html), connecting circuit models and energy levels.

## Teaching model and parameters

Use two Duffing transmons with exchange coupling under the rotating-wave approximation. Write and explain the Hamiltonian yourself.

- f1 = 5.0 GHz; sweep f2 from 4.4 to 5.7 GHz using at least 201 points.
- alpha1 = −0.25 GHz; alpha2 = −0.28 GHz.
- The exchange coefficient in H/h is g = 0.020 GHz.
- Begin with four levels per transmon and test other truncations.

## Exercises

1. Calculate the low-energy levels and transition frequencies of one transmon to check the parameter definitions.
2. Construct the two-transmon Hilbert space, sweep f2, and plot low energies relative to the ground state.
3. Identify the single-excitation avoided crossing and compare g = 0, 10, and 20 MHz.
4. Use bare-state overlaps to explain mode mixing. Distinguish energy ordering from labels based on state character.
5. Compare N = 3, 4, and 5 levels per subsystem for the energies of interest. Explain the scope of convergence.
6. Choose a drive operator and discuss bright and dark transitions. Optionally calculate transition matrix elements.

## Learning checks and discussion

The g = 0 limit should recover independent systems. Check unit conversions, state character, and truncation before interpreting the spectrum.

How does an eigenenergy diagram differ from an experimental absorption spectrum? Does every energy difference imply an observable peak?
