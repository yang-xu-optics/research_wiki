---
type: concept
name: "Silicon nitride on sapphire"
aliases: ["SiNoSa", "SiN on sapphire", "Si3N4 on sapphire"]
sources: [[crack-free-silicon-nitride-on-sapphire-lu]]
related: [[silicon-nitride, wide-band-photonics]]
tags: [photonics, materials, silicon-nitride, sapphire]
---

# Silicon nitride on sapphire

> Silicon nitride on sapphire is a photonics platform that grows stoichiometric LPCVD [[silicon-nitride|Si3N4]] directly on sapphire rather than oxidized silicon, using sapphire's thermal expansion behavior to reduce residual tensile stress and avoid cracking in thick films.

## Origin

The paper traces the idea to earlier low-stress Si3N4-on-sapphire work and a recent telecom photonics demonstration, then adds systematic stress, material, and device measurements across multiple wavelengths — [[crack-free-silicon-nitride-on-sapphire-lu]].

## How it works

The mechanism is mechanical rather than optical:

- LPCVD Si3N4 is deposited at high temperature with intrinsic tensile stress.
- During cooldown, oxidized silicon shrinks less than Si3N4, effectively adding tensile stress to the film.
- Sapphire shrinks more than Si3N4, which the authors argue relieves residual tensile stress during cooldown.
- Lower residual stress lets thick stoichiometric films survive dicing and processing without trench-line or tiling-pattern crack stops.

The reported experimental anchor is crack-free growth up to about 1960 nm, with residual tensile stress near 200 MPa. A 620 nm film was fabricated into microring devices and measured at visible, near-IR, and telecom/U-band wavelengths — [[crack-free-silicon-nitride-on-sapphire-lu]].

## Trade-offs / Contrasts with

- vs Si3N4 on oxidized silicon — lower stress and thicker crack-free films, but a less conventional substrate for packaging and electronic integration.
- vs damascene Si3N4 — simpler direct growth without crack-management structures, but it still needs device-level process optimization for ultra-low-loss applications.
- vs PECVD SiN — keeps stoichiometric LPCVD material quality, while PECVD offers lower stress through a different deposition route with more material variability.

## Open questions

- Will the same stress behavior hold across larger wafers and foundry process windows?
- How much do sapphire's transparency and etch resistance help or hinder real device flows?
- Can the platform support heterogeneous integration with active materials, heaters, electrodes, or photoconductive stacks?

## Related

- [[silicon-nitride]]
- [[wide-band-photonics]]
- [[nist]]

