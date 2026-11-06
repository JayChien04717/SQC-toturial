# Q2 | Fluxonium Spectrum and Matrix Elements vs. Flux

## Where to Learn

1. Review operator construction, diagonalization, and matrix elements. [QuTiP quantum object documentation](https://qutip.readthedocs.io/en/stable/apidoc/quantumobject.html)
2. Study the fluxonium Hamiltonian and the representation of charge and phase in an LC oscillator basis. Use the conventions below when comparing results. [scqubits fluxonium reference](https://scqubits.readthedocs.io/en/latest/api-doc/_autosummary/scqubits.core.fluxonium.Fluxonium.html)
3. See Fig. 6.25 for a measured two-tone fluxonium spectrum and §6.2 for a discussion of selection rules. [Long Nguyen's thesis](../01_paper_reading/LongNguyen_thesis_final.pdf)

## Exercises

Use one fluxonium with the teaching parameters $E_J/h = 4.0$ GHz, $E_C/h = 1.0$ GHz, and $E_L/h = 0.5$ GHz. Sweep the reduced external flux $f = \Phi_{\mathrm{ext}}/\Phi_0$ from 0 to 1, including $f = 0.5$. Use the following Hamiltonian convention.

$$
H = 4E_C\hat n^2 + \frac{E_L}{2}(\hat\varphi - 2\pi f)^2 - E_J\cos\hat\varphi .
$$

Here $\hat n$ is the dimensionless Cooper-pair number operator and $\hat\varphi$ is the dimensionless junction phase operator. They are conjugate, with $[\hat\varphi,\hat n]=i$ in the untruncated Hilbert space.

1. Construct $\hat n$, $\hat\varphi$, and $H$ in a truncated LC oscillator basis using QuTiP. Diagonalize $H$ at each flux point and retain the lowest five eigenstates.
2. **Spectrum plot.** Plot $(E_j-E_0)/h$ for $j=1,\ldots,4$ versus $\Phi_{\mathrm{ext}}/\Phi_0$, with frequency in GHz. Compare the spectrum at zero flux and half a flux quantum. Use the measured spectrum in Fig. 6.25 as a qualitative comparison.
3. **Charge matrix elements.** Plot $|\langle i|\hat n|j\rangle|$ versus $\Phi_{\mathrm{ext}}/\Phi_0$ for the $0\to1$, $0\to2$, $0\to3$, and $1\to2$ transitions.
4. **Phase matrix elements.** Plot $|\langle i|\hat\varphi|j\rangle|$ versus the same flux sweep for the same transitions. Evaluate both operators in the energy eigenbasis at each bias.
5. At zero flux and half a flux quantum, use the symmetry of the potential and the parity of the eigenstates to explain which matrix elements vanish. Compare the charge and phase plots away from these biases. As a consistency check, derive the relation between the two off-diagonal matrix elements from $[H,\hat\varphi]$.
6. Increase the oscillator basis cutoff and check convergence of both the spectrum and the matrix elements. Check that the transition frequencies at the endpoints agree, as the spectrum repeats after one flux quantum. Distinguish small numerical residues from physically allowed transitions.
