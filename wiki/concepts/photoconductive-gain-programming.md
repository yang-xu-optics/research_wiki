---
type: concept
name: "Photoconductive-gain programming"
aliases: ["photoconductive programming", "virtual electrode programming"]
sources: [[2d-programmable-linear-waveguide-mcmahon, 2d-programmable-nonlinear-waveguide-mcmahon]]
related: [[programmable-photonic-waveguide, lithium-niobate]]
tags: [photonics, programmability, mechanism]
---

# Photoconductive-gain programming

> A way to spatially program a high-voltage bias field across a photonic chip using **patterned light** instead of lithographically patterned electrode arrays. A photoconductor layer becomes locally conductive where it is illuminated, switching a single uniform bias voltage onto thousands of "virtual electrodes" simultaneously — the shared mechanism behind both McMahon-group [[programmable-photonic-waveguide]] papers.

## Origin

The principle of photoconductive gain has been used for decades (e.g. in detectors and image sensors). Its use as a *programming* mechanism for photonic computing chips was scaled to 2D and ~10⁴ degrees of freedom in [[2d-programmable-linear-waveguide-mcmahon]] (refractive index) and [[2d-programmable-nonlinear-waveguide-mcmahon]] (χ⁽²⁾ nonlinearity).

## How it works

Stack: substrate (also serves as ground electrode) → optical waveguide → photoconductor → transparent top electrode (e.g. ITO). A bias voltage is applied across the whole stack via a single pair of electrodes.

1. In the dark, the photoconductor has high impedance; most of the bias voltage drops across it; very little reaches the waveguide.
2. Where a projected light pattern illuminates the photoconductor, its impedance drops sharply. The voltage divider shifts: most of the bias now drops across the waveguide in that region.
3. The result is a spatially patterned bias electric field E_bias(x, z) inside the waveguide that mirrors the projected illumination pattern.
4. That spatially varying field modulates an optical property of the waveguide (Δn via [[electro-optic-effect|Pockels]] in lithium niobate; χ⁽²⁾ via electric-field-induced nonlinearity in SiN).

**Why it matters:** standard CMOS backplanes can only deliver ~10 V per pixel. The photoconductor lets a single uniform 1,000 V be applied across the stack while still being "switched in" optically at ~10⁴ sites. This is what makes large Δn (~10⁻³) and meaningful χ⁽²⁾ programmability achievable at large N.

## Trade-offs / Contrasts with

- vs **lithographically patterned electrode arrays** — eliminates the O(N²) wiring problem and the need for a CMOS backplane bonded to the photonic chip.
- vs **directly modulating with the programming light** (photorefractive crystals) — decouples the *physical* effect (Pockels / EFI-χ⁽²⁾) from the *programming* effect, so the achievable Δn or χ⁽²⁾ isn't bottlenecked by the photorefractive coefficient.
- **Update-rate cost:** the RC time of the photoconductor stack limits how fast the pattern can be rewritten — ~20 Hz device limit in [[2d-programmable-nonlinear-waveguide-mcmahon]], with the actual demonstrations slower due to projector limits.
- **Resolution cost:** fringing fields between bright and dark regions blur the projected pattern; effective minimum feature size ~7.5 µm in the nonlinear paper, ~9 µm in the linear paper.

## Open questions

- What's the practical path to kHz update rates? Thinner photoconductor? Different photoconductive material?
- Could the same stack be designed to support **both** linear (Δn) and nonlinear (χ⁽²⁾) programming?
- Long-term reliability under sustained 1,000 V bias and high optical pump power.

## Related

- [[programmable-photonic-waveguide]]
- [[electro-optic-effect]]
- [[lithium-niobate]]
