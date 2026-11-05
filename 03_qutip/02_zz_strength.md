# Q2 | Static ZZ Strength

Complete Q1 and use the same model and parameters.

## Where to learn

- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html): eigenstates, overlaps, and expectation values.
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html): composite bases and operators.
- [QuTiP Master Equation Guide](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html): dynamics for the extension exercise.

These resources teach the tools. You must combine them to build the ZZ model and label the relevant states.

## Definition

Use ζ = (E11 − E10 − E01 + E00)/h and express it in MHz. Eij denotes the dressed energy associated with bare |ij〉. Establishing that association is part of the exercise.

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
