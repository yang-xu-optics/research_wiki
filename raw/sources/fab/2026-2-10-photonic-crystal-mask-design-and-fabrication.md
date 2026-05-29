---
type: craft-export
title: "2026-2-10 photonic crystal mask design and fabrication"
craft_document_id: 355C6D02-767C-4223-AD27-397F96EFBB7A
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2026-2-10 photonic crystal mask design and fabrication
## Mask Design

We are going to make our fourth mask.  We are going to seperate this into two sections:

1. Straight waveguides, waveguides with entrance tapers, and slowly varying adiabatic waveguides
2. Photonic crystal waveguides

The former are for known experiments (spatially adaptable poling, SPDC) and the latter is more of a test for future experiments.

I don’t personally feel a need to taper the input of these photonic crystal waveguides, so I will not do it

Below is what we expect the grating periods to be (we are only going to use first order

![Image.png](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-001.png)

408 is the period for 1565.  Below is the perutbration to the period of 1565 if our neff is wrong

![Image.png](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-002.png)

This is still well within the above range, so lets use 390 nm, 400 nm, 410 nm, 420 nm, and 430 nm.

Lets use perturbations between 5 um and 5.75, 6.5, and 7.25 um wide.  Lets make three of every waveguide and separate each linear period section.  All of these will be square.  The more important thing is we want to scan the perturbation length.

Below is the mask we have designed

[ASML_Pad4_pass2.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/725977CB-BB65-48B3-B411-5831271A6495_2/OvupimMnmzpdfDmHzAxJqZNwIMAvE1ob0Ruidif3Ic4z/ASML_Pad4_pass2.gds)

There are two sections: Photonic crystals on top and conventional structures on the bottom.  For the photonic cystals, I used lengths of 10, 50, 100, 500, 1000, and 5000 um for the grating.  I used grating periods of 390 nm, 400 nm, 410 nm, 420 nm, and 430 nm.  I made the baseline waveguides 5 um wide and the perturbation sections 5.75 um, 6.5 um, and 7.25 um wide.  Each waveguide was a different combination of the above.  I only made one of each waveguide on-chip, as they collectively take up a lot of space.

For the conventional devices, I made different baseline straight sections that were 3, 3.5, 4, 4.5, 5, 5.5, 6, 6.5, 7, 7.5, and 8 um wide.  This is for SCG, as I can control spectral broadening this way. I can also probably extract the sidewall loss from this array of structures.  I don’t want these to be tapered, as the taper will then dominate the spectral broadening.

Next, I have a section of straight waveguides that are 4, 5, and 6 um wide.  These have input tapers on both sides and could be useful for mode filtering the input and output.  I do the same thing above, but instead of having the tapers at the input and output, it is offset a bit away from the middle.  This makes input coupling easier and mode sorts later

The last section in the conventional devices are the slowly periodic adiabtic tapers (triangle-shaped).  These go between 5um and 10 um with periods of 250, 500, 750, 1000, 1250, 1500, 1750, and 2000 um.  This is to test whether we can do spatially adaptable poling (which we know we can do, just not the minimum feature size).  

Now lets figure out how to build Mandar’s taper for 785 nm.  Below is a simple 

## Fabrication

### Dose test

We were told that we should do a dose test on the mask.  While resolving our photonic crystal features should be possible on the ASML, apparently we are somewhat close to the tipping point of the Heidelberg as well.  We want to bias the mask such that the gratins have slightly wider Cr regions, as we will generally want to over dose than underdose.  We created a new pattern (attached below) that will allow us to dose test our gratings.  It varyins the height and duty ratio of different waveguides (though it keeps the period all at 400 nm)

[ASMLDoseTest2.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/CB406B9F-FCB8-4536-A856-7039414BD5B6_2/F4BURZ8cdeJlT93UhSOKMOWZJP97a857eutxsY1G8L8z/ASMLDoseTest2.gds)

We vary the dose in intervals of 5 (as that is all the tool allows) from 65 to 100. the Defocus is the default value of -12.  We did not quite seperate all the dies correctly, but we should still be able to see something

Dose of 90

Below are some of the best 5 to 5.3 differences 

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-003.jpeg)

Above DR 0.467

Wide 5.66, dr 0.422

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-004.jpeg)

For dose of 70

W 5.33, Dr 0.6

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-005.jpeg)

W 5.66, Dr 0. 476

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-006.jpeg)

Very consistently 0.467 is the best duty ratio. Like, almost irregardless of feature size . 

For dose of 95, it goes down to 0.3.

I say we use a dose of 80 with 0.467. Slightly larger features, perhaps use 0.422

For dose of 65, 0.512 is better for duty ratio

We will expose with 80 as the dose.  We will add some small duty ratio corrections (that very by size) to the DBR gratings

### Mask Exposure

Before exposing

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-008.jpeg)

Now for etching the Cr and developing

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-009.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-010.jpeg)

### ASML job creation

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-013.jpeg)

For the crystals job (which I believe should be done on a different wafer)

![Photo from Library.jpeg](../../assets/fab/2026-2-10-photonic-crystal-mask-design-and-fabrication-014.jpeg)