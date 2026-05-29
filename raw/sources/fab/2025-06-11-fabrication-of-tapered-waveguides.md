---
type: craft-export
title: "2025-06-11 fabrication of tapered waveguides"
craft_document_id: B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-11 fabrication of tapered waveguides
While we have shown super linear scaling over large distances, we seem to be struggling with sub-optimal scaling (closer to linear instead of quadratic) for the ending regions of our waveguides.  This makes Ryo and I suspect that there is some multi-modeness issue causing the SHG signal to couple to higher order spatial modes at bends.  Because different modes don’t interfere, we will get suboptimal scaling.  Below is the newly designed GDS file that I want to use

[Pad6_Pass4_negative_final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/BDF390B4-A58D-4D05-9BA3-0E59A122C7F5_2/AZN0HE6yWicokidN0SBzkPvoflEH13xww0B0SrqHj8Ez/Pad6_Pass4_negative_final.gds)

In this file, we taper things from 6 → 2 or 6 → 3 um wide bends, with differnet poling distances

# Preparing wafers

We received a new batch of wafers from SVM. They have 2 um PECVD SiN on 1 um of thermal oxide. The substrate is conductive Si.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-001.jpeg)

15:15 RCA cleaning them.

We process 4 of these wafers,

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-002.jpeg)

# Pecvd

Before season

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-003.jpeg)

## Main run 1 for 500 nm

We do 3 mins of smooth oxide deposition.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-004.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-005.jpeg)

This should give us roughly 500 nm of SiO2.

16:02 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-006.jpeg)

16:05 Finished.

## Main run 2 for 500 nm

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-008.jpeg)

16:14 Finished.

Venting.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-009.jpeg)

## Cleaning 10 mins

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-010.jpeg)



## Seasoning 

We do 2 mins of seasoning.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-011.jpeg)

Made a mistake of running this without setting the time. We jump through.



![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-012.jpeg)

## Main run 3 for 1.5 um of oxide

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-014.jpeg)

9 mins smooth oxide.

Starting now.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-015.jpeg)

17:01 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-016.jpeg)

Finishes.

## Cleaning

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-017.jpeg)

17:03 Starting.

## Seasoning　

[`Ben Ash`](craftdocs://users?id=d9d2fbda-3d0b-154c-637c-be9f41830cae) run the seasoning

## Main run 4 for 1.5 um oxide

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-018.jpeg)

We use this wafer. The other processed wafer has been moved to the ASML step [2025-05-23 Oxide Hard Mask Testing](craftdocs://open?blockId=122F1589-6CC0-4921-B10C-DEEA9900CD36&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-020.jpeg)

9 mins smooth oxide

17:41 Finished.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-022.jpeg)

## Cleaning

We do 20 mins cleaning.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-023.jpeg)



### AJA

Sputter recipe

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-024.jpeg)

Pressure at load

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-025.jpeg)

During first wafer

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-027.jpeg)

Pressure at load for 2

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-028.jpeg)

During second wafer

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-030.jpeg)

### Lithography

Our recipe

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-031.jpeg)

We use 1805

During 90 bake for 1 min

New nominal focus. Still use 53 as dose

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-032.jpeg)

Development

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-033.jpeg)

We use recipe 4



# Oxford 82 for descum

Venting the chamber 

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-034.jpeg)



We realized that no Cr etch is left. We call it a day. We will need to run descum and Cr etch tomorrow.

The next day, we resume where we left off.  I am running 10 min preclea of the 100

We will descum for 1:30

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-035.jpeg)

Before season for 4 mins on 100

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-036.jpeg)

We then do the full etch for 7 mins

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-037.jpeg)

Took 2 mins to Cr etch 

During etch

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-038.jpeg)

I forgot to remove edge bead, so we are going to do a quick clean clean before acid etching

Some gunk on wafer

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-039.jpeg)

we now do Cr etch for 20 mins and BOE dip for 20 seconds

After

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-040.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-043.jpeg)

Waveguides look un effected by dust. Probably just water or edge bead issues

### Oxide Capping

We first cleanf or 10 mins.  We do oxide deposition for 9 and 8 mins

Before season 1

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-044.jpeg)

Before dep 1

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-045.jpeg)

Before dep 2

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-046.jpeg)

We do 8 mins smooth oxide dep

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-047.jpeg)

Cleaning 10 mins

### Oxide Thinning

We now do season of the 100 for two mins (I left it clean).  We then etch for 13.5 minutes like last time.

Before seasoning

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-048.jpeg)

Edges are comically dirty

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-049.jpeg)

We now do 13.5 mins of etching

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-050.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-051.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-052.jpeg)

This is less than I expected. We should have around 2000, though I am going to check the sides now

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-053.jpeg)

No idea why the middle had so little. Mate we should put like 2 mins of smooth on again

Another central spot

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-054.jpeg)

We, def less. We probably over etched a bit. Either way, we can at least do RTA

During calibration

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-055.jpeg)

During main run

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-056.jpeg)

# PECVD

We add some extra oxide. We do 2.5 mins of smooth oxide.

## Oxide dep 

After cleaning.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-057.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-058.jpeg)

14:52 Starting.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-059.jpeg)

## Cleaning

We do 5 mins cleaning.

Starting

## Seasoning

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-060.jpeg)

15:14 Seasoning start.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-061.jpeg)

## SRN deposition

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-062.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-063.jpeg)

32 mins starting now.

16:01 Venting

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-064.jpeg)

## Cleaning 40 mins

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-065.jpeg)



After PVD

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-066.jpeg)