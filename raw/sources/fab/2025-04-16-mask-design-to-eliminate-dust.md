---
type: craft-export
title: "2025-04-16 mask design to eliminate dust"
craft_document_id: 6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-16 mask design to eliminate dust
Despite our persistent efforts, we will have dust after SiNx etching with a Cr hard mask in the oxford 100.  It would be nice to figure out the optimal etching process so we can easily design new waveguides in future runs.  Below is what we have observed:

1. After a 12:45 etch of oxide in the oxford 100 (no mask), we don’t see any dust
2. After a 9.5 etch of nitride in the oxford 100 (resist mask), we don’t see any dust
3. After a 10.5 etch of nitride in the oxfrod 100 (Cr mask wet and dry patterned), we see dust
4. Using the oxford 82 for 25 mins for fused SiO2 (Cr mask wet patterned), we don’t see dust

So there seems to be something about Cr in the 100 that is the issue.  So we are going to try two new approuches:

1. Thick pad oxide with resist on top.  We use the resist to set the step height, but we intentially etch through the resist so we don’t need to deal with the impossible task of removing it later.  We also have resist on top of oxide to minimize any optical loss.  We etch with oxford 100.
2. Use our existing mask design, but etch in the oxford 82 for a longer time.  The hope is the different etch chemistry will save us

Personally, I am more of a fan of 1.  My personal explaination of what is going on is the Oxford 100 is sputtering our Cr layer, which is causing us to redeposit a micromask.  So while I hope the Oxford 82 is a bit more gentle, I really think using a resist is a more sure way of doing things.  We are going to do the following (at a high level) today:

1. RCA clean a new SVM wafer, deposit 300 nm of oxide on the PECVD, and sputter 225 nm of Cr mask from the AJA1.
2. Pattern the Cr hard mask wafer using the same photolithography process as yesterday (and same GDS file).  I will also use a long piece of SVM wafer with 1 um of oxide on top and pattern it the same way
3. Descum both wafers for 50 seconds
4. For the Cr wafer, use wet etching for ~3.5 minutes to wet etch the mask, giving us the pattern we want
5. For the oxide wafer, we will immediately go to the Oxford 100.  I say we do a 10 min preclean, 1.5 min season, and 3 minute etch.  This should give us an idea of whether it is even possible to get no dust with our proposed process.  If there is no dust (and we are able to characterize the thickness of all the layers), we can proceed with a longer etch to get through the SiNx.
6. For the Cr wafer, we cleave it up.  We then go to the Oxford 82 and run a 20 minute oxifrd etch using the CF3H chemistry.  We can then characterize the etch rate after.  We will not etch each piece in case different chemistries work better or worse

Below are the two GDS files we are using (2 for the Cr wafer, 3 for the oxide wafer)

[pad4 pass2 (negative).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/21C2A93C-D660-41AC-AAF0-400AB54BAC45_2/UiKYGVmWZuOxfJui4xAug7ZMJkYAXKOew7DxPjVRV2sz/pad4%20pass2%20negative.gds)

[pad4 pass3 (negative).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9A39E0E7-727E-445D-AACE-05A133336BB2_2/NjtyFcksLyX2hCRGfsplivPsgFWa7TVCxihmwckbjYUz/pad4%20pass3%20negative.gds)

I am currently running RCA clean and 10 min pre clean of the Pecvd 

Below is the old wafer I want to use, though I will also check it with ellipsometer

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-001.jpeg)

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-002.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-003.jpeg)

Below is a note from the tech session:  People did not seem to believe Cr was the issue.  There was broad concensus that we should use the oxford 100.  It seems that the more basic CHF3/O2 recipe is best.  There seems to be concern that we are having polymerization issues.  We might want to run shorter etches.

### Pecvd

Before season

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-004.jpeg)

Before deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-005.jpeg)

During deposition

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-006.jpeg)

### Aja sputtering

Pressure when loading

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-007.jpeg)

Our process

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-008.jpeg)

During run

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-009.jpeg)

### Photolithography

Spin recipe

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-010.jpeg)

We also do 90 C for 1 min

First exposure

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-011.jpeg)

Use same dose of 53, 0

Second exposure has hard time automatic centering. The piece is a lot longer than wide. I am using the mask package to proceed

It is a bit confused about the size, but oh well. It should still expose where it does not think there is wafer

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-012.jpeg)

It seems to be writing over the full piece, which is good

Development of 1

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-014.jpeg)

Second develop foe 1 min

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-015.jpeg)

### Descum

I am doing the descums seperately

50 second descum after the 5 min pre clean

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-016.jpeg)

During descum

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-017.jpeg)

Resist thickness after descum is 400 nm

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-018.jpeg)

# Cr etch

We do 3.5 mins of wet etch.

### 82 etch

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-019.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-020.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-021.jpeg)

Inspection

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-023.jpeg)

Profilometer

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-024.jpeg)

### Etching

By the end of the development and descum, we should have 8 pieces that have oxide hard mask and 9 pieces with Cr hard mask.  I say, at the beginning, we put 3 of the Cr hard mask pieces into the Oxford 82 for like 20 minutes.  This will still leave us with plenty to play with.

For the 100, we should start by cleaning for 10 mins and seasoning for 5.  We should then do a 3 minute etch of an oxide hard mask chip.   Lets see if there is an issue there.  We then will keep iterating every 3 minutes.  I say we start with the CHF3 recipe.  We should also measure the resist thickness before starting.  We will then, if things work, do one longer etch.

We can do the same thing with the CH2F2 recipe.  Or we can use the CHF3 recipe on a Cr hard mask.  Either way, I say we take it slow.

# Oxford 100 for the first piece

![Drawing](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-025.jpg)

Just started the 10 min pre clean 

We are going to try the recipe below for 5 min season

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-027.jpeg)

19:37 Finished

## First etch CHF3 recipe

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-028.jpeg)

We use this piece

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-030.jpeg)

Mounted on the wafer

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-031.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-033.jpeg)

19:42 Starting.

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-034.jpeg)

Looks good. The plasma is on and bright.

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-035.jpeg)

He flow is also very low.

19:50 Venting

## Inspection

![2025-04-16-first-etch.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-036.jpeg)

Small amount of dusts observed under dark field microscope 

1.1 um deep

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-037.jpeg)

## Second etch CHF3 recipe

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-040.jpeg)

20:02 Starting.

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-041.jpeg)

20:08 Low He

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-042.jpeg)

20:11 Finished.

![2025-04-16-second-etch.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-043.jpeg)

The amount of dusts seemed to have decreased!

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-044.jpeg)

Etched 2.4 um.  If we etched 2.4 um in 6 mins, then the rate is 400 nm/min.  Lets etch for 5:15 mins.  We will leave a small amount of nitride left

## Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-045.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-046.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-047.jpeg)

## Wet etching

![2025-04-16-after-wet-etch.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-048.jpeg)

No visible increase in the amount of dusts



# Larger Piece Etch

5 min season

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-049.jpeg)

5:15 etch

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-050.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-051.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-052.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-053.jpeg)

## Inspections

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-054.jpeg)

![2025-04-16-main.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-055.jpeg)

Very few dusts!

### RTA

We are going to do 2 dies at 800 C and leave the other at room temp

Calibration run

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-056.jpeg)

During run

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-057.jpeg)

Final RTA

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-058.jpeg)

I am using a clean carrier as well

During 

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-059.jpeg)

Inspection after

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-060.jpeg)

It seems that the SiNx burst off. Below is filmetrics of the holes

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-061.jpeg)

Of the film

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-062.jpeg)

Microscope 

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-063.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-064.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-065.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-066.jpeg)

Everything else looks safe, with no cracks on waveguides

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-067.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-068.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-069.jpeg)

---

[`Thu, Apr 17`](day://2025.04.17) 

# Room temp chip

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-070.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-071.jpeg)

### First straight

4.7 mW / 49 mW = 4.7/49=0.0959 

### Second straight

5.1 mW / 49 mW = 5.1/49=0.104 

### Third straight

5.2 mW / 49 mW = 5.2/49=0.106 

### First snail

0.3 mW / 49 mW = 0.3/49=0.00612 

### Second snail

0.28 mW / 49 mW = 0.28/49=0.00571 

### Third snail

0.1 mW / 49 mW = 0.1/49=0.00204 

![Image.png](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-072.png)

# 800 C chip

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-073.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-074.jpeg)

### First straight

1.2 mW / 49 mW = 1.2/49=0.0245 

### Second straight

0.25 mW / 49 mW= 0.25/49=0.0051 

### Third straight

1 mW / 49 mW = 1/49=0.0204 

### Snails

We see only few microwatts from the first and second snails

# 800 C #2

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-075.jpeg)

We use the longer one.

### First straight

0.5 mW / 49 mW = 0.5/49=0.0102 

---

New cleaved wafers

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-076.jpeg)

After 800 c

### First straight

7 mW / 49 mW = 7/49=0.143 

### Second straight

7.3 mW / 49 mW = 7.3/49=0.149 

### Third straight

6.9 mW / 49 mW = 6.9/49=0.141 

### First snail

0.55 mW / 49 mW = 0.55/49=0.0112 

### Second snail

0.88 mW / 49 mW = 0.88/49=0.018 

### Third snail

0.7 mW / 49 mW = 0.7/49=0.0143 

### Die 2

### Snail 2

0.57 mW

### Snail 3

0.95 mW

### Longest snail 

0.24 mW

I would still like to test the other die (I was just dreadful at switching the microscope).  I think I have enough to work with now though for loss measurements





Compiled losses are below

![Image.png](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-077.png)

Below is a loss matrix

|       | Room Temp | 650 RTA | 800 RTA |
| ----- | --------- | ------- | ------- |
| CH2F2 | 3.148     | 1.963   | 1.525   |
| CHF3  | 3.546     | \-      | 2.475   |



Now I coat resist for oxide hard mask. I use 1813 for 4500, 8000, 45. I want thicker resist because our recipe will etch it fast

Before spin

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-078.jpeg)

115 C for one minute

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-079.jpeg)

For exposure

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-080.jpeg)

We used 70, -1 last time, so I will do that again

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-081.jpeg)

Writing is going well

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-082.jpeg)

Develop in 726 for 1 min

![Photo from Library.jpeg](../../assets/fab/2025-04-16-mask-design-to-eliminate-dust-083.jpeg)