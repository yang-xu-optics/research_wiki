---
type: craft-export
title: "2024-11-17 svm annealing at 1100"
craft_document_id: 115E2573-E1D6-464D-AA1A-9E31BBB64B8E
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-11-17 svm annealing at 1100
According to Ryo, it seems that we can anneal SiNx at roughly 1100 C and get rid of N-H bonds.  Below are some excerpts that seem to suggest why we need to go to these tempuratures.

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-001.png)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-002.png)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-003.png)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-004.png)

At some level, I am a bit skeptical of whether we will see a huge loss reduction, because of the thickness of our waveguides.  I just don’t think all the hydrogen will diffuse out.  Then again, we should see some loss reduction.  Moreover, stress might be an issue.  It seems that other people use much thinner waveguides.  It is also not ideal that we don’t have more etched trenches to take the stress cracks either.  The hope basically is that the waveguides don’t crack even if the rest of the film starts to crack.  Our annealing recipe is below

Gas: N2

Load: 300

Ramp: 160 mins (300 → 1100 at 5 C/min)

Anneal: 180 mins (3 hrs at 1100)

Ramp down: A while (Overnight, I will just log off)

According to the CNF website, it seems that the furnace I want to use only goes to 1100 C ([https://www.cnfusers.cornell.edu/node/63](https://www.cnfusers.cornell.edu/node/63)).  We can manually set the tempurature setpoints in the software.

We are going to start by cleaving and wet etching our samples

# Wet etching

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-005.jpeg)

10:12 20 mins Cr etch



# Furnace

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-006.jpeg)

We use this tube

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-007.jpeg)

In files, we open

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-008.jpeg)

Open tube 3

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-009.jpeg)

Choose recipe. We then change the temperature and time.

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-010.jpeg)

Unload at 300

Load at 300

Ramp is 1100

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-011.jpeg)

Ramp time 160 mins

Anneal 180 mins

Unload at 300

120 mins

Go to files

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-012.jpeg)

Hit save

Overwrite the existing recipe

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-013.jpeg)

ITS onrhe desktop

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-015.jpeg)

Download

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-016.jpeg)

Begin download

Operate

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-017.jpeg)

Select recipe

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-018.jpeg)

Select the recipe

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-019.jpeg)

We hit run whenever is ready

10:41 Hitting run

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-020.jpeg)

We manually unload

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-023.jpeg)

Switch to auto mode. 2

Step lets you skip

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-024.jpeg)

Decreasing load speed

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-025.jpeg)

5 ipm 

After anneal

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-026.jpeg)

I then cracked it open and logged off

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-028.jpeg)

It’s hot

It seems to be cooling off

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-029.jpeg)

It is dropping a bit fast, but oh well

After 4 hours

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-030.jpeg)

Now time to unload at 3 inches per minute

During unload

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-031.jpeg)

Image of waveguides

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-033.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-034.jpeg)

Very close

Other piece

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-037.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-038.jpeg)

Top view

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-039.jpeg)

Observation a couple of days later to see if there is transient solution

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-040.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-17-svm-annealing-at-1100-041.jpeg)

More of those delamination center than I remember 

But cracks did stop where expected

