---
type: craft-export
title: "2025-04-07 special oxide deposition and etching for reduced bending losses"
craft_document_id: CABA1948-4897-432B-840C-3E02E2383972
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-07 special oxide deposition and etching for reduced bending losses
While testing the previous waveguides, it seemed that we were seeing a lot of bending loss into the photoconductor due to bends in the previously fabricated negative devices.  While I have not run rigorous simulations of these bending losses, intuitively, more oxide is always better.  The way we do this (getting more oxide on the side) is either CMP or etching.  CMP is down right now, so we can’t use that.  But a way to do this is deposit extra oxide and then do a very directional etch after.  This is nice in the sense that it is very controlled (Even if it won’t solve the lower breakdown issues).  We are going to do this to the 4 layer device.

Currently, the device still has Cr hard mask on.  So we need to etch that off.  That requires 15 minute Cr etch and 15 second BOE dip.  We then want to move to the PECVD.  For TEOS, we know the dep rate is 55.5 nm/min.  This means, if we want 2 um of oxide, lets deposit for 35-ish minutes.  Obviosuly, the clean afterwards is going to take forever, but that is totally fine.  Please also add 12 minute pre-heat.   We also want to put in a witness sample.

Next, lets etch.  From previous experience (a while back) we found the etch rate of oxides on pieces (so attached with cool grease) to be 150 nm / min.  We will first season and etch the witness sample for 3 minutes.  We can use that rate to calibrate the etch of the main sample (though we guess an etch time of ~6.6 minutes.

If we overetch, we can always just deposit more high rate oxide.  So I am not super worried about that.

Below are the steps:

1. Preclean for 5 minutes and season for 2 minutes PECVD chamber (season with TEOS)
2. Run TEOS deposition for 35 minutes, expecting 1950 nm of oxide.  (Add witness sample too)
3. Clean PECVD chamber (do this is parallel with things below)
4. Clean Oxford 100 chamber for 10 minutes, and season for 1 minute
5. For the high rate etch (below is an image of the recipe) for 3 minutes on the witness sample.  Measure the etch rate on the witness sample
6. Etch such that you have roughly 1 um of oxide remaining on the top.  
7. Try to use ellipsometry to test that things turned out ok.  If they did not, use high rate PECVD to make sure you have enough top oxide

Below is the etching recipe we want to use.

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-001.jpeg)

We want to use the four layer device wafer box!!!

# Note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

14:47 Cr etch started. We did acetone bath beforehand.

[2025-04-07 Fabrication of etched waveguide with thick core](https://tdwg.craft.me/5C86K6Mt8nfxJx)

Beginning part of the process

15:15 Acetone bath

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-002.jpeg)

17:43 Logging into the tool

## Precleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-003.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-004.jpeg)

5 mins starting 17:45

## Seasoning

We use CNF CMOS TEOS

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-006.jpeg)

17:54 Seasoning

This time, I’m not setting the heating to 12 mins. We do it for the main run.

18:01 Finished

## Main run

35 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-007.jpeg)

12 mins heating

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-008.jpeg)

35 mins dep

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-009.jpeg)

18:04 Starting

![Drawing](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-010.jpg)

This will put extra 1.5 um of oxide

18:54 Finished

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-012.jpeg)

No oxide? We need to do this again.

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-014.jpeg)

No clear indication on how this went wrong 

## Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-016.jpeg)

We skip this process

## Retake the main run

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-018.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-020.jpeg)

12 mins heating, 35 mins main dep

19:22 Heating finished

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-022.jpeg)



We now start the pre clean for 13 mins on the Oxford 100

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-023.jpeg)

Reminder of recipe below

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-024.jpeg)

Oxide and nitride are the same

We seasoned for 1 minute

Yesterday was a complete failure, so we are restarting now

I am running a 5 min preclean on the PECVD.  

Jeremy recommends we use the smooth recipe, pictured below

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-025.jpeg)

I will run with witness sample to get dep rate

# Note on [`Tue, Apr 8`](day://2025.04.08)

16:06 cleaning 5 mins

## Seasoning

2 mins

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-027.jpeg)

16:08 Seasoning starting

16:16 Finished

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-028.jpeg)

330 nm per minute. This means we need 15 mins 10 s of deposition

![IMG_0592.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-029.png)

## Main run

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-031.jpeg)

We aim at 2.5 um

16:22 Starting.

16:42 Finished

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-033.jpeg)

2615 nm.



## Cleaning

30 mins





I am running a 5 min pre clean on the Oxford 100

I am going to run a 1.5 minute season of the Oxford 100 and put a witness sample in to verify the etch rate

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-034.jpeg)

We use the thinner

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-035.jpeg)

16:54 Seasoning finished

16:55 Venting

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-037.jpeg)

115 nm. This is 330 - 115 =215 nm etched. 215/1.5=143.333 nm/min

215/90=2.389 nm/sec. 1600/2.389=669.736 seconds. 11 mins 10 sec.

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-040.jpeg)

Plasma on

During etch

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-041.jpeg)

17:23 completes. Stop and vent

17:30 Cleaning. 15 mins.

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-043.jpeg)

Almost perfectly 1 um!



---

# Retaking data with the IR camera on [`Thu, Apr 10`](day://2025.04.10) 

# Measurement of loss with oxide deposited

Using the IR camera and 1570 nm light source, we measure the propagation loss of the snake and snail waveguides with oxide cladding but with no SRN on top. 

## Snake waveguide chip

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-044.jpeg)

### First snake

3 mW / 49 mW = 3/49=0.0612 

### Second snake

2.7 mW / 49 mW = 2.7/49=0.0551 

### Third snake

2.4 mW / 49 mW = 2.4/49=0.049 

### Fourth snake

2.4 mW / 49 mW = 2.4/49=0.049 

### Fifth snake

0.47 mW / 49 mW = 0.47/49=0.00959 

### Sixth snake

0.6 mW / 49 mW = 0.6/49=0.0122 

### Seventh snake

0.3 mW / 49 mW = 0.3/49=0.00612 

## Snail waveguide chip

### First straight

9.5 mW / 49 mW=9.5/49=0.194

### Second straight 

9.2 mW / 49 mW = 9.2/49=0.188 

**Third straight**

9.4 mW / 49 mW = 9.4/49=0.192 

### Fourth straight

9.4 mW / 49 mW = 9.4/49=0.192 

### First snail

1.5 mW / 49 mW = 1.5/49=0.0306 

### Second snail

1.7 mW / 49 mW = 1.7/49=0.0347 

### Third snail

0.35 mW / 49 mW = 0.35/49=0.00714 

### Fourth snail

0.35 mW / 49 mW = 0.35/49=0.00714 

Below are the loss measurements for thick oxide claddings 

![Image.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-045.png)

![Image.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-046.png)



---

### [`Fri, Apr 11`](day://2025.04.11) Measurement of loss after SRN deposition

We measure the loss of the waveguides after SRN is deposited.

## Snail waveguide

It was difficult to couple selectively into the straight waveguide. There is a good chance that the power numbers include the contributions from the photoconductor modes.

### First straight 

5.4 mW / 49 mW = 5.4/49=0.11 

### Second straight

6.3 mW / 49 mW = 6.3/49=0.129 

### First snail

0.057 mW / 49 mW = 0.057/49=0.00116 

### Second snail

0.16 mW / 49 mW = 0.16/49=0.00327 

### Third snail

0.23 mW / 49 mW = 0.23/49=0.00469 

### Fourth snail

0.21 mW / 49 mW= 0.21/49=0.00429 

## Snake waveguide

Quite challenging to selectively couple light into the straight ones because we end up optimizing for the photoconductor mode. We saw about 1 mW in that case.

### First snake

2.7 mW / 49 mW = 2.7/49=0.0551 

![Photo from Library.jpeg](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-047.jpeg)

Somewhat very good coupling and also the mode is solitary.

### Second snake

2.3mW / 49 mW = 2.3/49=0.0469 

### Third snake

2 mW/49 mW=2/49=0.0408 

### Fourth snake 

2.1 mW / 49 mW = 2.1/49=0.0429 

[Recording 2025-04-11 131317.mp4](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/E78A0187-C44D-4B25-BE58-35BA35850230_2/Rl5LKRWPCNc2jgfzi7nmyAB66EiEtKFf2RA5YwMu8PIz/Recording%202025-04-11%20131317.mp4)

We move the beam up and down. Moving the beam up couples the light into the weaker mode with tails of light. This seems to suggest that the brightest mode is indeed the main mode.

### Fifth snake

0.33 mW / 49 mW = 0.33/49=0.00673 

### Sixth snake

0.4 mW / 49 mW = 0.4/49=0.00816 



![Image.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-048.png)

![Image.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-049.png)

From snake data, it would seem we have very similar loss to before.  It is slightly higher than we would like as baseline, but that is.  So thick side oxide seems like the trick

## Air cladded snail device

### First straight

8.1 mW / 49 mW = 8.1/49=0.165 

### Second straight 

7.6 mW / 49 mW= 7.6/49=0.155 

### Third straight

7.9 mW / 49 mW = 7.9/49=0.161 

### First snail

1.2 mW / 49 mW = 1.2/49=0.0245 

### Second snail

1.4 mW / 49 mW =1.4/49=0.0286 

### Third snail

0.32 mW / 49 mW = 0.32/49=0.00653 

![Image.png](../../assets/fab/2025-04-07-special-oxide-deposition-and-etching-for-reduced-bending-losses-050.png)

Interesting that we observe again that the longer difference, the lower our loss guess.  Either way, I am generally confident side oxide worked.  Below is the full document for all these loss calculations

[2025-04-10 Cutback Loss Measurement.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/974F8941-317A-46F1-A774-A7A4CE80313C_2/ujagf62CPvhzLAefSxcyEyozyO8rYEzzyRU2Tv0xZecz/2025-04-10%20Cutback%20Loss%20Measurement.pdf)