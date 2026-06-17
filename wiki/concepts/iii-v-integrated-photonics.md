---
type: concept
name: "III-V integrated photonics"
aliases: ["III-V photonics", "compound semiconductor photonics", "GaAs photonics", "AlGaAs photonics"]
sources: [[carrier-induced-index-iii-v-bennett, algaas-nonlinear-integrated-photonics-mobini, nonlinear-integrated-quantum-photonics-algaas-baboux]]
related: [[algaas-on-insulator, semiconductor-phase-matching, electro-optic-modulation, integrated-quantum-photonics]]
tags: [photonics, integrated-photonics, iii-v, algaas]
---

# III-V integrated photonics

> III-V integrated photonics uses compound semiconductors such as GaAs, AlGaAs, InP, and InGaAsP as optical platforms where passive waveguides can potentially coexist with lasers, amplifiers, detectors, electro-optic modulators, and strong nonlinear devices.

## Origin

The oldest paper in this batch treats carrier-induced index change in InP, GaAs, and InGaAsP as a route to phase shifters and switches — [[carrier-induced-index-iii-v-bennett]]. The later AlGaAs literature reframes III-Vs as a nonlinear/quantum photonics platform because they combine high index contrast, high chi(2), high chi(3), direct band gaps, and mature epitaxy — [[algaas-nonlinear-integrated-photonics-mobini]], [[nonlinear-integrated-quantum-photonics-algaas-baboux]].

## How it works

The central advantage is co-location. A III-V chip can, in principle, host:

- active sources and gain from direct band-gap materials;
- [[electro-optic-modulation]] through Pockels or carrier mechanisms;
- [[second-harmonic-generation]], DFG, SPDC, four-wave mixing, combs, and supercontinuum through strong optical nonlinearities;
- photodiodes and possibly integrated quantum-light components.

The difficulty is that each function wants a different epitaxial stack, loss budget, band gap, mode confinement, and phase-matching strategy.

## Trade-offs / Contrasts with

- vs [[silicon-nitride]] — III-Vs offer active and stronger nonlinear functionality; SiN often wins on passive loss and process stability.
- vs [[lithium-niobate]] — III-Vs offer monolithic gain and compact high-index waveguides; lithium niobate offers excellent Pockels/chi(2) performance but usually needs heterogeneous integration for lasers.
- vs [[programmable-photonic-waveguide]] — III-V literature usually hard-codes function in epitaxy/geometry; programmable waveguides move function into a reconfigurable pattern.

## Open questions

- What is the simplest III-V stack that supports useful active, EO, chi(2), and chi(3) functions without becoming a fabrication compromise?
- Can III-V platforms become reconfigurable enough to act as research accelerators, not just fixed-function devices?

## Related

- [[algaas-on-insulator]]
- [[semiconductor-phase-matching]]
- [[electro-optic-modulation]]
- [[integrated-quantum-photonics]]

