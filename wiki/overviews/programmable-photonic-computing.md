---
type: overview
title: "Programmable photonic computing — McMahon-group research program"
scope: "How the McMahon Lab + NTT Research PIN program for 2D-programmable photonic substrates fits together and where it sits in the broader optical-computing landscape"
tags: [photonics, optical-computing, programmable-waveguide, mcmahon-lab, ntt-research]
---

# Programmable photonic computing — McMahon-group research program

**Last revised:** 2026-05-28
**Scope:** How the [[mcmahon-lab-cornell|McMahon Lab]] + [[ntt-research-pin-labs|NTT Research PIN]] program for 2D-programmable photonic substrates fits together, and where it sits in the broader [[optical-neural-network|optical-computing]] landscape.

> Across two papers in late 2025 and early 2026 the McMahon group has demonstrated a single programming primitive — patterned light → photoconductor → ~10⁴ "virtual electrodes" on a slab waveguide — applied to two different physical effects on two different substrates. The result is a unified architecture for **programmable photonic computing** that decouples the wiring problem from the compute problem.

## Landscape

Three layers fit together:

- **The programming primitive:** [[photoconductive-gain-programming]]. A photoconductor between bias electrodes lets a single uniform high voltage be optically "switched in" to thousands of independent regions at once, bypassing the O(N²) wiring bottleneck of CMOS-backplane-driven photonic chips.
- **The linear arm:** [[2d-programmable-linear-waveguide-mcmahon]] applies the primitive to a [[lithium-niobate]] slab via the [[electro-optic-effect|Pockels effect]] to program a refractive-index distribution Δn(x, z). The programmed pattern is a trainable parameter for an [[optical-neural-network|optical neural network]]; demonstrated up to 49-dim inputs (vowel classification, MNIST) with **N^1.5** chip-area scaling vs **N²** for MZI meshes.
- **The nonlinear arm:** [[2d-programmable-nonlinear-waveguide-mcmahon]] applies the primitive to a silicon-nitride slab via electric-field-induced χ⁽²⁾ to program an arbitrary 2D distribution of nonlinearity. Demonstrated programmable [[quasi-phase-matching|QPM]] gratings for [[second-harmonic-generation|SHG]], with spectral, spatial, and spatio-spectral engineering, plus in-situ inverse design and real-time feedback against environmental drift.

## Key axes

- **What is programmed:** refractive index (linear) vs χ⁽²⁾ nonlinearity (nonlinear).
- **Substrate:** lithium niobate (linear; intrinsic Pockels) vs silicon nitride (nonlinear; induced χ⁽²⁾).
- **Target application:** linear MVMs / inference (linear arm) vs frequency conversion, quantum light, NLO signal processing (nonlinear arm).
- **Programming-rate ceiling:** ~3 Hz (linear) and ~1 Hz (nonlinear) demonstrated — projector- and RC-limited.
- **Comparison to alternatives:** [[programmable-photonic-waveguide]]'s "Trade-offs / Contrasts with" lists how this stacks up against [[optical-neural-network|MZI meshes]], microring banks, phase-change cells, free-space diffractive ONNs, and historical photorefractive slabs.

## Current thinking

The two papers are best read as **one device family with one programming primitive**, instantiated for two different physical effects. The most consequential claim is the **N^1.5 area scaling** for ONN inference in [[2d-programmable-linear-waveguide-mcmahon]] — if it holds up at higher N, it's the first asymptotic (not just constant-factor) advantage over MZI meshes anyone has shown.

The nonlinear paper is closer to a quantum-photonics / NLO-engineering enabler than to a raw-compute play: programmable [[quasi-phase-matching]] in 2D unlocks adaptive, fab-tolerant nonlinear devices, and gestures toward programmable quantum-light sources and gates.

A plausible third milestone (not yet published) would be a **single stack that programs both Δn and χ⁽²⁾** — putting linear MVMs and nonlinear activations on the same chip, the missing piece for fully-optical deep networks. The overlap of authors and the architectural similarity make this a natural next step to watch for.

## Open threads

- N-scaling test: can a follow-up demonstrate N ≳ 200 or 1,000 in the linear waveguide? The paper's main accuracy/area claims rest on it.
- Update-rate engineering: kHz operation would change what closed-loop quantum / adaptive applications are feasible. The bottleneck appears to be the photoconductor RC and the projector.
- Hybrid stack: a stack supporting both [[electro-optic-effect|Pockels]] (Δn) and induced χ⁽²⁾ would let one chip carry both linear and nonlinear functions.
- Long-term reliability under sustained ~1 kV bias and high pump powers — not characterized in either paper.
- Author network: [[ryotatsu-yanagimoto]], [[tatsuhiro-onodera]], Logan Wright, Marc Jankowski, [[peter-mcmahon]] appear on both papers; their next first-author work is worth watching.

## Sources

- [[2d-programmable-linear-waveguide-mcmahon]]
- [[2d-programmable-nonlinear-waveguide-mcmahon]]
