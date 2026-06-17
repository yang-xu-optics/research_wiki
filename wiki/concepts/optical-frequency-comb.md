---
type: concept
name: "Optical frequency comb"
aliases: ["frequency comb", "Kerr comb", "microcomb", "supercontinuum"]
sources: [[frequency-comb-algaas-oi-pu, chip-frequency-comb-parallel-data-hu, octave-supercontinuum-algaas-oi-kuyken]]
related: [[algaas-on-insulator, wide-band-photonics, integrated-quantum-photonics]]
tags: [photonics, nonlinear-optics, combs, communications]
---

# Optical frequency comb

> An optical frequency comb is a spectrum of evenly spaced optical lines. Integrated combs turn nonlinear waveguides or resonators into compact multi-wavelength sources for metrology, communications, spectroscopy, and potentially quantum photonics.

## Origin

In this batch, AlGaAsOI appears both as a resonant Kerr-comb platform — [[frequency-comb-algaas-oi-pu]] and as a non-resonant high-efficiency comb source for massive data transmission — [[chip-frequency-comb-parallel-data-hu]]. The supercontinuum paper extends the same platform toward octave bandwidths useful for self-referencing — [[octave-supercontinuum-algaas-oi-kuyken]].

## How it works

Comb generation is powered by chi(3) nonlinearities such as four-wave mixing, self-phase modulation, and soliton/supercontinuum dynamics. Resonators reduce pump threshold through high Q; straight dispersion-engineered waveguides can improve robustness and pump-to-comb conversion efficiency.

## Trade-offs / Contrasts with

- resonator combs — low threshold and compact, but sensitive to detuning and thermal dynamics.
- straight-waveguide combs — higher pump energy can be needed, but conversion efficiency and robustness can be better.
- vs [[second-harmonic-generation]] — combs are usually chi(3)-driven; octave comb systems often need chi(2) SHG for self-referencing, making AlGaAs's dual chi(2)/chi(3) capability interesting.

## Open questions

- Can one AlGaAs chip combine comb generation, SHG self-referencing, modulation, and gain?
- Can classical comb multiplexing infrastructure help scale quantum photonic sources?

## Related

- [[algaas-on-insulator]]
- [[wide-band-photonics]]
- [[integrated-quantum-photonics]]

