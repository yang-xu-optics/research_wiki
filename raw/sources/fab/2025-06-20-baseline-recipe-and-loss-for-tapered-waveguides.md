---
type: craft-export
title: "2025-06-20 baseline recipe and loss for tapered waveguides"
craft_document_id: 7CA1AE59-4B37-4AA8-A260-87A62519919D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-20 baseline recipe and loss for tapered waveguides
We have so far struggled to make low-loss waveguides for our tapered structures.   This is turning into a real pain.  We have so far only tried oxide hard mask recipes, and I am getting the suspiscion that something is off there.  The only difference between our previously owrking hard mask recipea dn the one we are doing now is the thickness of the resist mask.  While this might not sound like much, my hunch is that the CH2F2 etch reacts weirdly with ARC.  I don’t have a better explaination than that, as it is just a hunch.  It is sorta like how CH2F2 reacts weirdly with Cr.

Anyway, we are going to do two things to settle this loss issue once and for all:

1. Make an SVM wafer with 800 nm of resist on oxide hard mask.  Literally copy the extra recipe from before
2. Make an SVM wafer with 600 nm of resist on Cr hard mask (just copy the Cr recipe).  

At the very minimum, 2 is a process we have ues so often that I really feel like it will work.  If neither works, we know the issue is just the etcher.  We are going to use the tapered waveguide pattern.  We can us the power out of the straight waveguides as our baseline to compare the performance.  We expect roughly 5 mW out of the straight waveguides using the main setup, EDFA, and 10X at 1570.

As a future thing, I would also like to calculate the viability of using CHF3/O2 to etch the oxide instead of CH2F2/He.  I can’t explain why, but I feel like the latter recipe is a bit cursed.

We have found that 750 nm of oxide allows us to etch through 2000 nm of SiNx.  This means the selectivity is 2.66:1 for CHF3/O2/N2 for nitride to oxide.  This is good.  Another important note is we will probably do this etch for a minute shorter in the future, as we want to strip the top oxide anyway.  We ideally want 100 nm of SiNx left to protect the bottom oxide from BOE stripping.  We did a 6 minute etch, so we know oxide etched at roughly 125 nm/min (again, a bit of an estimate).  This means nitride etched at 325 nm/min, which is consistent with earlier findings for nitride.  We then know we etch oxide at 180 nm/min with CHF3/O2 and resist at 120 nm/min.  So we still want around 1000 nm of oxide, so we need 660 nm of resist.  This means we must use the thick resist recipe and not descum for too long.  It might be possible.  We would then leave the wafer in BOE for 5-10 mins to strip off any remaining hard mask.

In previous studies ([https://tdwg.craft.me/9TKpCasWHuS8oN](https://tdwg.craft.me/9TKpCasWHuS8oN)), we definitely hit the ARC using the CHF3/O2 etch, so this is not unprecedented there.  It seems, using our preovously working hard mask thicker resist, after 1:20 of descum, we get 700 nm of resist, which should give us 1000 nm of oxide.  At this point, we just hope to get lucky on selectivities.  It is defintiely a bit tight.

### Photolithography

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-001.jpeg)

Oxide top, Cr bottom 

Arc

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-002.jpeg)

We first run the thinner coating on the Cr wafer, so 600 nm

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-003.jpeg)

We then run recipe 1206 for thicker resist on oxide.  I don’t see any issues with ARC coating at the moment.  Resist coating was a little bit nonuniform, but this could have been from the markings left from the sputter.  I don’t think this is out of the ordinary from what I remember

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-004.jpeg)

Before thick resist

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-005.jpeg)

Before edge clear

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-006.jpeg)

During edge clear 1

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-007.jpeg)

During edge clear 2

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-008.jpeg)

We read mask

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-009.jpeg)

Before exposing Cr

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-010.jpeg)

During Cr

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-011.jpeg)

Before exposing oxide (use dose of 20) and changed all images

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-012.jpeg)

During oxide

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-013.jpeg)

Before developing 

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-014.jpeg)

Once more, Cr does. Not fully expose

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-015.jpeg)

Let’s do 1:20 descum on both and see what we get

### Etching

We clean 82 for 5. We now do 1:20 descum on both wafers

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-016.jpeg)

Plasma during process

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/71A3195C-8677-4B73-B0E4-3AE2DE3CD792_2/nIlp3D8yHvIEUlJukOmLlVF5I31GVTq00dLxuUlidhIz/Video%20from%20Library.mov)

45 seconds to a minute is needed to change color

Let’s measure resist thickness after on thick wafer

After 

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-017.jpeg)

Profilometer

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-018.jpeg)

Very consistent

5 days later, resist broadly seems fine

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-019.jpeg)

We will just do Cr wafer as truest baseline

100 during 5 min clean

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-020.jpeg)

Good cooling

We did a 4 minute season, then a 7 minute etch

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-021.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-022.jpeg)

After etch

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-024.jpeg)

This is ~100 nm shorter than last time.  Frustrating, but I don’t think this is critical.  Last time, I also looked around a waveguide, not a larger step.  We will just have to see.

I will also do a piranha clean of my wafer after the acid etching.  I don’t think it will hurt.  I won’t do eco clean in case the Cr oxidizes.  In theory, the eco clean should be fine, but I don’t want to play with fire.  I will then do 10 mins of smooth oxide deposition.

Before piranha clean

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-025.jpeg)

After Piranha

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-028.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-031.jpeg)

Still a bit of micro masking

Before Pecvd

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-032.jpeg)

### RTA

During calibration

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-033.jpeg)

During main

![Photo from Library.jpeg](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-034.jpeg)

Half the chips don’t have RTA

### Loss test on Cr

Edfa main setup 10x

3 um RTA die 1

Straight 1

3.9 mW

Straight 2

2.8 mW

Straight 3

2.5 mW

Straight 4

2.7 mW

Straight 5

1.5 mW

Euler 

0.5 mW

Circle short

0.2 mW



RTA 3um die 2

Straight 1

3 mW

Straight 2

3.5 mW

Straight 3

3.4 mW

Straight 4

3.2 mW

Euler

0.33 mW

Short circle

0.5 mW

Long circle

50 uW

![Image.png](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-035.png)

Not a perfect calculation, but ~2.5-3 dB/cm feels right to me



3 um no RTA die 1

Straight 1

1.7 mW

Straight 2

2.1 mW

Straight 3

2.2 mW

Straight 4

2 mW

Euler

0.18 uW

Short circle

100 uW

Long circle

30 uW

![Image.png](../../assets/fab/2025-06-20-baseline-recipe-and-loss-for-tapered-waveguides-036.png)

We don’t really need to run the 2um waveguides, as I can’t get the idea above.  We roughly get the idea that the waveguides are still pretty lossy.

Unless we see a mW out of these device, we have some issues.  The main challenge is we have seen at least 1 mW out of comparable Euler Spirals in the past.  We have definately had some waveguides with 2dB/cm look like this with euler spirals.  So if you think the loss is dominated by some bending behaviour there, then maybe it is not such a big deal. We did find the in the past that the circular spirals always did have lower loss than the euler spirals.  I guess I wish I had put a cicular spiral in the baseline die at the bottom.  Oh well.  This is roughly consistent with the values found here: [https://tdwg.craft.me/xR4W6jytzF1ND1](https://tdwg.craft.me/xR4W6jytzF1ND1).  We can somehwat glean that the oxide hard mask was not the issue, and ARC was not an issue either.

While I want to believe this is a mask-specific issue, there is a part of me that is starting to doubt the new SVM wafers.  I have a suspision they are inherently higher-loss.  This means we will need SRN3 more and more, which should have a lower loss in the RTA annealed state (at least less than 1 dB/cm).  I am also not quite willing to blame the bad cooling, as things have been rather consistent.