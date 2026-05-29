---
type: concept
name: "Second-harmonic generation (SHG)"
aliases: ["SHG", "frequency doubling"]
sources: [[2d-programmable-nonlinear-waveguide-mcmahon]]
related: [[quasi-phase-matching, programmable-photonic-waveguide]]
tags: [nonlinear-optics]
---

# Second-harmonic generation (SHG)

> A χ⁽²⁾ nonlinear-optical process where two photons of frequency ω combine into one photon at frequency 2ω. The workhorse demonstration process for nonlinear photonic devices, including the programmable nonlinear waveguide of [[2d-programmable-nonlinear-waveguide-mcmahon]].

## Origin

First observed by Franken et al. (1961) shortly after the invention of the laser. The textbook NLO process; the most-used demonstration of new nonlinear materials and devices because it is conceptually simple and easy to measure.

## How it works

- A pump field E_ω at frequency ω drives a polarization with a quadratic term P^(2) ∝ χ⁽²⁾ E_ω², which radiates at frequency 2ω.
- Efficient SHG requires **phase matching**: the second-harmonic light generated at different points along the propagation must add coherently — k₂ω = 2k_ω.
- In dispersive materials this fails naturally; the practical fixes are **birefringent phase matching** or **[[quasi-phase-matching|QPM]]**.
- The SHG efficiency scales with (χ⁽²⁾)² × L² × pump intensity (in the undepleted-pump regime), so longer interaction lengths, stronger nonlinearity, and tighter mode confinement all help.

In [[2d-programmable-nonlinear-waveguide-mcmahon]], SHG is the demonstration process used to characterize three programmable knobs: spectral (which pump wavelength is doubled), spatial (mode shape of the SH output), and spatio-spectral (joint).

## Trade-offs / Contrasts with

- vs **sum-frequency / difference-frequency / parametric generation** — same family of χ⁽²⁾ processes; SHG is the simplest, hence the standard benchmark.
- vs **third-order processes (χ⁽³⁾, e.g. four-wave mixing)** — χ⁽³⁾ is universal but much weaker per unit volume; χ⁽²⁾ requires non-centrosymmetric materials (or electric-field-induced χ⁽²⁾, as in this work).

## Open questions

- How efficient can programmable-χ⁽²⁾ SHG become with the photoconductive-bias stack, vs intrinsic χ⁽²⁾ in periodically poled lithium niobate?
- The same machinery should enable **parametric down-conversion** for entangled-photon-pair sources — a path toward programmable quantum-light sources flagged by the authors.

## Related

- [[quasi-phase-matching]]
- [[programmable-photonic-waveguide]]
- [[2d-programmable-nonlinear-waveguide-mcmahon]]
