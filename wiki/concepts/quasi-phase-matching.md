---
type: concept
name: "Quasi-phase matching (QPM)"
aliases: ["QPM", "quasi-phase-matching grating"]
sources: [[2d-programmable-nonlinear-waveguide-mcmahon, type-ii-qpm-superlattice-waveguides-hutchings, periodically-inverted-algaas-waveguides-ota, directionally-induced-qpm-algaas-morais]]
related: [[second-harmonic-generation, programmable-photonic-waveguide]]
tags: [nonlinear-optics, photonics]
---

# Quasi-phase matching (QPM)

> A technique for making nonlinear optical processes (e.g. [[second-harmonic-generation|SHG]]) efficient by **periodically modulating the sign of χ⁽²⁾** along the propagation direction, compensating the phase mismatch between interacting frequencies that would otherwise cause destructive interference.

## Origin

Classic nonlinear-optics result (Armstrong/Bloembergen/Ducuing/Pershan, 1962; experimentally realized via periodically poled materials decades later). Historically implemented by **periodically poling** ferroelectric crystals (e.g. periodically poled lithium niobate, PPLN) or by orientation-patterned epitaxy on semiconductors. Recontextualized in [[2d-programmable-nonlinear-waveguide-mcmahon]] as something that can be programmed in 2D rather than sculpted at fab time.

## How it works

- A nonlinear process like SHG needs the second-harmonic field generated at one point to add constructively to the fields generated downstream. This requires the wavevectors of the pump and second-harmonic waves to be matched: Δk = k₂ω − 2k_ω = 0.
- In a real material with dispersion, Δk ≠ 0; SHG light generated at different points along the propagation interferes destructively after a "coherence length" π/Δk.
- **QPM fix:** flip the sign of χ⁽²⁾ every coherence length (period Λ = 2π/Δk). The sign flip cancels the destructive part of the phase, and SHG accumulates coherently again.
- More elaborate QPM grating structures (chirped, apodized, 2D, holographic) enable bandwidth engineering, pulse shaping, multi-band SHG, and structured second-harmonic outputs.

In [[2d-programmable-nonlinear-waveguide-mcmahon]], the period Λ is set by the spacing of bright stripes in the projected illumination pattern; sweeping Λ tunes the resonant pump wavelength. A measured nominal poling period of 16.65 µm and group-velocity mismatch of −92 fs/mm characterize their device.

In III-V semiconductors, QPM becomes a fabrication and architecture problem because cubic materials like GaAs/AlGaAs cannot be simply periodically poled like ferroelectrics. This batch shows three alternatives: sublattice reversal in periodically inverted AlGaAs, post-growth domain disordering by quantum-well intermixing, and geometry-induced effective QPM in curved waveguides — [[periodically-inverted-algaas-waveguides-ota]], [[type-ii-qpm-superlattice-waveguides-hutchings]], [[directionally-induced-qpm-algaas-morais]].

## Trade-offs / Contrasts with

- vs **birefringent phase matching** — birefringence uses material anisotropy to align phase velocities; works only for some materials/wavelengths and constrains polarization choices.
- vs **periodic poling at fab time** — the chip is fixed; one chip = one set of QPM gratings = one set of supported processes.
- vs **programmable QPM** (this work) — the same physical chip can host many different gratings, retuned in real time. Enables in-situ inverse design and adaptive operation.

## Open questions

- 2D QPM structures (varying transversely as well as longitudinally) unlock spatio-spectral engineering — what new NLO functions become accessible?
- How well do programmable QPM gratings compare to PPLN in absolute efficiency at the same active length?

## Related

- [[second-harmonic-generation]]
- [[programmable-photonic-waveguide]]
- [[2d-programmable-nonlinear-waveguide-mcmahon]]
