## Where to Learn

1. [4.01 Capacitance matrix and LOM analysis](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.01-Capacitance-and-LOM.html): capacitance extraction and lumped-element modeling.
2. [4.32 Transmon Analytics](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.32-Transmon-analytics-HCPB.html): charging energy and transmon parameters.

## Exercises

Using the layout from **01_layout.md**, tune the transmon charging energy to **EC/h = 250 MHz**.

1. Extract the capacitance matrix for the single-qubit system. Identify the nodes, reference ground, matrix convention, and units.
2. Determine the effective qubit capacitance, accounting for the readout resonator, charge line, and feedline with appropriate boundary conditions.
3. Vary the TransmonCross dimensions or gaps to reach the target charging energy.
4. Re-extract the capacitance of the tuned layout and check numerical convergence.
5. Keep the updated layout for the frequency-tuning exercise in **03_eigenmode.md**.
