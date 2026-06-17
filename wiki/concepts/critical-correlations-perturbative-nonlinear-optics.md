---
type: concept
name: "Critical correlations in perturbative nonlinear optics"
aliases: ["critical SHG squeezing", "critical THG entanglement", "correlated-matter nonlinear quantum optics"]
sources: [[critical-correlations-hhg-entanglement, critical-hhg-simulation-framework, second-harmonic-generation, quasi-phase-matching]]
related: [[second-harmonic-generation, critical-correlations-hhg-entanglement, integrated-quantum-photonics, algaas-on-insulator]]
tags: [nonlinear-optics, quantum-optics, entanglement, squeezing, ferroelectrics]
---

# Critical correlations in perturbative nonlinear optics

> The idea that matter correlations can create light correlations is not specific to HHG. Perturbative processes such as SHG, THG, SPDC, and four-wave mixing can also map fluctuations of nonlinear susceptibility or polarization into squeezing and entanglement, though usually in a cleaner but less extreme regime.

## Origin

The [[critical-correlations-hhg-entanglement|critical-HHG]] idea starts from a source-current viewpoint: harmonic-mode quantum correlations are determined by connected matter current or polarization correlations. The same input-output logic applies to perturbative nonlinear optics. The source is now a lower-order nonlinear polarization, for example `P^(2) = chi^(2) E^2` or `P^(3) = chi^(3) E^3`, rather than a nonperturbative HHG current.

## How it works

In ordinary textbook SHG or THG, `chi^(2)` and `chi^(3)` are treated as fixed classical tensors. Then a coherent pump mostly produces a coherent harmonic field in the undepleted-pump limit.

If the nonlinear medium is quantum and correlated, the emitted field instead depends on fluctuations of the nonlinear polarization:

`delta P_NL(t) = delta chi^(n)(t) E_cl(t)^n + chi^(n) delta[E(t)^n] + ...`.

Near a ferroelectric, structural, excitonic, or magnetic transition, the nonlinear susceptibility is tied to order-parameter correlation functions. Critical fluctuations can therefore change not only conversion efficiency, but also the quantum noise and correlations of the generated light.

## Process comparison

- **SHG/THG.** A coherent pump can produce harmonic squeezing or pump-harmonic entanglement when pump depletion, nonlinear backaction, resonant enhancement, or susceptibility fluctuations are included. In the simplest undepleted classical-susceptibility limit, the output may remain nearly coherent.
- **SPDC/SFWM.** These perturbative processes already generate photon-pair entanglement from vacuum fluctuations. A correlated or critical medium could add a material-correlation control knob over pair statistics, multimode structure, and excess or squeezed noise.
- **HHG.** HHG is more broadband and nonperturbative, with stronger natural backaction and many harmonic modes. This can make matter-mediated correlations more visible, but also harder to model and measure.

## Why perturbative processes may be useful

Perturbative nonlinear optics may be the better first experimental and theoretical platform because phase matching, cavities, homodyne detection, and integrated devices are mature. SHG/THG in a correlated or ferroelectric medium can test the mechanism in a small number of modes before moving to the full HHG comb.

The sharp question becomes: does a critical material only enhance the mean nonlinear coefficient, or does it also imprint connected susceptibility noise that produces nonclassical light?

For a concrete cavity simulation/theory blueprint, see [[critical-cavity-shg-thg-simulation-framework]].

## Open questions

- Can SHG or THG near a ferroelectric transition show squeezing below shot noise after subtracting classical critical noise?
- Can a cavity-enhanced SHG/THG system make matter-mediated pump-harmonic entanglement observable at lower intensities than HHG?
- Do SPDC/SFWM pair correlations acquire measurable critical scaling when the nonlinear susceptibility is tied to an order parameter?
- Which platform gives the cleanest separation between classical susceptibility fluctuations and genuine quantum squeezing: bulk ferroelectric, thin-film lithium niobate, quantum paraelectric, excitonic material, or integrated AlGaAs?

## Related

- [[critical-correlations-hhg-entanglement]]
- [[critical-hhg-simulation-framework]]
- [[critical-cavity-shg-thg-simulation-framework]]
- [[second-harmonic-generation]]
- [[quasi-phase-matching]]
