# Solver Preparation and Checks

Start with the official [Render to Ansys tutorial](https://qiskit-community.github.io/qiskit-metal/tut/3-Renderers/3.3-Render-your-design-to-Ansys.html), then follow the resources linked in M2–M4. Learn the implementation from those sources.

## Before solving

- Explain why Q3D, HFSS, or another solver is appropriate and which quantities it can determine.
- Identify Metal, renderer, solver, and OS versions, and check license access.
- Check geometry units, substrate materials, metals, ground connectivity, signal nets, and coupling gaps.
- Explain how junction treatment differs between electrostatic and eigenmode calculations.
- Identify ports, open or short terminations, boundaries, and airbox dimensions.

## After solving

- Keep a reproducible project and the nondefault settings for your own work.
- For capacitance, identify node ordering, matrix convention, reference ground, and units.
- For eigenmodes, inspect frequencies, field patterns, mode labels, and mesh dependence.
- For S21, inspect complex data, sweep settings, calibration, and fitting residuals.
- Diagnose failed convergence checks and decide what to change next.

Discussion: could another student reconstruct the same physical problem from your settings? What information might be missing?
