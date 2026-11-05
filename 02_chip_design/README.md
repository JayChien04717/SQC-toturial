# 02 | Design a Single-Qubit System

Develop one connected TransmonCross design through four exercises. Learn the implementation from the official Metal tutorials, then choose and tune the geometry and model parameters yourself.

| Exercise | Goal | Guide |
|---|---|---|
| M1 | Build a TransmonCross system with a readout resonator, charge line, and CPW feedline | [Layout](01_layout.md) |
| M2 | Tune EC/h to 250 MHz using the M1 layout | [Capacitance and EC](02_capacitance_ec.md) |
| M3 | Tune the transmon transition to 4 GHz and the readout resonator to 6 GHz | [Eigenmodes](03_eigenmode.md) |
| M4 | Tune the readout resonator's loaded linewidth to 2 MHz | [Linewidth](04_linewidth.md) |

Use the same evolving layout throughout. Changes made for a later target can affect earlier results, so recheck EC, frequencies, and linewidth after tuning.

For each calculation, understand the geometry, materials, nodes or ports, boundary conditions, junction model, units, and convergence. Start with the [Solver checklist](solver_workflow.md).

Numerical convergence and proximity to a design target are separate checks. The instructor can set target tolerances appropriate to the available solver accuracy; the convergence checks in each exercise are starting points.
