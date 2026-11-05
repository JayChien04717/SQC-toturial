# Units, Notation, and Model Scope

| Quantity | Convention |
|---|---|
| f, g, alpha, EC/h, EJ/h | GHz, equivalent to cycles/ns; g denotes the exchange coefficient in H/h |
| H/h | GHz; energies divided by h |
| H/hbar | rad/ns; differs from H/h by a factor of 2π |
| Time | ns; 30 μs = 30000 ns |
| C | fF; multiply by 10⁻¹⁵ for SI calculations |
| Linewidth Δf | Power-Lorentzian FWHM in GHz |
| κ | Energy decay rate in ns⁻¹; κ = 2πΔf and QL = fr/Δf for the isolated-mode convention |
| ζ | (E11 − E10 − E01 + E00)/h; multiply GHz by 1000 to obtain MHz |

For a single linear mode, energy decays as exp(−κt), while field amplitude decays as exp(−κt/2). These lifetimes differ. The single-photon loss collapse operator is √κ a.

For a floating transmon, define the differential charge coordinate and the boundary conditions of the other nodes before calculating charging energy. An arbitrary diagonal element of a Maxwell capacitance matrix is not generally the effective capacitance. Coordinate changes must also be reflected in the Hamiltonian.

The introductory QuTiP exercises use weakly anharmonic Duffing transmons, exchange coupling under the rotating-wave approximation, and a finite level truncation. This model is unsuitable for arbitrary fluxonium circuits, high excitation, or operation far outside the transmon regime. A fluxonium extension requires an appropriate basis for 4EC n² + EL(φ − φext)²/2 − EJ cos φ and the corresponding coupling matrix elements.

Here, spectrum refers to Hamiltonian energies and transition frequencies. Experimental absorption spectra and two-time correlation spectra also depend on drive operators, dissipation, populations, and selection rules.
