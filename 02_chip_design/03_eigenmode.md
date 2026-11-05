## Where to Learn

1. [4.02 Eigenmode and EPR analysis](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.02-Eigenmode-and-EPR.html): eigenmodes, field distributions, and nonlinear quantization.
2. [4.32 Transmon Analytics](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.32-Transmon-analytics-HCPB.html): estimating transmon transition frequencies.
3. [Metal tutorial index](https://qiskit-community.github.io/qiskit-metal/tut/): sections 4.11–4.13 on tuning a transmon, resonator, and their combined system.

## Exercises

Using the layout from **01_layout.md** and the charging energy from **02_capacitance_ec.md**, tune the **transmon transition frequency to 4 GHz** and the **readout resonator frequency to 6 GHz**.

1. Define the junction inductance and capacitance and run an eigenmode simulation.
2. Identify the qubit-like and resonator-like modes from their field distributions.
3. Tune the junction parameter to obtain a transmon transition frequency f01 of 4 GHz. Use an appropriate circuit or EPR analysis to distinguish f01 from the linear eigenfrequency.
4. Tune the resonator geometry to obtain a resonator frequency of 6 GHz.
5. Check numerical convergence and verify that the combined design retains EC/h = 250 MHz. Iterate if geometry or coupling changes shift the earlier targets.
