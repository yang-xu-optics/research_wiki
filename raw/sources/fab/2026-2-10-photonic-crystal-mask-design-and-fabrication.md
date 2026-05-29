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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/c8dec36e-65aa-c4b3-6ed3-3e60cf5995d5/2Nt1mqFtuecfYfyOFtt8dJ8u3TlFfVtTuL08TdTKJw8z/Image.png)

408 is the period for 1565.  Below is the perutbration to the period of 1565 if our neff is wrong

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/5fba2a3d-d678-4616-568a-98100c93c542/mf5Fny1irL2Et8LkTxhDk1XmXuclqpxeQeJd1GsN7dMz/Image.png)

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

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/76B746F3-4EDB-4DA5-9B6B-2478A6F15E61_2/2RqAF6xjPe31WOJ6kmcABJ2u1xKmrz9PjKlVFKpxowYz/Photo%20from%20Library.jpeg)

Above DR 0.467

Wide 5.66, dr 0.422

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/C6C64FDA-B21C-45F4-BA24-C55BE147CFC8_2/TnTnoJ7wSMDC7ZjMcHwRfMFp3I4qO86jxH3SvYQ9Sqwz/Photo%20from%20Library.jpeg)

For dose of 70

W 5.33, Dr 0.6

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/9276E2FE-E123-41EA-9E91-B9E41C7BDFBD_2/VOy9xR6Md4r2bua8uluUUkfKecN0fONkPygnMpjy8Wcz/Photo%20from%20Library.jpeg)

W 5.66, Dr 0. 476

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/61EC0AEB-D7E4-479B-B781-F9B31A8C220B_2/erMk5HyZXWtoSvTk8uZ8ZcMKJgH4GlbEeU72rFipXOAz/Photo%20from%20Library.jpeg)

Very consistently 0.467 is the best duty ratio. Like, almost irregardless of feature size . 

For dose of 95, it goes down to 0.3.

I say we use a dose of 80 with 0.467. Slightly larger features, perhaps use 0.422

For dose of 65, 0.512 is better for duty ratio

We will expose with 80 as the dose.  We will add some small duty ratio corrections (that very by size) to the DBR gratings

### Mask Exposure

Before exposing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/71098222-291C-415B-BF2F-7535531928DA_2/PVPp09iBtxbGcqHWRfY7WDDCWAe0QrsUyW1AtWfQgPUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/6A5D0100-4791-4133-8818-68739CEB5904_2/z73GYoGRKMCyP8hnFTCm41kcCpOVc9dnwcCUxMbJkRwz/Photo%20from%20Library.jpeg)

Now for etching the Cr and developing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/EF6D051D-6485-4321-B86C-0ACF1D5E399D_2/HJXca2U4BXCE2DV7o09KbLfIMdzh7oVv8h36ICbnM6cz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/87877E04-519B-44BB-AF3B-D7766E265CFA_2/GoOKEAh5xh7ovyTnCr2619zj3vUpYWc5wKB7eCq0b4Mz/Photo%20from%20Library.jpeg)

### ASML job creation

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/CAC94A7A-8835-4594-8877-CC0D66F53C67_2/lOa2Bdlep4LIf2L72BRj8UsXHiM5lU1GRtAuybzHkRUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/47355727-A25F-48A4-8542-63420E578B62_2/FB3KK2AhKGRQ4ZMo6OUxLlw9PuMXXKynMdO7NnxzjBoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/C2992C60-70E7-4CCF-8C32-36A8A2937464_2/LOUhXBu0RfAPPx3jQQRGkzxwVK92dQbW0CuIQmLqLkQz/Photo%20from%20Library.jpeg)

For the crystals job (which I believe should be done on a different wafer)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/355C6D02-767C-4223-AD27-397F96EFBB7A/28A2F81F-2C91-4F2B-A00E-3C463DF49C18_2/YJkeLVvbiknTMhDOvqqAaSN4UBsZZxXpomrohE6zE9oz/Photo%20from%20Library.jpeg)