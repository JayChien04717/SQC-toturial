# Q3 | Static ZZ Strength

Complete Q1 and use the same model and parameters.

## Where to learn

- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): eigenstates, overlaps, and expectation values.
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): composite bases and operators.
- [QuTiP Master Equation Guide](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html): dynamics for the extension exercise.

These resources teach the tools. You must combine them to build the ZZ model and label the relevant states.

## What Is Static ZZ?

Static ZZ is the change in one qubit's transition frequency when the other qubit switches from $|0\rangle$ to $|1\rangle$. For example, qubit 2 has transition frequency $(E_{01}-E_{00})/h$ when qubit 1 is in $|0\rangle$ and $(E_{11}-E_{10})/h$ when it is in $|1\rangle$. Their difference defines the signed ZZ strength.

$$
\zeta = \frac{E_{11}-E_{10}-E_{01}+E_{00}}{h}.
$$

Express $\zeta$ in MHz. Each $E_{ij}$ is the dressed energy associated with bare $|ij\rangle$. In the effective diagonal two-qubit Hamiltonian, the interaction term in $H/h$ is $(\zeta/4)Z\otimes Z$, with $Z|0\rangle=|0\rangle$ and $Z|1\rangle=-|1\rangle$. Residual static ZZ causes an unwanted conditional phase to accumulate while the qubits idle.

## FTF Reference

The fluxonium–transmon–fluxonium (FTF) architecture couples two fluxonium qubits through a tunable transmon. Read §5.1.2 and Figs. 5-1 and 5-3 for the device layout, how the coupler helps suppress static ZZ, and a comparison of measured and simulated ZZ versus coupler flux. [Leon Ding's thesis, Chapter 5](<../01_paper_reading/ding-leonding-phd-physics-2023-thesis (1).pdf>)

## Exercises

1. Define a consistent assignment rule for the four states, avoiding assigning one eigenstate to two labels.
2. Sweep f2 and plot ζ alongside the four dressed-state overlaps.
3. Identify strong |11〉–|20〉 or |11〉–|02〉 mixing. Explain where a computational-state ZZ interpretation becomes unreliable.
4. Compare g = 0, 10, and 20 MHz, and discuss trends at a dispersive operating point.
5. Compare N = 2, 3, 4, and 5. Explain the role of higher levels and model limitations.
6. At a weakly mixed operating point, relate ζ to the effective Z⊗Z coefficient and conditional frequency shift. Define the Z and 2π conventions.

## Extension

Perform conditional Ramsey evolution for two control-qubit initial states. Estimate ZZ from the phase evolution and compare it with the energy-difference method. If exchange dynamics remain significant, explain how they affect the interpretation.

## Learning checks and discussion

Test zero coupling and truncation convergence. Do not identify E11 solely by its sorted energy index.

If ζ suddenly jumps, how can you distinguish a physical feature from label switching or a numerical problem?
