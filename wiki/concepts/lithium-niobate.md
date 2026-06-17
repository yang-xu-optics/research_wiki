---
type: concept
name: "Lithium niobate (LiNbO₃)"
aliases: ["LiNbO3", "LN", "TFLN", "thin-film lithium niobate"]
sources: [[2d-programmable-linear-waveguide-mcmahon]]
related: [[programmable-photonic-waveguide, electro-optic-effect, quasi-phase-matching]]
tags: [material, photonics]
---

# Lithium niobate (LiNbO₃)

> Ferroelectric crystal that is the **workhorse material of modern integrated photonics**: strong Pockels (electro-optic) effect, high χ⁽²⁾ nonlinearity, transparency from visible into mid-IR, and a mature thin-film integration story (TFLN). The slab waveguide material in [[2d-programmable-linear-waveguide-mcmahon]].

## Origin

Synthetic crystal grown by Czochralski pulling since the 1960s. Discrete LiNbO₃ modulators have dominated long-haul telecom for decades. **Thin-film lithium niobate** (TFLN) on insulator — wafer-bonded thin LiNbO₃ on SiO₂/Si — became viable in the late 2010s and enabled compact, high-confinement integrated-photonic devices.

## How it works (relevant properties)

- **Pockels (linear electro-optic) effect.** Refractive index changes linearly with applied E-field: Δn = (½) n³ r_eff E. The r_eff of LiNbO₃ (~30 pm/V for r₃₃) is among the highest in commonly-available materials. Exploited in [[2d-programmable-linear-waveguide-mcmahon]] to program Δn ~10⁻³ via patterned bias fields.
- **χ⁽²⁾ nonlinearity.** Non-centrosymmetric crystal → intrinsic, large χ⁽²⁾ (d₃₃ ~25 pm/V). Periodically poled LN (PPLN) is the dominant medium for quasi-phase-matched [[second-harmonic-generation|SHG]] and other χ⁽²⁾ NLO.
- **Transparency window.** ~350 nm to ~5 µm — covers VIS, NIR (telecom), and most of MIR.
- **Z-cut, X-cut, MgO-doped variants** trade off electro-optic vs nonlinear performance and photorefractive damage thresholds.

In the [[2d-programmable-linear-waveguide-mcmahon|McMahon linear paper]], a Z-cut LN slab with SiO₂ cladding sits between a Si substrate (ground) and a gold top electrode, with a photoconductive layer mediating optical programming — see [[photoconductive-gain-programming]].

## Trade-offs / Contrasts with

- vs **silicon photonics** — Si lacks both a useful Pockels effect and intrinsic χ⁽²⁾ (centrosymmetric); LN provides both. But Si has cheaper, more mature fab.
- vs [[silicon-nitride]] — SiN is low-loss and CMOS-compatible but lacks Pockels and χ⁽²⁾; [[2d-programmable-nonlinear-waveguide-mcmahon]] gets around the χ⁽²⁾ gap by *inducing* it electrically.
- vs **III–V semiconductors (InP, GaAs)** — those host gain (lasers) but worse passive losses than LN.

## Open questions

- Photorefractive damage at high optical intensity in undoped LN — does the McMahon stack architecture mitigate or exacerbate this?
- Scaling Δn beyond 10⁻³ in TFLN without dielectric breakdown of the surrounding stack.

## Related

- [[programmable-photonic-waveguide]]
- [[electro-optic-effect]]
- [[quasi-phase-matching]]
- [[2d-programmable-linear-waveguide-mcmahon]]
