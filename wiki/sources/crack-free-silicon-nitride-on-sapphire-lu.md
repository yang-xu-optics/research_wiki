---
type: source
title: "Direct growth of crack-free stoichiometric silicon nitride on sapphire for wide-band photonics"
authors: [Zhaohui Ma, Ashish Chanana, Zhiquan Yuan, Khoi Hoang, Yiliang Bao, Daron Westly, Kartik Srinivasan, Xiyuan Lu]
url: null
date_published: 2026-06-17
date_ingested: 2026-06-17
source_file: raw/sources/articles/2026-06-17-crack-free-silicon-nitride-on-sapphire.pdf
kind: paper
tags: [photonics, silicon-nitride, sapphire, integrated-photonics, wide-band-photonics, nist]
---

# Direct growth of crack-free stoichiometric silicon nitride on sapphire for wide-band photonics

> Materials/platform paper arguing that [[silicon-nitride-on-sapphire|SiN on sapphire]] can keep the low-loss, wide-band advantages of [[silicon-nitride]] photonics while avoiding the high tensile-stress cracking problem of thick LPCVD Si3N4 on silicon.

## TL;DR

- The paper compares stoichiometric LPCVD [[silicon-nitride]] on fused silica, oxidized silicon, and sapphire, and argues that sapphire's larger coefficient of thermal expansion relieves residual tensile stress during cooldown.
- On oxidized silicon, stoichiometric LPCVD Si3N4 sits near 900-1100 MPa tensile stress and tends to crack above roughly 350-400 nm; on sapphire, the authors report crack-free films up to about 1960 nm with roughly 200 MPa stress.
- The result is positioned as a foundry-friendly route to thick, low-stress, stoichiometric Si3N4 without trench lines, tiling patterns, damascene processing, or other stress-mitigation structures.
- Fabricated microring devices on 620 nm Si3N4/sapphire show propagation losses on the order of 0.2-0.4 dB/cm across visible, near-IR, and telecom/U-band measurements, comparable to established Si3N4-on-silicon platforms.
- The platform is pitched for [[wide-band-photonics]] use cases where transparent sapphire, visible/deep-visible operation, mid-infrared reach, and thick direct wafer-scale Si3N4 are attractive.

## Key claims

- **The stress problem is substrate-driven.** Silicon's coefficient of thermal expansion is smaller than Si3N4's, so cooling from LPCVD temperatures adds tensile stress to the film; sapphire shrinks more and reduces the residual tensile stress instead.
- **Stress mitigation is a workaround, not a cure.** Trench lines, tiling patterns, rotate-and-grow processes, and damascene flows can confine cracks or enable thicker waveguides, but they add process complexity and do not universally lower the film stress in an unpatterned wafer.
- **Sapphire changes the thickness regime.** The authors report direct growth of crack-free stoichiometric Si3N4 up to nearly 2 micrometers on sapphire, with stress staying near 200 MPa rather than rising with thickness.
- **The optical platform remains competitive.** Ring-resonator losses at 775 nm, 1062 nm, and telecom/U-band wavelengths are in the same broad range as comparable Si3N4-on-silicon devices made with similar recipes; reported values cluster around 0.2-0.4 dB/cm depending on wavelength and fitted mode.
- **The most likely platform advantage is not just lower loss.** The differentiators are process robustness, thick films without crack-management structures, sapphire transparency, and potential access to deep-visible and mid-infrared regimes.

## Notable quotes

> "We advocate silicon nitride on sapphire" — Introduction

> "No cracks even near the diced edges" — Fig. 3 caption

## Open questions

- How does the platform perform on full foundry-scale wafers rather than diced pieces and 4-inch wafers?
- Does sapphire introduce packaging, thermal, RF, or heterogeneous-integration constraints that offset the stress advantage?
- Can losses below 0.1 dB/cm be reached on this stack with sidewall smoothing, annealing, or damascene-style process refinements?
- How far into the deep-visible and mid-infrared can the practical low-loss window extend once cladding, coupling, and packaging are included?

## Pages updated by this ingest

- [[silicon-nitride]] — created; general Si3N4 photonics material page.
- [[silicon-nitride-on-sapphire]] — created; platform concept introduced by the paper.
- [[wide-band-photonics]] — created; application frame used throughout the paper.
- [[zhaohui-ma]] — created; first author.
- [[kartik-srinivasan]] — created; corresponding author.
- [[xiyuan-lu]] — created; corresponding author.
- [[nist]] — created; author affiliation and fabrication context.
- [[joint-quantum-institute]] — created; author affiliation.
