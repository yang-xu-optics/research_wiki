---
type: concept
name: "Electro-optic effect"
aliases: ["Pockels effect", "EO effect", "linear electro-optic effect"]
sources: [[2d-programmable-linear-waveguide-mcmahon, carrier-induced-index-iii-v-bennett, low-voltage-high-power-algaas-mzi-bhasker]]
related: [[electro-optic-modulation, lithium-niobate, iii-v-integrated-photonics, programmable-photonic-waveguide]]
tags: [photonics, electro-optics, modulation]
---

# Electro-optic effect

> The electro-optic effect is the change of a material's optical refractive index under an applied electric field. In this vault it connects [[lithium-niobate]] programmable waveguides, [[electro-optic-modulation|EO modulators]], and possible reconfigurable III-V photonic devices.

## Origin

The Pockels effect is the linear electro-optic response found in non-centrosymmetric materials such as lithium niobate and many III-V semiconductors. Carrier-induced index change is a separate but adjacent semiconductor mechanism for electrically or optically controlled phase shifts — [[carrier-induced-index-iii-v-bennett]].

## How it works

An applied field changes the refractive index, which changes optical phase accumulation. In an MZI, that phase shift becomes an intensity modulation. In a [[programmable-photonic-waveguide]], a spatially patterned field can become a spatially patterned optical medium.

## Trade-offs / Contrasts with

- vs carrier-induced modulation — Pockels modulation can be fast and low-loss, while carrier effects can be strong but often introduce absorption or speed/energy trade-offs.
- vs thermo-optic tuning — EO tuning can be much faster and lower energy, but needs suitable materials and electrodes.
- vs [[photoconductive-gain-programming]] — photoconductive gain is a way to spatially deliver a large field; the EO effect is one possible optical response to that field.

## Open questions

- Can EO tuning become a large-scale programmable control plane rather than a collection of local phase shifters?
- Which platforms best combine EO response with low loss, strong nonlinearity, and active integration?

## Related

- [[electro-optic-modulation]]
- [[lithium-niobate]]
- [[iii-v-integrated-photonics]]
- [[programmable-photonic-waveguide]]

