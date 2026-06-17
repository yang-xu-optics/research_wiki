---
type: concept
name: "Semiconductor phase matching"
aliases: ["AlGaAs phase matching", "III-V phase matching"]
sources: [[ridge-bragg-reflection-waveguide-shg-helmy, type-ii-qpm-superlattice-waveguides-hutchings, periodically-inverted-algaas-waveguides-ota, directionally-induced-qpm-algaas-morais]]
related: [[quasi-phase-matching, bragg-reflection-waveguide, second-harmonic-generation, iii-v-integrated-photonics]]
tags: [nonlinear-optics, phase-matching, algaas, iii-v]
---

# Semiconductor phase matching

> Semiconductor phase matching is the family of design strategies used to make chi(2) nonlinear processes efficient in cubic III-V materials, where strong nonlinearity exists but natural birefringence is absent.

## Origin

The batch shows several generations of solutions: Bragg reflection waveguides — [[ridge-bragg-reflection-waveguide-shg-helmy]], domain-disordered QPM — [[type-ii-qpm-superlattice-waveguides-hutchings]], periodically inverted AlGaAs — [[periodically-inverted-algaas-waveguides-ota]], and directionally induced QPM in curved homogeneous waveguides — [[directionally-induced-qpm-algaas-morais]].

## How it works

The design goal is always the same: arrange propagation constants, nonlinear tensor signs, or modal symmetries so that nonlinear polarization adds constructively rather than washing out. The implementation differs:

- Bragg reflection waveguides use modal dispersion from a vertical photonic-bandgap structure.
- Domain-disordered QPM modulates the nonlinear susceptibility after growth by quantum-well intermixing.
- Periodically inverted AlGaAs attempts a more literal QPM domain pattern through sublattice reversal epitaxy.
- Directionally induced QPM changes the effective nonlinear tensor projection by bending the propagation direction.

## Trade-offs / Contrasts with

- vs [[quasi-phase-matching]] in ferroelectrics — semiconductors lack easy periodic poling, so the device geometry and epitaxial process carry more of the burden.
- vs [[photoconductive-gain-programming]] — most semiconductor phase matching is fixed at fabrication; programmable field patterns hint at a future where phase matching could be adaptive.

## Open questions

- Which phase-matching scheme is easiest to combine with active lasers and modulators?
- Can phase matching be made tunable enough to support multi-process or self-optimizing nonlinear chips?

## Related

- [[bragg-reflection-waveguide]]
- [[quasi-phase-matching]]
- [[second-harmonic-generation]]

