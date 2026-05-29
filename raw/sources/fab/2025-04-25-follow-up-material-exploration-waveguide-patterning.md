---
type: craft-export
title: "2025-04-25 follow up material exploration waveguide patterning"
craft_document_id: 66BB881D-386C-478B-B552-1647DB0FD75E
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-25 follow up material exploration waveguide patterning
We previously fabricated waaveguides with the PECVD and Takachi to test differnet SiNx deposition recipes.  We will use previous GDS files to explose three rows of 3 dies so we can test material loss on these waveguides.  We will then save two of the three rows to test RTA on different chips.  Right now, we have the following:

1. SRN3.5 on 1.75 um of oxide.  840 nm of waveguide and 450 nm of top pad oxide
2. SRN2.7 on 1.75 of oxide.  830 nm of waveguide and 450 nm of top pad oxide
3. Baseline Takachi on 1um of oxide.  1190 nm of waveguide and 450 nm of top pad oxide

First, we will use our normal Cr hard mask recipe of 1210 seconds of Cr sputtering at 7 mTorr.  We will then do lithography and etching after.  Before putting the Cr hard mask on, I will spin clean the wafers

### Aja sputter

Main recipe

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-001.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-002.jpeg)

Pressure when loading 3.5

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-003.jpeg)

During 3.5 dep

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-004.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-005.jpeg)

Pressure when loading 2.7

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-006.jpeg)

During 2.7 dep

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-008.jpeg)

Pressure when loading takachi

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-009.jpeg)

During takachi dep

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-011.jpeg)

### Photolith recipe

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-012.jpeg)

Then 90 C for 1 min

For MLA

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-013.jpeg)

Before 3.5 exposure

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-014.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-015.jpeg)

I am going to start a system where I process these wafers in parallel. 

Before 2.7 exposure

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-016.jpeg)

Before development of 3.5

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-017.jpeg)

Before takachi exposure

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-018.jpeg)

Before 2.7 development

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-019.jpeg)

Before takachi development

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-020.jpeg)

### Descum and Cr wet etch

I am running 7 min pre clean on 82

We use 50 seconds for all

Before 3.5 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-021.jpeg)

I only needed 2.5 mins to wet etch, mostly because this was a fresh batch of Cr etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-022.jpeg)

We can use the clamp regions as baseline for filmetrics

Before 2.7 descum

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-023.jpeg)

Side of 3.5

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-024.jpeg)

Middle

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-025.jpeg)

They are a bit differently

Let’s check ellipsometer

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-026.jpeg)

Fitting pretty much works. I will put in Cr etch for another 15 seconds to make sure 

2.7 took 2 mins to etch the Cr. 

Before takachi descum

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-027.jpeg)

Ellipsometery of 2.7

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-028.jpeg)

Fits good, I say we are good there

Takachi took a bit over 2 mins to finish

Observation after etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-031.jpeg)

Ellipsometer 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-032.jpeg)

It’s extremely close, so I think we are fine

I say we run takachi wafer for 5.5 mins

### Oxford 100 etch

Season for 5 mins, was already cleaned

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-033.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-034.jpeg)

3.5 before etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-036.jpeg)

2.7 before etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-037.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-038.jpeg)

I will dip and wash 2.7 for an extra 15 seconds before etching it.  We should probably etch 5 minutes on the SRN 2.7 and SRN 3.5 recipes

Before 3.5 etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-040.jpeg)

During 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-041.jpeg)

After etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-042.jpeg)

Perfectly depth, we will do it again

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-043.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-044.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-045.jpeg)

Minimal dust

Before 2.7 etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-046.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-047.jpeg)

After etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-048.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-049.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-050.jpeg)

Looks clean and good

Before takachi etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-051.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-052.jpeg)

After takachi etch

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-053.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-054.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-055.jpeg)

We run 25 min post clean. This will now go in acid bath

### PECVD cap

I am doing a 1 min of smooth season

3.5 after Cr strip

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-056.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-057.jpeg)

Before 3.5 cap

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-058.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-059.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-060.jpeg)

2.7 after Cr strip

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-061.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-062.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-063.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-064.jpeg)

Corners are a bit more dirty

3.5 after cap oxide

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-065.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-066.jpeg)

Before 2.7 season

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-067.jpeg)

Before 2.7 deposition

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-068.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-069.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-070.jpeg)

Takachi after Cr strip

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-071.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-072.jpeg)

Before season 3

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-073.jpeg)

Before takachi dep

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-074.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-075.jpeg)

## Loss measurement 

All measurements taken at 1570 with dichroic mirror and no EDFA

### SRN 2.7

Straight one

41.5 uW with 9.5 mW in

Straight two

40 uW with 9.6 mW in

Straight three

44 uW with 9.5 mW in

Snail 1

Could not find it or any other snails

I double checked these numbers at the end. They are repeatable

### SRN 3.5

Straight one

1.3 mW with 9.2 mW in

Straight two

1.25 mW with 9.2 mW in

Straight three

1.2 mW with 9.2 mW in

Snail one

150 uW with 9.2 mW in

Snail two

180 uW with 9.2 mW in

Snail three

130 uW with 9.2 mW in

Snail four

I think I ran out of room, so I could not find it

![Image.png](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-076.png)

### Takachi

Straight one

161 uW with 8.8 mW in

Straight two

170 uW with 8.8 mW in

Straight three

170 uW with 8.8 mW in

Snail one

21 uW with 8.8 mW in

Snail two

24 uW with 9.3 mW in

Snail three

1 uW, it was really tough

The reason the above was so low is I used the 10X objective, not the aspheric below are two waveguides I already did with aspheric

Straight three redo

1.128 mW

Snail one redo

150 uW

![Image.png](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-077.png)

![Image.png](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-078.png)

It seems that SRN2.7 is a bust.  Takachi and SRN3.5 are good.  Lets do 800 C RTA next with the two pieces of the bottom die remaining.

## First RTA 

We are going to do the two dies at 800 C for 5 mins. Doing all recipes at the same time

Calibration

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-079.jpeg)

I am now going to spin clean our chips

Before

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-080.jpeg)

SRN 3.5 on top, SRN 2.7, takachi at bottom

During

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-081.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-082.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-083.jpeg)

## Loss #2

### SRN 3.5

Straight first 

1.8 mW for 9.6 mW in

Straight second

1.63 mW for 9.6 mW in

Straight third

2 mW for 9.6 mW in

Snail one

582 uW for 9.6 MW in

Snail two

680 uW for 9.6 mW in

Snail three

741 uW for 9.6 mW in

![Image.png](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-084.png)

### Takachi

Seems that the straight ones are dead, only 40 uW on several waveguides

### SRN 2.7

Straight one

177 uW for 9.5 mW in

Straight two

150 uW for 9.5 mW in

Straight three

190 uW for 9.6 mW in

Straight four

228 uW for 9.5 mW in

Snail one 

Could not find it

I would still say the loss here is quite high 

## Second RTA

Given the results above, it seems that Takachi was broken by 800 C RTA.  This could be because of the high ramp or the tempurature.  Either way, I don’t think we suffer my lowering ramp to 5 C/s, so lets do that in general.  I say we try Takachi at 600 C.  Given that SRN 3.5 survived at 800 C and had a decent loss reduction, we should continue to try to push that loss number down.  The best way to do this right now is to continue increasing the RTA annealding tempurature.  I say we try to do 925 C.  I don’t want to push the tempurature too high, as we might start to break stuff.  

Below is the calibration of Takachi (we will use lower ramp during real run)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-085.jpeg)

After spin cleaning, below is the takachi run

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-086.jpeg)

I have been checking on the N2 as well lol

Unload at 350.

Calibration of 925

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-087.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-088.jpeg)

Starting off a bit warm. Took a minute to get to right temp

Later on

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-089.jpeg)

Unload at 450

## Loss #3

This was done on second setup with santec at 1570

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-090.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-091.jpeg)

Power before front objective is 10 mW. Generally the coupling efficiency is lower, but all we care about is the relative number

### SRN 3.5 925 C

Straight one

53 uW

Straight two

38 uW 

Straight three

38 uW

Straight four

38 uW

Straight five

54 uW

Given some of my results below, I think 54 is more reliable 

Snail one

16.3 uW

Snail two

16 uW

Snail three

15.2 uW

Snail four

6.9 uW

### Takachi 600 C

Straight one

14.5 uW

Straight two

15.3 uW

Straight three

14 uW

Straight four

15 uW

Snail one

While I can see it on camera, it’s a bit too dim for power meter. So the loss is still quite high

![Image.png](../../assets/fab/2025-04-25-follow-up-material-exploration-waveguide-patterning-092.png)

The general high level idea is we did not see some large decrease in loss.  While there is a bit of error in this measurement, we should have noticed if the loss was half as large.  So same order as before. It is possible loss went up be a slight amount