---
type: craft-export
title: "2025-05-22 zr co-sputtering literature review"
craft_document_id: 0B3F655E-F4C2-44AE-BCE6-283380A8A120
craft_collections: [fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-05-22 zr co-sputtering literature review
Because the Hf target has been delayed on arrival, we can try co-sputtering with Zr instead in the near-term.  The CNF has it in-stock, so that is a huge plus.  Below are some articles no sputtering ZrO2.

[High-rate reactive magnetron sputtering of zirconia films for laser optics applications](https://link.springer.com/article/10.1007/s00339-013-8214-1)

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-001.png)

At least they are very forward about ZrO2’s use in the UV range.

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-002.png)

They mention the arcing problem, which is nice.  Hf did not mention this, so I was getting worried

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-003.png)

Pressure = 2.5 mTorr and Ar flow is 20 sccms

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-004.png)

I don’t think we can replicate pulsed-DC in the AJA.  They also mention pre-sputtering, which is something we ought to probe Tom on (as we have observed transient solutions

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-005.png)

Interesting that higher temp promotes oxidation.  At some level, this completely makes sense, as higher temp promotes O2 to ionize, but it is nice to see it in writing

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-006.png)

Interested to note that N2 seems to reduce arcing, so this seems to give us an extra degree of freedom (N2 should stay fairly inert, so I would be surprised if much reacts into our film

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-007.png)

It seems that roughness of these pure ZrO2 films is about 1 nm.  We ought to measure the roughness of the other Al2O3 films we have made.  Either way, a trick for the future can always be polishing these films.

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-008.png)

Higher tempurature seems to help, at least generally speaking.  

[Understanding the discharge voltage behavior during reactive sputtering of oxides](https://pubs.aip.org/aip/jap/article/101/1/013301/916838/Understanding-the-discharge-voltage-behavior)

A paper more about how the dischage voltage changes with increased or decreased oxidation

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-009.png)

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-010.png)

The high level conclusion seems to be that different metals have different discharge voltage behaviours for different amounts of oxidation.

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-011.png)

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-012.png)

These plots are sputtering fully oxidized targets in pure Ar.  The time scale is not important, rather the fact that Al and Zr behave quite differently.

[Structural and optical properties of thin zirconium oxide films prepared by reactive direct current magnetron sputtering](https://pubs.aip.org/aip/jap/article/92/7/3599/485314/Structural-and-optical-properties-of-thin)

They DC sputter ZrO2 in a reactive plasma (so exactly what we are interested in).

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-013.png)

Almost all of the intuitions from Al reactive sputtering still apply, which is quite cool.  The only issue is the voltage bias direction is different

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-014.png)

They claim transition at 2.7 sccms of O2 flow.  This is kinda a useless number, as I would imagine it depends strongly on the other depositions parameters

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-015.png)

Quite surprisingly, it is very challenging to finesse the window for soitchiometric and near the transition region

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-016.png)

This is very useful, and confirms a lot of loss intuitions.  Sputtering in the oxidized regime gives films with lower density.  I imagine some of this can be addressed with furnace anneals, but the key point remains.  We will probably need to polish for the best performance

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0257897299005010?via%3Dihub)

They use pulsed DC.  Not the same, but something of a start

![Image.png](../../assets/fab/2025-05-22-zr-co-sputtering-literature-review-017.png)

The one thing that is qutie noticable is the high power.  That would explain the high sccm flow.