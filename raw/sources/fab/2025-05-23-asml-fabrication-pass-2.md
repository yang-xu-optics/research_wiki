---
type: craft-export
title: "2025-05-23 asml fabrication pass 2"
craft_document_id: 4CB064B0-38AE-44EF-A3E8-434F531BEEAD
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-05-23 asml fabrication pass 2
In our first ASML fabrication run, we seem to have broke our waveguides.  There are two likely explainations:

1. We did not remove ARC when removing edge bead, which means that we contaminated the wafer during the BOE dip
2. We annealed with Takachi oxide, which can’t handle higher tempuratures

Today, we will try to rectify these issues.  I will make new wafers, and be more systematic about testing loss as we go.  We will follow the same proceedure as before, which is:

1. RCA clean
2. 500 nm of pad oxide with 3 mins smooth deposition
3. Cr sputtering for 1210 seconds at 7 mTorr
4. ASML with existing recipe, dose 15 mJ/cm2, arc and 600 nm of DUV resist.  Develop and coat using gamma.  Make sure to use edge removal
5. Descum for 1:45.  
6. Cr hard mask etch for 3.5 mins
7. Oxford 100 CHF3/O2/N2 etch for 7 mins with 5 min season
8. 20 min Cr mask removal and 15 seconds BOE dip
9. 9+8 min smooth oxide deposition (in seperate steps)
10. 12.5 oxide thinning using CHF3/O2 recipe.

Below is Oscar’s recommendation for ARC removal

![Image.png](../../assets/fab/2025-05-23-asml-fabrication-pass-2-001.png)

We can even use 2 mins.  

### Mask prep

Just finished RCA clean

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-002.jpeg)

Before season (Jeremy cleaned when he was fixing tool)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-003.jpeg)

During season (we changed to smooth deposition becayse we hope this will slightly reduce roughness

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-004.jpeg)

Before deposition 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-005.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-006.jpeg)

Before second deposition

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-007.jpeg)

During second deposition 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-008.jpeg)

During sputter 1

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-009.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-010.jpeg)

During sputter two

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-012.jpeg)

# Resist coating

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-013.jpeg)

Dummy in slot 1

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-014.jpeg)

We do ARC first

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-016.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-017.jpeg)

Noting N2 is on

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-018.jpeg)

ARC coating started

Now PR coating 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-019.jpeg)

Start sequence now

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-020.jpeg)

Finished.

Turning off the N2



### ASML

Read the mask

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-021.jpeg)

First, we run edge clear

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-023.jpeg)

During first run

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-025.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-026.jpeg)

During main

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-027.jpeg)

# Development 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-028.jpeg)

Turning N2 on

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-031.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-032.jpeg)

After development, no edge bead

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-033.jpeg)

### Etching

82 pre clean

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-034.jpeg)

100 pre clean

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-035.jpeg)

We will descum for 2 mins just to be safe

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-036.jpeg)

Before 100 season

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-037.jpeg)

Inspection after descum

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-039.jpeg)

After Cr etch



![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-040.jpeg)

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-041.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-042.jpeg)

Depth after etch

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-043.jpeg)

After Cr strip, I do some Ellipsometer

In trench

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-044.jpeg)

With mask

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-045.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-046.jpeg)

# PECVD

## Seasoning 1 min

Seasoning smooth oxide recipe

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-047.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-048.jpeg)

Last user cleaned it well.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-049.jpeg)

19:50 Starting.

19:59 Finished

## Main run 9 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-050.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-051.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-052.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-053.jpeg)

20:02 Loading the wafer.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-054.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-055.jpeg)

We got 1.5 um, to be expected

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-056.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-057.jpeg)

## Cleaning 10 mins

Clean done

## Seasoning 2 1 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-058.jpeg)

## Main run 2 8 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-059.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-060.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-061.jpeg)

### Oxford 100 thinning

We expect 3.4 um of oxide at the end.  So we want to etch down 2.4 um.  This means etching for 14 mins.  For square spiral, we etched for 14 mins, and started with 3.2 (we used a different pad oxide).  Lets see the final, but plan for 14.  

Before season (I already left chamber clean).  I season for 2 mins.  

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-062.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-063.jpeg)

We will do 13.5 to be extra cautious 

Before

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-064.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-065.jpeg)

Almost spot on thickness

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-066.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-067.jpeg)

### Loss test room temp

I used 10 x objective with EDFA. 1570 is the wavelength 

Straight one

3.2 mW for 84 mW in

Straight two

3 mW

Middle square spiral 

120 uW

Middle circle spiral

230 uW 

Looks decent enough. We will try RTA now

### RTA test

I spin cleaned the test wafer

Calibration

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-068.jpeg)

During main run

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-069.jpeg)

Small explosion 

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-070.jpeg)

### Loss on RTA

Using 10 X objective, Edfa, and 1570

Straight 1

5.3 mW for 94 mW in

Straight 2

5.9 mW

Square medium 

1.6 mW

Circular medium

1.7 mW

Fast adibatic 

6.2 mW

Fast hump

3 mW

Fast hump 2

3.6 mW

So it does seem that having the structures does increase loss, which is a bit unfortunate.

### Main RTA

I cleaved and spin cleaved new pieces

Below is calibration of RTA

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-071.jpeg)

Main run

Before

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-072.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-073.jpeg)

# PECVD for SRN deposition

We start with some pre cleaning, just 5 mins.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-074.jpeg)

Previous user.

16:36 Venting

## Pre cleaning: 5 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-075.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-076.jpeg)

16:37 Starting.

16:47 Finished.

## Seasoning 1: 2 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-077.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-078.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-079.jpeg)

16:49 Starting

16:55 Finished

The color of the sample looks good.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-080.jpeg)

## Main run 1: 32 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-081.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-082.jpeg)

17:00 Starting

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-083.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-084.jpeg)

17:36 Finished

The colors of the samples look good.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-085.jpeg)

## Cleaning 1: 20 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-086.jpeg)

17:39 Starting

18:02 Finished

## Seasoning 2: 2 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-087.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-088.jpeg)

18:05 Starting

18:11 Finished

The color of the sample looks okay.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-089.jpeg)

## Main run 2: 32 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-090.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-091.jpeg)

18:15 Starting.

18:52 Venting.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-092.jpeg)

## Cleaning 2: 20 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-093.jpeg)

18:54 Cleaning started

19:18 Finished.

## Seasoning 3: 2 mins

We load a witness sample,

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-094.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-095.jpeg)

19:20 Started.

19:27 Finished. The color looks good.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-096.jpeg)

## Main run 3: 32 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-097.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-098.jpeg)

19:30 Starting.

20:06 Finished.

20:07 Venting.

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-099.jpeg)

## Cleaning 3: 20 mins

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-100.jpeg)

20:10 starting.

# ITO deposition

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-101.jpeg)

20:39 starting

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-102.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-103.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-104.jpeg)

Try to make waveguides 1.7 long

### Loss sanity check at end

Medium square

1.76 mW (so same as baseline)

