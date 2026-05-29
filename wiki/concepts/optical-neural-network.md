---
type: concept
name: "Optical neural network"
aliases: ["ONN", "photonic neural network"]
sources: [[2d-programmable-linear-waveguide-mcmahon]]
related: [[programmable-photonic-waveguide, programmable-photonic-computing]]
tags: [photonics, machine-learning, computing]
---

# Optical neural network

> A neural network whose linear (matrix-vector multiply) layers — and sometimes nonlinear activations — are executed by **light propagating through a photonic device**, instead of by digital electronics. Motivated by the prospect of dramatically lower per-MAC energy costs at scale.

## Origin

Long-running research direction; the modern revival is driven by the energy cost of deep-network inference. Early on-chip demonstrations used Mach–Zehnder interferometer (MZI) meshes (Shen et al., 2017) and microring banks. [[2d-programmable-linear-waveguide-mcmahon]] introduces the **continuous-substrate** alternative.

## How it works

A typical photonic MVM chip:

1. **Encode** the input vector x as optical amplitudes (one mode per element, or a single mode whose amplitude is time-multiplexed).
2. **Transform** the optical state through a programmable linear photonic network whose unitary (or sub-unitary, after loss) corresponds to the weight matrix W.
3. **Detect** the output as intensity per mode → entries of y = Wx (with detection performing |·|² nonlinearity).
4. Apply digital nonlinearity and feed into the next layer (hybrid optical/electronic), or chain optically with a nonlinear photonic block.

The **continuous-substrate** variant — [[programmable-photonic-waveguide]] — replaces the discrete photonic network with a single multimode slab whose refractive index distribution is the trainable parameter.

## Trade-offs / Contrasts with

- **MZI mesh** — well-understood, unitary by construction, but O(N²) wiring and component area; demonstrated N is far below the N ≳ 1,000 threshold for energy-efficiency advantage over electronics.
- **Microring banks** — wavelength-multiplexed, compact per channel, but thermal crosstalk and limited free-spectral-range constrain N.
- **Phase-change cells** — non-volatile but limited rewrite cycles (~4,000) and lossy.
- **Continuous programmable substrate** ([[programmable-photonic-waveguide]]) — better area scaling (~N^1.5 per the linear paper), no wiring bottleneck, but lower update rate and lower per-pixel Δn than ideal.
- **Free-space diffractive ONNs** — print or fab a fixed 3D structure; cheap and parallel, but not programmable post-fab.

## Open questions

- What's the smallest practical N at which **continuous-substrate** ONNs beat **MZI meshes** in some operationally meaningful metric (energy/op, accuracy/op, area/op)?
- How well do these chips perform under realistic training pipelines (online retraining, fine-tuning) given limited rewrite speed?
- Where does nonlinearity come from in deep optical networks? Detection nonlinearity, electronic interlayer, or programmable on-chip χ⁽²⁾ (cf. [[2d-programmable-nonlinear-waveguide-mcmahon]])?

## Related

- [[programmable-photonic-waveguide]]
- [[programmable-photonic-computing]]
- [[2d-programmable-linear-waveguide-mcmahon]]
