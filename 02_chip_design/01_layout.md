## Where to Learn

1. [Single Transmon – Grounded (Xmon)](https://qiskit-community.github.io/qiskit-metal/circuit-examples/A.Qubits/01-Transmon_cross.html): the TransmonCross component.
2. [1.1 Quick start](https://qiskit-community.github.io/qiskit-metal/tut/1-Overview/1.1-Quick-start.html): designs, components, pins, and the GUI.
3. [2.12 Simple Meander](https://qiskit-community.github.io/qiskit-metal/tut/2-From-components-to-chip/2.12-Simple-Meander.html): CPW routing and resonator geometry.
4. [Metal tutorial index](https://qiskit-community.github.io/qiskit-metal/tut/): charge-line, launchpad, and readout-line examples.
5. [3.3 Render to Ansys](https://qiskit-community.github.io/qiskit-metal/tut/3-Renderers/3.3-Render-your-design-to-Ansys.html): transferring geometry to the solver.

## Exercises

Build a single-qubit system using **TransmonCross**. Use this same layout throughout Exercises 02–04.

1. Create the cross-shaped transmon and identify its island, Josephson junction, and surrounding ground.
2. Add a capacitively coupled readout resonator.
3. Add a separate charge-drive line coupled to the transmon.
4. Add a CPW waveguide / feedline coupled to the resonator in a hanger configuration, with input and output interfaces.
5. Check the component connections, coupling gaps, ground continuity, and routing. Identify the ports and terminations needed for later electromagnetic simulations.
