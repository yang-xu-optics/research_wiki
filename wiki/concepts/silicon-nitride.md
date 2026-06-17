---
type: concept
name: "Silicon nitride"
aliases: ["SiN", "Si3N4", "silicon nitride photonics"]
sources: [[crack-free-silicon-nitride-on-sapphire-lu, 2d-programmable-nonlinear-waveguide-mcmahon]]
related: [[silicon-nitride-on-sapphire, wide-band-photonics, second-harmonic-generation]]
tags: [photonics, materials, nonlinear-optics]
---

# Silicon nitride

> Silicon nitride is a low-loss dielectric photonics material used across visible, near-infrared, telecom, and mid-infrared integrated optics. In this vault it matters both as the waveguide material for programmable nonlinear photonics and as the material whose stress limits motivate [[silicon-nitride-on-sapphire]].

## Origin

Silicon nitride became a major integrated-photonics platform because it combines broad optical transparency, low propagation loss, CMOS-adjacent fabrication, and useful dispersion engineering. The Si3N4-on-sapphire paper frames it as the dominant wide-band platform for nonlinear and quantum photonics, especially when grown by LPCVD as stoichiometric Si3N4 — [[crack-free-silicon-nitride-on-sapphire-lu]].

## How it works

For photonics, Si3N4 is patterned into waveguides, resonators, and photonic integrated circuits. The paper distinguishes several practical regimes:

- **Stoichiometric LPCVD Si3N4** gives strong optical performance and repeatability, but on silicon it has high residual tensile stress.
- **Si-rich SiN** can reduce stress, but the paper says that comes with higher optical loss.
- **PECVD SiN** can grow thicker films and is CMOS-compatible, but the paper describes wider variation in material indices and reported propagation losses.
- **Si3N4 on sapphire** keeps the stoichiometric LPCVD material target while changing the substrate mechanics — [[crack-free-silicon-nitride-on-sapphire-lu]].

In [[2d-programmable-nonlinear-waveguide-mcmahon]], SiN is also important because it is centrosymmetric: it lacks intrinsic chi(2), but can host electric-field-induced chi(2) when biased through the photoconductive stack.

## Trade-offs / Contrasts with

- vs [[lithium-niobate]] — SiN is lower-loss and fabrication-friendly but lacks intrinsic Pockels and chi(2); lithium niobate has strong electro-optic and nonlinear coefficients but a different fabrication stack.
- vs silicon photonics — SiN has a wider transparency window and lower nonlinear absorption in many regimes, but less mature electronics integration than silicon.
- vs [[silicon-nitride-on-sapphire]] — SiN is the material; SiNoSa is a substrate/platform choice meant to reduce stress and cracking for thick stoichiometric LPCVD films.

## Open questions

- Which combination of substrate, cladding, and anneal best balances low loss, stress, and foundry manufacturability?
- Can Si3N4-on-sapphire become a standard platform, or will sapphire-specific packaging and integration limits keep it niche?

## Related

- [[silicon-nitride-on-sapphire]]
- [[wide-band-photonics]]
- [[second-harmonic-generation]]
