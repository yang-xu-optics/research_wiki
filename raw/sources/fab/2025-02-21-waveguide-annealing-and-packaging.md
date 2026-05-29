---
type: craft-export
title: "2025-02-21 waveguide annealing and packaging"
craft_document_id: 48A6CA69-EF26-4C0B-9438-0F900ABA2B26
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-02-21 waveguide annealing and packaging
Before Cr mask removal

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-001.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-002.jpeg)

I am now going to do a 20 minute Cr etch.  I will then do a 15 second BOE etch after.  I will check under dark-field microscope and filmetrics to make sure Cr is gone.  Last time, our anneal was using O2/N2 Anneal recipe

Last time, the editted recipe looked like

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-003.jpeg)

So we load and unload at 300 C.  We manually input the setpoint.  We ramped up for 160 mins and annealed for 180 mins.  I will increase anneal time to 200 mins.  We anneal at 1100 C.  Lets load and unload at 4 ipm.  

I edited the recipe accordingly

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-004.jpeg)

After first Cr etch, there were still some areas without total Cr removal. Will do another 15 mins

Second Cr etch did the job

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-006.jpeg)

Surface oxide has a bit of discoloration, but not too bad. 

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-007.jpeg)

I think we are ready to anneal

I am also doing a quick tumble dry and wash of the wafer 

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-008.jpeg)

Before anneal

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-009.jpeg)

Loading at 4ipm

Further during load

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-010.jpeg)

The tube is ramping

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-011.jpeg)

During anneal

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-013.jpeg)

The system is now ready for overnight cool off

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-014.jpeg)

Before unloading 

We unload at 4 ipm

During unload

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-015.jpeg)

So the edges do look as expected

Once out

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-016.jpeg)

Under microscope

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-018.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-020.jpeg)

Dark field

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-024.jpeg)

More bright

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-025.jpeg)

More bent waveguides survived in bottom right

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-028.jpeg)

It seems like the middle of the wafer has the most issues. Either way, let’s continue

Now lets Cr etch the other device and do some RTA

I am pre cleaning the PECVD with big wafer 

We willa slo RTA at 650 for 3 mins for the smaller piece

Smaller piece after Cr etch

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-031.jpeg)

No evidence of Cr flakes

Because the RTA is down, we will deal with TEOS later

Given this result, it seems clear that we either need a lot more trenching, or to use a negative tone pattern.  Negative tone either means using a negative resist or doing a flood exposure with a positive resist.  I am a bit biased towards using positive resist still, just because we know how that works.  We are going to get some serious feature distortion though.  We also know from the recent waveguide tests that we hvae a more limited field of view in the imaging setup than we previously believed.  So we need to account for that too.  In the next round, I say we get more ambitious than our current chips, and go all the way for 10 cm.  I also say that we should add a few ring structures just to see what happens.  I think we generally have too many straight structures at the moment, and we probably made the last useful straight structure in this anneal.

Before RTA

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-032.jpeg)

During calibration

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-033.jpeg)

During run

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-034.jpeg)

I am gonig to do a 1 minute season with TEOS

There was a comment on the PECVD recently that the TEOS dep rate was elevated (to 78 nm/min).  We really only need an extra 800 nm, so I say we do 12 mins and see what we get.  Before we thought it was 50 nm/min, so this would still give us like 600 nm.  We can always do a small cap with high rate.  I am putting witness sample in to be sure.  We also require 12 min preheat

Before dep

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-036.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-037.jpeg)

Witness sample thickness

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-038.jpeg)

Microscope after dep

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-040.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-042.jpeg)

Our dep rate with TEOS is about 56 nm/min.  We really would probably like a couple hundred nm more just to make sure of breakdown and no leakage of modes.  I way we deposit another 150 nm.  If we have a dep rate of 230 nm/min, this means we want to dep for an additional 38 seconds.  

Before second oxide

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-043.jpeg)

During second oxide

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-044.jpeg)

Another Ellipsometery of witness sample

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-045.jpeg)

Seems like what we want!!

Before first SRN season

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-046.jpeg)

We will now do 23.5 min depositions.  The right side of the LN box has the chips we want to use.  everything (including witness sample) was spin cleaned

Before dep 1

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-047.jpeg)

During dep 1

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-048.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-049.jpeg)

I think doing the fully 24 mins of cleaning is insane.  20 is definatley fine considering our dep rate is not super high anyway.

Ellipsometery of the first sample

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-050.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-051.jpeg)

---

# [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) continuing the process [`Fri, Feb 28`](day://2025.02.28)

[`Ben Ash`](craftdocs://users?id=d9d2fbda-3d0b-154c-637c-be9f41830cae) did a first round of deposition. There is 1.5 um of SiN already.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-052.jpeg)

Cleaved the witness samples. The main witness sample has 1.5 um of SRN.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-053.jpeg)

## Seasoning 2nd round

12:51 Venting

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-054.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-055.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-056.jpeg)

12:53 Starting

13:02 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-057.jpeg)

The color of the witness sample looks good and uniform. We’ll continue.

## Main 2nd round

13:06 start. 23.5 mins.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-058.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-059.jpeg)

Same recipe for the same duration.

13:35 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-060.jpeg)

Now doing characterizations

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-061.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-062.jpeg)

Quick characterizations with filmetrics. The thickness looks good.

## Cleaning 2nd round

We do 20 mins of cleaning.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-063.jpeg)

13:39 Started.

14:02 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-064.jpeg)

## Seasoning 3rd round

3 mins seasoning.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-065.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-066.jpeg)

14:05 Seasoning started.

14:12 Finished.

14:13 Venting.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-067.jpeg)

## Main run 3rd round

We do 23.5 mins of deposition.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-068.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-069.jpeg)

14:17 loading

14:17 Started.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-070.jpeg)

Remaining pieces in the box.

14:44 finished.

14:46 venting

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-071.jpeg)

## Cleaning 3rd round

20 mins cleaning.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-072.jpeg)

14:50 Started.

15:11 Done.

## Seasoning 4th round

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-073.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-074.jpeg)

15:17 Seasoning started. 3 mins.

15:25 Done.

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-075.jpeg)

## Main run 4th round

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-076.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-077.jpeg)

15:29 Starting

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-078.jpeg)

Top left two are from this round

---

# [`Ben Ash`](craftdocs://users?id=d9d2fbda-3d0b-154c-637c-be9f41830cae)  continuing the process [`Fri, Feb 28`](day://2025.02.28)

## Cleaning 4th round

![Drawing](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-079.jpg)

After taping

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-080.jpeg)

## ITO deposition

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-081.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-082.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-02-21-waveguide-annealing-and-packaging-083.jpeg)

Skipped at 300 A.