## Where to Learn

1. [4.03 Impedance, admittance and scattering](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.03-Impedance.html): driven simulations, ports, and frequency sweeps.
2. [4.17 S21 simulation and fitting](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.17-Fit-S21-of-Hanger-Resonator-Geometry.html): hanger-resonator transmission and complex S21 fitting.

## Exercises

Using the system from **01_layout.md** with the frequencies tuned in **03_eigenmode.md**, tune the **loaded readout-resonator linewidth to 2 MHz**.

1. Define the feedline ports and charge-line termination, then simulate S21 around the 6 GHz readout resonance.
2. Fit the complex S21 response to extract resonance frequency, loaded linewidth, and quality factor. Define linewidth as the isolated-mode power-Lorentzian FWHM parameter of the fitting model.
3. Adjust the resonator–feedline coupling gap or coupling length to reach a linewidth of 2 MHz.
4. Check frequency-sweep resolution, mesh convergence, and fitting residuals.
5. Verify that the tuned system retains the 6 GHz resonator frequency, 4 GHz transmon transition, and EC/h = 250 MHz. Retune as needed.
