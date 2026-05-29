---
type: craft-export
title: "2026-01-26 first photonic crystal fabrication and testing"
craft_document_id: 7277444A-3193-4640-807B-8C7E67D3BB45
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2026-01-26 first photonic crystal fabrication and testing
As our last experimental demonstration, we want to show phase-matching on photonic-crystal waveguides.  Presumably I will start with phase matching on straight waveguides again (with better alignment of the illumination optics), but this will immediately follow.  

Here is our first GDS design

[Photonic_Crystal_pass2_final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/43657C18-F81E-4525-81F6-1006B8BF1640_2/9eyrcOYji5UC7hmgh728LkZflGcBg9gkNLL7Ylski3Ez/Photonic_Crystal_pass2_final.gds)

This pattern really looks at the size of the perturbation.  There is something to be said different doses can kinda screw with this, but to first order, we can use a dose that is roughly right and move forward with that.  While we do look at different grating periods, it is fair to say that we could scan that more.  I generally just trust my simulations as being pretty close (and other literature papers for much smaller waveguides are close-ish).  Afterall, the way you calculate this period is actually pretty simple, and the period is not super super sensitive to the errors we are likely to use in the neff.

This experiment hopes to observe a photonic bandgap using the 10th order diffraction mode.

## Fabrication

Below is the fabrication we plan on using

1. Spin clean the wafer (we don’t need RCA, as losses won’t be tragic for us)
2. Deposit 6:35 mins of PECVD smooth oxide to get 1.1 um hard mask
3. Spin coat 1805 resist using 2000 rpm, 8000 ramp, and 45 seconds. We know we have an etch selectivity of 4:1, and we want to etch through 1um of oxide.  So we want at least 300 nm of resist.  I think this thickness should work, but just…
4. We will develop the wafer using the hamatech tool.  We used recipe 6 in the past (MIF726 for 1 min).  Just check the number
5. Descum for 45 seconds on oxford 81 (I know we usually do 1:15, but I feel like 90 nm should be good enough)
6. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe (it seems we raised this time slightly from 7-1 to the 7-30 deposition)
7. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
8. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
9. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition

I would just check resist thickness after development and after descum to confirm that we can clear.

Below is Ellipsometer of starting SVM wafer

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-001.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-002.jpeg)

### Top oxide depostion

I cleaned the chamber for 6 mins and seasoned for 1

Before top cap dep

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-003.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-004.jpeg)

Before second dep on different wafer

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-005.jpeg)

we do a 10 min clean and are going to season again for 1 min before doing the last wafer.

Before last dep

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-006.jpeg)

Ellipsometery check

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-008.jpeg)

Just some misc notes about organization 

Below is the SVM box

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-009.jpeg)

Middle three are SVM with oxide. Back are just SVM. Front is not fitting, but I suspect it’s 800 nm SRN3

### Lithography

Below is the thickness we expect

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-010.jpeg)

So 1805 at 2000 should be good

we used 2000_8000_45 for spin coat, and 90 C for 1 minute to bake

Before exposure

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-011.jpeg)

We develop with recipe 4

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-012.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-016.jpeg)

There is an obvious blur, but that could be from over exposure or bad MLA. I say we continue.  This goes to show we will have to be more deliberate about dose tests in the future, but the period should be right (which is most important).  And we should get qualitative feedback on what perturbation size is best. 

### Etching

We run 5 min pre clean on 81 and 100.

Before oxide etch season

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-017.jpeg)

Before descum

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-018.jpeg)

The He flow on the etcher seems fine

Profilometer for resist thickness

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-019.jpeg)

At 550, we will make it

As a note, before the etch below, we wiped off the edge bead (almost forgot this, as I am used to ASML doing it for me)

Before oxide etch

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-020.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-021.jpeg)

He flow is a bit high, but we are getting a seel still. Settled closer to 4.7

We now run a 7 minute clean on 100.  Ontop EcoClean for the wafer

Before eco clean starts

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-022.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-023.jpeg)

Before nitride season

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-024.jpeg)

Thickness of oxide

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-025.jpeg)

Basically spot on

We are going to skip piranha for now

Before nitride etch

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-026.jpeg)

During nitride etch

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-027.jpeg)

Thickness of nitride

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-028.jpeg)

2.4 um, so we still had oxide

Images

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-031.jpeg)

I am not sure how nice our tapers are

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-032.jpeg)

Given that some of the tapers look a bit funny, I am going to cleave around them for some of the chipes.

I am going to anneal 2 non-cladding pieces, and all the cladded pieces

### Top Cap

We now run 6 min clean and 1 min season for oxide.  We will run 16 min dep to get ~2.5um of oxide

Before cap

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-033.jpeg)

During RTA calibration

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-034.jpeg)

Image of non cladded waveguides with annealing

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-037.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-038.jpeg)

Now with cladding

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-040.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-042.jpeg)

### Supplemental Dose test

We are going to run a followup-dose test to figure out what is the best dose, as I really should know the geometry

We will scan from 40 as the dose to 60.  We did 2000_8000_45, and 90C for 1 min.

Before starting

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-043.jpeg)

We run this process on 1 um of thermal oxide wafer.  We did use optical focus for this, so that is one difference

Exposure starts in top left

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-044.jpeg)

Second is on the row of 4

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-045.jpeg)

So it scans across a row first, then does different rows 

We use program 4 to develop

Taper on top left

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-046.jpeg)

Each division is 2um

5 by 8, period 4

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-047.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-048.jpeg)

Third, top row

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-049.jpeg)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-050.jpeg)

Taper

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-051.jpeg)

This taper is def a bit less then 2um

Bottom first

Taper

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-052.jpeg)

Crystal

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-053.jpeg)

Further over (largest dose)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-054.jpeg)

We might have had functional tapers, but they would have been small (and this was was optical, not pneumatic, so that is also a difference)

![Photo from Library.jpeg](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-055.jpeg)

## Testing

Skip the first 20 waveguides at the bottom, they are straight

Next couple vary length.  We should skip those for now too.  there are 16 of those

Using the camera, below is what

![Image.png](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-056.png)

With a finer scan

![Image.png](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-057.png)

![Image.png](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-058.png)

This is a touch annyoing, as I don’t see an obvious discontinuity.  Then again, this background has always been a problem.

Some issue is the stopband (With the worse index contrast and lower resolution) is our stop band could be really really small.  Again, we are looking for a distinct drop in tranmission, something that looks discontinuous.

If I were thinking of what could have gone wrong, below are some hypothesis:

- Because we are over-exposed (and the MLA struggles to resolve small features anyway) we truly might have very small features at the spatial frequencies we want.
- MLA increases resist roughness, which increases loss (this point I think goes undermentioned, but we only saw a maximum of 100 uW instead of several mW.  Meaning, at least a factor of 10 higher loss.  I suspect we need smaller perturbation sizes, as we were not able to see any light in the 5-8 um devices.  I suspect that using 5-6 um is probably safer)
- Our waveguides could be a lot narrower than we suspect, which could cause the dispersion to be much different than suspected (though we did test several periods, and we know that we have a decent amount of room for wiggle room with index).

We generally see that people use first-order diffraction, so it is perhaps posible that getting higher-order terms to work for us was just going to be too hard.  We should still investigate second or third order diffraction, as they are only removed from the fundamental period by 1/2 or 1/4.  Basically, they should be noticable.  I am generally less willing to believe that we were super off on the expected period, as most periods I see only are very close to what I used.  The size of our perturbation was not insane either, but most people use DBR structures that are much shorter than ours.  I guess it is possible that our DBRs were too effective, but I kinda doubt that.

We should take a picture of our waveguides with no cladding under SEM.  I want to see our exact feature size and look at the dose test as well.  I don’t think we will be able to use the MLA to get these made.  On our ASML mask, we should also leave a section for normal periodic tapered waveguides, as that is just a nice experiment to include.  

For the next fab, I would indeed try to use the ASML.  I would only have two waveguides of each type and I would make the photonic crystals much shorter.  Of course, the issue with this is that the dispersive section might be so short that we hardly notice on the nonlinear scan.  I could just see this being hard is all.  We will of course want to use the EDFA, but in some sense using higher-order diffraction was a saving grace for this.

Lets try something where we vary the length of our waveguides.  We should try something where we use waveguides that are 10 um of perturbation, 50um of perturbation, 100 um of perturbation, 500 um of perturbation, 1 mm of perturbation, 5 mm of perturbation, and 1 cm of perturbation.  We will make waveguides default 5um wide just to be safe.  I would also choose to make waveguides either 6.25 um wide or 7.5 um wide for the larger sections.  We can otherwise very the grating between 3.8um and 4.3 um (with iterations of 0.1 um).  I will double check the period length later.

Below are the SEM images.

Narrow = 5, Wide = 8 (I think the period for all of this is about 4)

![Etched_N5_W8_P3.900.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-059.tiff)

![Etched_N5_W8_P4.501.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-060.tiff)

![Etched_N5_W8_P4.502.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-061.tiff)

![Etched_N5_W8_P4.503.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-062.tiff)

![Etched_N5_W8_P4.504.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-063.tiff)

Narrow = 4, Wide = 5

![Etched_N4_W5_P4.507.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-064.tiff)

![Etched_N4_W5_P4.508.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-065.tiff)

Sidewalls of etched devices

![Etched_sidewall10.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-066.tiff)

For the lithography test, everything seemed to be the same size.  Nonetheless, below are the dimensions for the things we exposed

![Litho_7_N5_W8_P418.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-067.tiff)

![Litho_7_N5_W8_P419.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-068.tiff)

And sidewalls (though they are a bit more blurry)

![Litho_Sidewall22.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-069.tiff)

![Litho_Sidewall23.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-070.tiff)

![Litho_Sidewall24.tiff](../../assets/fab/2026-01-26-first-photonic-crystal-fabrication-and-testing-071.tiff)

A lot of the roughness I see after the etch I don’t see on the resist.  So our sidewalls are pretty shitty, and this is probably because we are etching so far down.

So now we really want to focus on designing the new GDS.  Firstly, Mandar had a really nice suggestion that we ought to have a wide input coupling region, but then have short tapers.  This should really help us mode-filter.