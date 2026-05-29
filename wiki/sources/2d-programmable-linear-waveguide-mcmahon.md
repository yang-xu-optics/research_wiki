---
type: source
title: "Arbitrary control over multimode wave propagation for machine learning"
authors: [Tatsuhiro Onodera, Martin M. Stein, Benjamin A. Ash, Mandar M. Sohoni, Melissa Bosch, Ryotatsu Yanagimoto, Marc Jankowski, Timothy P. McKenna, Tianyu Wang, Gennady Shvets, Maxim R. Shcherbakov, Logan G. Wright, Peter L. McMahon]
url: https://doi.org/10.1038/s41567-025-03094-2
date_published: 2025-12-08
date_ingested: 2026-05-28
source_file: raw/sources/articles/2026-05-28-programmable-2d-linear-waveguide.pdf
kind: paper
tags: [photonics, optical-computing, programmable-waveguide, lithium-niobate, neural-networks, mcmahon-lab, ntt-research]
---

# Arbitrary control over multimode wave propagation for machine learning

> First demonstration of a **2D-programmable lithium niobate waveguide** with ~10,000 spatial degrees of freedom, used to perform neural-network inference (vowel classification, MNIST) directly via optically-programmed multimode wave propagation — Nature Physics, Vol 22, Jan 2026, pp. 164–171. From the [[mcmahon-lab-cornell|McMahon Lab]] (Cornell) and [[ntt-research-pin-labs|NTT Research PIN Labs]].

## TL;DR

- A photonic chip whose **refractive index distribution Δn(x, z)** can be reprogrammed across ~10⁴ regions of a [[lithium-niobate]] slab waveguide — without lithographically defining devices.
- Programming mechanism: shine a patterned **green light** onto a photoconductor layer; the illuminated regions become conductive, locally raising the bias electric field, which modulates the waveguide's refractive index via the [[electro-optic-effect|Pockels effect]]. See [[photoconductive-gain-programming]].
- The trained 2D pattern *is* the neural-network weight matrix. The chip performs a linear transform via multimode wave propagation; output intensity is binned to read out a class prediction.
- Demonstrated **vowel classification** (12-dim input → 7 classes, 96% test accuracy) and **MNIST** (49-dim → 10 classes).
- **Scaling claim:** programmable-waveguide area grows as **N^1.5**, vs **N^2** for discrete-component meshes (MZI / microring) — a real asymptotic, not just constant-factor, advantage.
- Training: **physics-aware training** — a hybrid in-situ optical forward pass + in-silico digital backprop through a differentiable model.
- Update rate: 3 Hz; pixel resolution 9 µm × 9 µm; active area 9 mm × 1 mm; max Δn ~10⁻³; bias voltage up to 1,000 V.

## Key claims

- **The discrete-component bottleneck.** Existing photonic neural networks built from MZIs / microrings / phase-change cells need 𝒪(N²) electronic wires routed through the chip perimeter, and individual optical components are large — so far limited to vectors well below the N ≳ 1,000 needed for an optical energy-efficiency advantage.
- **Treating the chip as a blank slate.** Instead of discrete components connected by single-mode waveguides, sculpt n(x, z) of the *whole* substrate. The programmable matrix W maps to the programmable Δn(x, z); inputs encode into the input optical field E(x, z=0); outputs are read out as binned intensity at z = L.
- **Photorefractive crystals tried this in the 1980s–90s** but failed: max Δn ~10⁻⁴ meant even centimeter-scale devices couldn't do large-scale ops. Phase-change materials (newer) hit limited rewrite cycles (~4,000) and high loss (>2.8 dB/mm).
- **Photoconductive gain is essential.** CMOS backplanes only deliver ~10 V per pixel; the photoconductor lets a single uniform 1,000 V bias be "switched in" optically at ~10⁴ virtual electrodes simultaneously.
- The propagation is governed by the paraxial Helmholtz equation: ∂_z E = (i/2k)∂²_x E + i k₀ Δn(x, z) E.
- **N^1.5 area scaling** is the headline asymptotic result. Linked to the fact that wave propagation across a 2D region carries more information per unit area than 1D-routed networks.

## Notable quotes

> "Instead of defining discrete elements, one can sculpt the continuous substrate of a photonic processor to perform computations through multimode interference in two dimensions."

> "Two-dimensional programmable waveguides may offer not only a constant-factor reduction in device area but also a scaling benefit, with the area required growing as N^1.5 rather than N^2."

> "Our use of photoconductive gain was essential for achieving large electro-optic modulation."

## Open questions

- What is the practical N ceiling? 49-dim is far below the N ≳ 1,000 the paper says is needed for an energy-efficiency advantage. What blocks scaling here?
- Optical losses and noise floor at higher Δn or longer propagation distances — not characterized in detail in the main text.
- Update rate is 3 Hz; can it match neural-net training cadences without redesigning the photoconductor RC time?
- How does it compare to the companion **nonlinear** chip ([[2d-programmable-nonlinear-waveguide-mcmahon]]) in fabrication tolerance and yield?

## Pages updated by this ingest

- [[programmable-photonic-waveguide]] — created; this paper is one of its two demonstrating works.
- [[photoconductive-gain-programming]] — created; the shared programming mechanism.
- [[electro-optic-effect]] — *not created this pass*; deferred until a paper requires its own page.
- [[lithium-niobate]] — created; the waveguide material in this paper.
- [[optical-neural-network]] — created; the application class.
- [[physics-aware-training]] — *not created this pass*; mentioned in the source summary above.
- [[mcmahon-lab-cornell]] — created; the originating lab.
- [[ntt-research-pin-labs]] — created; co-author affiliation (relevant to vault owner).
- [[peter-mcmahon]] — created; PI.
- [[tatsuhiro-onodera]] — created; co-first author.
- [[ryotatsu-yanagimoto]] — created via the companion paper; cross-listed here.
- [[programmable-photonic-computing]] — created as an overview tying this paper to its nonlinear companion.
