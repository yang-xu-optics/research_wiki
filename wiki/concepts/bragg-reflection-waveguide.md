---
type: concept
name: "Bragg reflection waveguide"
aliases: ["BRW", "Bragg reflection waveguides"]
sources: [[ridge-bragg-reflection-waveguide-shg-helmy, femtosecond-shg-algaas-brw-han, dfg-algaas-brw-han]]
related: [[semiconductor-phase-matching, second-harmonic-generation, integrated-quantum-photonics]]
tags: [photonics, waveguides, nonlinear-optics, algaas]
---

# Bragg reflection waveguide

> A Bragg reflection waveguide uses a multilayer photonic-bandgap mirror to guide one interacting mode while other modes may be guided by total internal reflection, enabling phase matching in otherwise non-birefringent semiconductor waveguides.

## Origin

In this batch, BRWs appear as a way to unlock efficient AlGaAs chi(2) interactions without periodic poling: ridge BRW SHG — [[ridge-bragg-reflection-waveguide-shg-helmy]], femtosecond SHG with pump depletion — [[femtosecond-shg-algaas-brw-han]], and DFG around telecom wavelengths — [[dfg-algaas-brw-han]].

## How it works

The device engineers the modal index of one wavelength through Bragg confinement and the other through conventional total-internal-reflection confinement. Matching those modal indices satisfies the nonlinear phase-matching condition while keeping strong spatial overlap.

## Trade-offs / Contrasts with

- vs domain-disordered or periodically inverted QPM — BRWs avoid domain engineering but can suffer from mode-coupling complexity and loss in the Bragg-confined mode.
- vs [[algaas-on-insulator]] nanowires — BRWs are an epitaxial/modal phase-matching solution; AlGaAsOI often relies on high confinement and dispersion engineering.

## Open questions

- Can BRW dispersion engineering be combined with resonators or programmable tuning?
- Are BRWs best viewed as legacy AlGaAs devices, or as a still-useful degree of freedom for integrated quantum sources?

## Related

- [[semiconductor-phase-matching]]
- [[second-harmonic-generation]]
- [[integrated-quantum-photonics]]

