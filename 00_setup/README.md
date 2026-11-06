# 00 | Preparation

## Prerequisites

Students should understand basic linear algebra, LC circuits, quantum states and operators, complex data, and basic programming. Use the official documentation to resolve installation issues and keep track of versions and error messages.

## Official starting points

- [Qiskit Metal / Quantum Metal](https://qiskit-community.github.io/qiskit-metal/): start with Get Started → Installing and Choose Your Path.
- [Metal tutorials](https://qiskit-community.github.io/qiskit-metal/tut/): complete Part 1, then study components, pins, and routing in Part 2.
- [QuTiP documentation](https://qutip.readthedocs.io/en/stable/): start with Installation and the Users Guide.
- For superconducting circuit models and flux sweeps, start with Install, Basics, and Single-Qubit Parameter Sweep. [scqubits documentation](https://scqubits.readthedocs.io/en/latest/)
- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): learn Qobj, states, operators, expectation values, and eigenstates.
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): learn composite operators and subsystem ordering.

## Preparation exercise P0

1. Set up the environment using the official instructions. Identify the OS, package versions, and available solvers.
2. Complete one official Metal introductory example. Identify a component, a pin, and a geometry parameter.
3. Complete one official QuTiP basic example. Explain the difference between a state, an operator, and an expectation value.
4. Check whether Q3D / HFSS licenses are available, or ask the instructor which alternative solver to use.
5. Read the [Units and conventions](units.md). Identify two unit conversions that require care.

Discussion: explain what each introductory example does and how you checked that it worked.

## Tool roles

Metal handles geometry and connections to analysis tools. Electrostatic and full-wave calculations require suitable solvers. QuTiP handles Hamiltonians and dynamics. scqubits provides circuit models for spectra, parameter sweeps, and matrix elements. Students without electromagnetic solver access can start with the numerical simulation exercises.

Choose compatible versions and renderers using the official documentation and the laboratory's available environment.
