---
type: overview
title: "Optics and photonics research map"
scope: "A cross-field synthesis of integrated optics/photonics papers aimed at surfacing reusable mechanisms and research ideas"
tags: [photonics, integrated-photonics, research-ideas, nonlinear-optics, quantum-photonics]
---

# Optics and photonics research map

**Last revised:** 2026-06-17
**Scope:** A high-level map of how this vault's optics/photonics papers connect across materials, devices, nonlinear mechanisms, quantum light, combs, modulation, attosecond science, and programmable platforms.

> The vault should not become a folder of isolated optics subfields. Its useful unit is a reusable design pattern: a material capability, phase-matching trick, confinement regime, control mechanism, or integration strategy that might recombine with another paper to inspire a new experiment.

## Current Landscape

The III-V / AlGaAs and HHG batches add two major axes to the existing programmable-photonics thread:

- [[programmable-photonic-computing]] asks how to make the optical medium itself reconfigurable, using patterned fields to program linear or nonlinear response.
- [[iii-v-integrated-photonics]] asks how to pack active, nonlinear, electro-optic, and quantum functions into a monolithic semiconductor platform.
- [[silicon-nitride]] and [[silicon-nitride-on-sapphire]] provide a low-loss, wide-band, process-stability counterpoint: excellent passive/comb platform, weaker native active/nonlinear functionality.
- [[algaas-on-insulator]] is the high-index-contrast version of the III-V story: strong chi(2), strong chi(3), low telecom nonlinear loss, and small footprint, but fabrication maturity and yield become central.
- [[high-harmonic-generation]] is the extreme-upconversion axis: nonperturbative light-matter dynamics can generate attosecond/XUV radiation and, once the field is quantized, nonclassical light states.

## Connecting Threads

- **Phase matching as architecture.** [[semiconductor-phase-matching]] appears in many forms: [[bragg-reflection-waveguide|Bragg reflection waveguides]], domain-disordered [[quasi-phase-matching|QPM]], periodically inverted AlGaAs, form birefringence, and directionally induced QPM. These are not just tricks for SHG; they decide whether the same platform can support lasers, modulators, quantum sources, and mid-IR generation.
- **One platform, many nonlinear jobs.** AlGaAs spans [[second-harmonic-generation]], DFG, SPDC photon-pair generation, Kerr combs, and supercontinuum generation. The recurring question is how to use both chi(2) and chi(3) without forcing a separate chip for each.
- **Active/passive integration.** III-Vs are valuable because a nonlinear device can plausibly sit next to an electrically pumped laser, amplifier, detector, or [[electro-optic-modulation|modulator]]. This is the sharp contrast with many passive nonlinear platforms.
- **Quantum and classical share hardware.** The same microresonator or waveguide physics that enables telecom combs and supercontinuum also enables [[integrated-quantum-photonics|quantum photonics]] through spontaneous four-wave mixing or SPDC.
- **Control variables migrate.** Older devices hard-code function in epitaxy, gratings, or geometry. Newer programmable-waveguide work moves the control variable into an applied optical/electrical pattern. A research opportunity is to combine strong III-V nonlinearities with reconfigurable control patterns.
- **Strong-field quantum optics extends the spectrum.** [[strong-field-quantum-optics]] asks whether HHG can do for XUV/attosecond light what chi(2)/chi(3) does for near-IR quantum frequency conversion: move quantum state structure across spectral ranges while also probing matter.
- **Quantum light becomes a driver, not only an output.** [[quantum-light-driven-hhg]] and [[bright-squeezed-vacuum]] turn photon-number, quadrature, polarization, and spatial fluctuations into control knobs for cutoffs, symmetry breaking, bunching, phase locking, and material response.
- **Materials become quantum-optical emitters.** [[solid-state-high-harmonic-generation]] connects topology, excitons, Mott physics, and semiconductor dynamics to photon statistics and squeezing in emitted harmonics.
- **Critical matter correlations become a light-state resource.** [[critical-correlations-hhg-entanglement]] asks whether ferroelectric phase transitions, soft modes, domains, and other long-range-correlated matter states can enhance HHG squeezing and harmonic-mode entanglement.

## Research Idea Prompts

- Can [[semiconductor-phase-matching]] be made post-fabrication programmable, borrowing from [[photoconductive-gain-programming]] or carrier-induced index control?
- Can [[algaas-on-insulator]] host both a low-voltage [[electro-optic-modulation|EO modulator]] and a nonlinear comb/photon-pair source without compromising optical loss?
- Can a [[silicon-nitride-on-sapphire]] or SiN platform borrow III-V active pieces only where needed, while keeping SiN as the low-loss routing/nonlinear backbone?
- Can [[bragg-reflection-waveguide|BRW]] phase matching be reinterpreted as a general dispersion-engineering method for quantum-state engineering, rather than only a frequency-conversion device geometry?
- Can comb/data-link work and quantum-source work share a common packaging stack, so that classical WDM infrastructure becomes a control/readout layer for quantum photonics?
- Can [[high-harmonic-generation]] become an extreme quantum frequency converter, moving squeezing or entanglement into XUV/attosecond bands?
- Can ferroelectric or long-range-correlated media turn critical matter correlations into measurable [[critical-correlations-hhg-entanglement|HHG squeezing and entanglement]]?
- Can [[bright-squeezed-vacuum]] or structured squeezed light serve as a low-damage "quantum dial" for spectroscopy of fragile 2D and correlated materials?
- Can photonic confinement ideas from [[algaas-on-insulator]], nanostructures, or metasurfaces reduce HHG field requirements enough to connect attosecond physics with integrated photonics?

## Sources

- [[algaas-nonlinear-integrated-photonics-mobini]]
- [[nonlinear-integrated-quantum-photonics-algaas-baboux]]
- [[frequency-comb-algaas-oi-pu]]
- [[octave-supercontinuum-algaas-oi-kuyken]]
- [[algaas-oi-entangled-photon-pair-microring-steiner]]
- [[chip-frequency-comb-parallel-data-hu]]
- [[programmable-photonic-computing]]
- [[quantum-optical-nature-hhg-gorlach]]
- [[high-harmonic-generation-driven-by-quantum-light-gorlach]]
- [[high-harmonic-generation-bright-squeezed-vacuum-rasputnyi]]
- [[entanglement-squeezing-optical-field-modes-hhg-stammer]]
- [[photon-antibunching-hhg-stammer]]
