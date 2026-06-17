---
type: source
title: "Programmable on-chip nonlinear photonics"
authors: [Ryotatsu Yanagimoto, Benjamin A. Ash, Mandar M. Sohoni, Martin M. Stein, Yiqi Zhao, Federico Presutti, Marc Jankowski, Logan G. Wright, Tatsuhiro Onodera, Peter L. McMahon]
url: https://doi.org/10.1038/s41586-025-09620-9
date_published: 2025-10-08
date_ingested: 2026-05-28
source_file: raw/sources/articles/2026-05-28-programmable-2d-nonlinear-waveguide.pdf
kind: paper
tags: [photonics, nonlinear-optics, programmable-waveguide, silicon-nitride, quantum-photonics, mcmahon-lab, ntt-research]
---

# Programmable on-chip nonlinear photonics

> First demonstration of a **programmable 2D χ⁽²⁾ distribution** on a [[silicon-nitride|silicon nitride]] slab waveguide — arbitrary in-situ quasi-phase-matching gratings for second-harmonic generation, including real-time feedback against environmental drift — Nature Vol 649, 8 Jan 2026, pp. 330–. Companion to [[2d-programmable-linear-waveguide-mcmahon]] from the same group; the *nonlinear* counterpart.

## TL;DR

- Same programming trick as the linear paper ([[photoconductive-gain-programming]]) — patterned green light → photoconductor → spatial bias field — but instead of programming refractive index, it programs the **second-order nonlinearity χ⁽²⁾(x, z)** via electric-field-induced χ⁽²⁾ (i.e. 3χ⁽³⁾ E_bias).
- Substrate is **[[silicon-nitride|silicon nitride (SiN)]]** rather than lithium niobate. The χ⁽²⁾ here is *induced*, not intrinsic — SiN is centrosymmetric.
- Programmable [[quasi-phase-matching]] (QPM) gratings in 2D enable arbitrary control of **broadband [[second-harmonic-generation]]** — spectral shape, spatial output mode, and joint spatio-spectral structure.
- Demonstrated **real-time feedback** that compensates for pump-wavelength random walk by retuning the QPM grating period — breaks the "one device, one function, fixed at fab" model.
- Demonstrated **in-situ inverse design**: optimize the QPM grating on the chip itself against the measured response — robust to fabrication imperfections.
- Specs: dynamic range 0.47 pm V⁻¹; spatial resolution 7.5 µm; active area ~0.7 × 0.4 cm; update rate ~1 Hz (projector-limited; device RC limit is ~20 Hz).
- Stack: Si substrate + SiN waveguide (2.05 µm core, 1 µm SiO₂ cladding) + 7.5-µm SRN photoconductor + 20 nm ITO transparent electrode.

## Key claims

- **Nonlinear photonics has been "one-device, one-function" by necessity.** χ⁽²⁾ structure has to be sculpted by nanofabrication (periodically poled lithium niobate, orientation-patterned epitaxy). Each chip serves one wavelength / function and is sensitive to fab and environment.
- **Electric-field-induced χ⁽²⁾** lets a centrosymmetric material like [[silicon-nitride|SiN]] host a programmable χ⁽²⁾, with the program living in a control field rather than the crystal.
- **Photoconductive virtual electrodes** allow that control field to be patterned in 2D with thousands of effective DOF, without lithography of electrode arrays. Same core idea as the linear paper, applied to a different physical effect (χ⁽²⁾ vs Δn).
- **2D programmability of χ⁽²⁾** — not just 1D longitudinal periodic poling — is the new capability. Prior reconfigurable QPM was limited to 1D geometries.
- **Three engineering knobs demonstrated:** spectral (vary period along z), spatial (vary transverse structure), spatio-spectral (vary both).
- **In-situ inverse design and real-time feedback** make the chip *adaptive* to fab tolerances and operating drift — historically a major yield/reliability problem in nonlinear photonics.
- Application targets named: programmable optical **quantum gates** and quantum-light sources, all-optical signal processing, optical computation, adaptive structured light for sensing.

## Notable quotes

> "The function of a nonlinear-optical device is typically determined during design and fixed during fabrication, restricting the use of nonlinear optics to scenarios in which this inflexibility is tolerable."

> "We can break from the conventional one-device–one-function paradigm."

> "The all-optical approach reconfigures the spatial pattern of nonlinearity depending on how the device is optically pumped."

## Open questions

- Dynamic range 0.47 pm V⁻¹ is modest vs intrinsic χ⁽²⁾ of, e.g., periodically poled lithium niobate. What's the path to closing the gap?
- 1 Hz update rate (projector-limited) and 20 Hz device RC limit — what blocks operating at, say, kHz? Implications for closed-loop quantum control are significant.
- The quantum-gate application is named as a goal, not demonstrated. What's the gap?
- How well does this stack tolerate the high optical powers needed for some target NLO applications?
- Could a **single** stack do *both* the linear (Δn) and nonlinear (χ⁽²⁾) program by combining the lithium niobate and SiN approaches?

## Pages updated by this ingest

- [[programmable-photonic-waveguide]] — updated; this paper is the nonlinear sibling.
- [[photoconductive-gain-programming]] — updated; SiN/SRN/ITO stack details added.
- [[quasi-phase-matching]] — created; the central NLO technique programmed here.
- [[second-harmonic-generation]] — created; the demonstration NLO process.
- [[ryotatsu-yanagimoto]] — created; lead author on this paper.
- [[peter-mcmahon]] — updated; corresponding-author on both papers.
- [[mcmahon-lab-cornell]] — updated.
- [[ntt-research-pin-labs]] — updated.
- [[programmable-photonic-computing]] — updated; this paper anchors the "nonlinear" arm of the program.
