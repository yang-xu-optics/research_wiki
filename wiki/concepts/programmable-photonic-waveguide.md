---
type: concept
name: "Programmable photonic waveguide"
aliases: ["2D programmable waveguide", "programmable slab waveguide"]
sources: [[2d-programmable-linear-waveguide-mcmahon, 2d-programmable-nonlinear-waveguide-mcmahon]]
related: [[photoconductive-gain-programming, lithium-niobate, quasi-phase-matching, optical-neural-network, programmable-photonic-computing]]
tags: [photonics, hardware, programmable]
---

# Programmable photonic waveguide

> A photonic chip whose spatial profile of an **optical material property** — refractive index Δn(x, z), or χ⁽²⁾ nonlinearity, or both — can be reprogrammed across thousands of independent regions of a slab waveguide, without lithographically defining discrete devices. Realized in two papers from the McMahon group in late 2025 / early 2026.

## Origin

Two companion papers from [[peter-mcmahon|McMahon]]'s group at [[mcmahon-lab-cornell|Cornell]] and [[ntt-research-pin-labs|NTT Research PIN Labs]]:

- **Linear** (programs refractive index): [[2d-programmable-linear-waveguide-mcmahon]] — Nature Physics, Dec 2025. Lithium niobate slab + photoconductor.
- **Nonlinear** (programs χ⁽²⁾): [[2d-programmable-nonlinear-waveguide-mcmahon]] — Nature, Jan 2026. Silicon nitride slab + photoconductor.

Conceptual roots: photorefractive crystals (1980s–90s) and inverse-designed nanophotonics. The new piece is **programmability at scale** — photorefractives had too little contrast (Δn ~10⁻⁴), inverse-designed chips are fixed at fabrication.

## How it works

A slab waveguide is sandwiched between a transparent top electrode and a conductive substrate, with a **photoconductor layer** in between. A patterned light beam (the "programming illumination") is projected onto the top:

1. Where the projected light is bright, the photoconductor becomes locally conductive — see [[photoconductive-gain-programming]].
2. The bias voltage applied across the stack drops mostly across the (still-insulating) waveguide in those regions, producing a patterned bias electric field E_bias(x, z) inside the waveguide.
3. That bias field changes a material property:
   - **Linear case:** via the [[electro-optic-effect|Pockels effect]] in [[lithium-niobate]], the field changes the refractive index by Δn ∝ E_bias.
   - **Nonlinear case:** via electric-field-induced χ⁽²⁾ in centrosymmetric [[silicon-nitride|SiN]], χ⁽²⁾(x, z) = 3χ⁽³⁾ E_bias(x, z).
4. The optical signal of interest propagates through the slab and "feels" the programmed 2D structure.

A signal beam co-propagates through the slab and is shaped (linearly or nonlinearly) by the programmed pattern. This avoids the O(N²) wiring problem of MZI-mesh photonic neural networks — only one uniform bias electrode is needed; the spatial programming is done optically.

## Trade-offs / Contrasts with

- vs **MZI / microring meshes** — discrete-component photonic NNs scale in chip area as O(N²) due to wiring and component size; programmable waveguides scale as ~O(N^1.5) per [[2d-programmable-linear-waveguide-mcmahon]].
- vs **inverse-designed nanophotonic chips** — those also exploit multimode 2D structure, but the structure is etched and fixed; programmable waveguides keep that structure rewritable.
- vs **photorefractive slab waveguides (historical)** — same idea but max Δn was ~10⁻⁴; photoconductive gain pushes useful Δn to ~10⁻³, enough to do meaningful computation.
- vs **phase-change-material programmable photonics** — PCM allows arbitrary patterns but is limited by rewrite cycles (~4,000) and high optical loss (>2.8 dB/mm). Photoconductive programmable waveguides have no comparable rewrite limit.

## Open questions

- Practical ceiling on N (vector dimension) — current demos at N=49; the energy-efficiency case for optics needs N ≳ 1,000.
- Could a single stack combine the linear (Δn) and nonlinear (χ⁽²⁾) functionalities?
- Long-term stability of the photoconductor and electrode stack under sustained bias / high optical power.
- Update-rate ceiling — currently ~3 Hz (linear) / ~1 Hz (nonlinear), projector- or RC-limited; what's the path to kHz+?

## Related

- [[photoconductive-gain-programming]]
- [[lithium-niobate]]
- [[quasi-phase-matching]]
- [[second-harmonic-generation]]
- [[optical-neural-network]]
- [[programmable-photonic-computing]]
