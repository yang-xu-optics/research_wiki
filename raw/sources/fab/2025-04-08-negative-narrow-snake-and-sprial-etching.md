---
type: craft-export
title: "2025-04-08 negative narrow snake and sprial etching"
craft_document_id: 3FDDE500-85E2-4EA7-A013-774B7FE0B9E1
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-08 negative narrow snake and sprial etching
We previously fabricated negative spiral and snake waveguides, but they were too wide.  This leads to loss to other modes from the fundamental, meaning these are not super useful.  So we designed a new GDS (attached below) that has much more and narrower spirals and snakes.  They are not quite as long (the max lenght is ~7 cm) but that is ok

[pad4 pass1.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7A6A0695-9B23-46E5-8D67-B0D2B0AAED2B_2/8N3L95EOFCbZkfoKuRx2Z93fnely0z0xuRKOxnXOVdwz/pad4%20pass1.gds)

All rotated as well

![Image.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-001.png)

We are also not going to use a Cr hard mask for this.  We will just spin clean, spin prime, and coat the wafer with 1813.  We are following a recipe Gui gave us, which is attached below

![Image.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-002.png)

He claims this should give us a micron, but I am going to quickly check on a dummy piece.  The procedure is going to go as below

1. Spin clean, vapor prime, and spin coat 1813.  Use 5000 rpm, with 8000 ramp, and 45 second spin.  Bake at 1 min at 115 C
2. Expose on the MLA with 70 mJ dose and defocus of -1.
3. Develop the resist with MIF 726 for 1 minute in the hamatech
4. Descum the resist for 1 minute in the oxford 81 or 82
5. Etch the SiNx in the Oxford 100 for 9.5 mins (as we clocked the etch rate on these samples previously to have been 210 nm/min).  In the book, it says we should get 4:1 selectivity
6. Remove remaining resist with O2 plasma, resist strip, RCA.  This we will come to later

Now I will coat an Si piece using Gui’s recipe just to verifiy it works as he is telling us

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-003.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-004.jpeg)

115 C, 1 min baking.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-005.jpeg)

It is a bit thinner than we want. We make the spin speed slower.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-006.jpeg)

Coating done

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-008.jpeg)

# Development 

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-009.jpeg)

Program 6

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-011.jpeg)

# Oxford 82 for descum

21:37 Logging in

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-013.jpeg)

21:38 10 min oxygen cleaning

21:57 Venting

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-014.jpeg)

1.1 um left. We can do 90 sec of descum

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-016.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-017.jpeg)

22:04 Start

Descum eats photolresist by 90 nm per minute

22:09 Venting



# Oxford 100

Below is before season

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-018.jpeg)

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-019.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-020.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-021.jpeg)

Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-022.jpeg)

15 mins

We have the Si wafer inside

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-023.jpeg)

We have height of 2.5 um



# Oxford 82 again

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-025.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-026.jpeg)

22:47 Mild descum 10 mins

Finished

We saw roughly 2 um of height after the profilometer, roughly confirming the 4:1 selectivity (as the descum removed ~ 500 nm of resist).  I will also put the wafer in the resist strip bath just to make sure.





# Note added on [`Thu, Apr 10`](day://2025.04.10)

# PECVD for SRN

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-027.jpeg)

16:42 Cleanimg 5 mins



![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-028.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-029.jpeg)

17:02 Done

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-030.jpeg)



23 mins for 1.5

23/1.5*2=30.667 

31 mins

### Main run

31 minutes

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-031.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-032.jpeg)

17:06 Started.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-033.jpeg)

17:41 Done now.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-034.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-035.jpeg)

Thickness came out mostly as expected

### Cleaning



---

# Note added on [`Fri, Apr 11`](day://2025.04.11)

We intend to perform PECVD deposition of smooth SiO2. See [2025-04-07 Special oxide deposition and etching for reduced bending losses](craftdocs://open?blockId=CC67967E-0650-4044-8C24-17BF920C8645&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8).

Last time, we got 2.5 um of SiO2 after 15 mins 10 secs of SiO2 smooth recipe. Dep rate is 2.75 nm/s.

![IMG_0596.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-036.png)

We aim at 1.5 um

![IMG_0597.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-037.png)

546 secs=9 mins 6 secs for 1.5 um. We do this twice.



# PECVD

## Cleaning 5 mins

15:39 running

15:45 Finished.

## Seasoning 2 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-040.jpeg)

15:46 Starting. We expect to see 330 nm after this.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-041.jpeg)



### Main run 9 mins 6 secs

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-043.jpeg)

16:14 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-044.jpeg)

### Cleaning 12 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-045.jpeg)

16:17 Starting

16:34 Done

### Seasoning 2 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-046.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-047.jpeg)

16:43 Done

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-048.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-049.jpeg)

Thickness good. May be a bit thinner.

### Main run 2 

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-050.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-051.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-052.jpeg)

Second run. 9 mins 6 secs.

16:45 Ｓｔａｒｔｉｎｇ．

16:59 Completed.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-053.jpeg)

### Cleaning

24 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-054.jpeg)

Started

# Oxford 100 etcher

- Clean 10 minutes
- Season for 1.5 minutes
- We aim at 1.9 um etching
- Last time, we got 143.3 nm/minute or 2.389 nm/sec. If we want to do 1900 nm, we should do 1900/2.389 = 795 secs=13 mins 15 seconds. 

![Image.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-055.png)

- To keep some safety margin, we can do 12 mins 45 secs.

## Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-056.jpeg)

I see a wafer inside already.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-057.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-058.jpeg)

10 mins Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-059.jpeg)

Because there’s already a wafer, we do the process on this one.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-060.jpeg)

16:56 Started.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-061.jpeg)

Plasma is on.

17:09 Wafer came back



### Seasoning

We use this one. 1.5 mins seasoning.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-062.jpeg)

This is the same recipe as before

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-063.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-064.jpeg)

Wafer is loaded.

17:11 Started.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-065.jpeg)

Flow is okay

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-066.jpeg)

Plasma on.

17:16 Finished. Venting.



### Main run

12 mins 45 sec.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-067.jpeg)

17:21 Loading the wafer.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-068.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-069.jpeg)

17:22 Started.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-070.jpeg)

He flow seems okay

17:40Venting

### Cleaning

15 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-071.jpeg)

Loading wafer

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-072.jpeg)

17:45 Starting

## Ellipsometry

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-073.jpeg)

The fit is pretty good. We might have left a bit too much SiN though. The oxide thickness is around 1.3 um. Again, we could have made this a bit thinner.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-074.jpeg)

The fit does not change even after we enforce the pre-determined values of SiN index.

Now I am precleaning the PECVD for SRN deposition for 5 mins.  I also spin cleaned everything after cleaving

Before season

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-075.jpeg)

Lets do 3 deps of 32 minutes to get our 6 um of SRN.  I realized after the fact that the recipe I input was slightly off.  To be clear, below is the full recipe we want

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-076.jpeg)

Before first deposition

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-077.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-078.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-079.jpeg)

First witness sample

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-080.jpeg)

Looks good to me

24 mins of cleaning worked. 

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-081.jpeg)

Before second deposition

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-082.jpeg)

During second deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-083.jpeg)

21 mins of cleaning worked

Before season 3

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-084.jpeg)

Before dep 3

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-085.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-086.jpeg)

During dep 3

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-087.jpeg)

# ITO

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-088.jpeg)

At end of sputter

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-089.jpeg)

---

[`Sat, Apr 12`](day://2025.04.12)

# Measurement of loss

## Oxide cladding device with no SRN

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-090.jpeg)

This waveguide has very low transmission. We measured only 4 uW at 1570 nm, out of 49 mW coupling.

## SRN device

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-091.jpeg)

We got a bit more transmission, e.g., 400 uW from the straight waveguide.

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-092.jpeg)

However, the mode is very messy. Also, the coupling is much less critical. This seems to indicate that the most of the power come from the photoconductor coupling, unfortunately.

Below is image of mla job

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-093.jpeg)

New one

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-094.jpeg)