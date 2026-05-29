---
type: craft-export
title: "2025-06-25 further baseline loss test for tapered and origonal pattern"
craft_document_id: 052442E1-763A-4798-AA5D-A06F0C6B218D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-25 further baseline loss test for tapered and origonal pattern
We are still having issues with Loss in the tapered waveguides.  The losses are still a couple of dB/cm, far higher than the 0.5 dB/cm we expect.  We are going to try to exactly replicate our previously working oxide hard mask on the new SVM wafers that gave us 0.5 dB/cm.  If this does not work, I am biased towards either blaming the tools in the CNF, or simply say this new SVM is just bad.  I really don’t have a great reason to suspect this is going to work, but hey, we did it before, and nanofab should be reproducible.  We can add some eco clean and piranha steps if we want, but that should not make a huge difference (it should theoretically only help). 

The hope from this baseline is that it would somehow help us to understand whether one of the tools is broken, and hopefully give us a baseline understanding of the SVM loss, as we could not simply use the longer spirals as a more reliable baseline.  Maybe we could at least compare spiral losses on the two wafers to see how bad the taper is.

### Photolihography of baseline wafer

Before arc

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-001.jpeg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-002.jpeg)

Before edge clear

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-003.jpeg)

During edge clear

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-004.jpeg)

Before main run (using exact same recipe as before)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-006.jpeg)

I adjusted both doses. They did not start out the same, so past device might have different waveguide widths for medium and long

During run

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-007.jpeg)

Before developing

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-008.jpeg)

Images of tapered mask

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-009.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-012.jpeg)

### Etching

We do a 5 min preclean of 82 and 100.  We only need to descum one wafer.  WE spinly spin dried the other

Before seasoning oxide of 1

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-013.jpeg)

1:20 descum

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-014.jpeg)

We now do 9.5 minute etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-015.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-016.jpeg)

We will do eco and piranha clean

We do 11 min clean on 100

We do 2 min strip on eco clean

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-017.jpeg)

Seems to be going

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-018.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-019.jpeg)

During piranha

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-020.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-023.jpeg)

Spot on etch, and the numbers check out 

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-025.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-026.jpeg)

Everything looks very clean.  I have not noticed any issues with these oxide etches either



Before second oxide etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-027.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-028.jpeg)

We run ecoclean again

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-030.jpeg)

During second piranha clean

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-031.jpeg)

Let’s do 2 minute season for nitride etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-032.jpeg)

We do a 6 minute etch on the tapered wafer

During etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-033.jpeg)

Given the amount of O2 flow and the fact that we did not clean there last time, I am good going straight to the cap.  I will take images beforehand.  I will clean chamber for 6 minute

After

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-034.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-037.jpeg)

2 min season for the next wafer

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-038.jpeg)

Before second etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-039.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-040.jpeg)

Inspection after etch

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-043.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-044.jpeg)

### PECVD

We start a 10 minute pre clean

Before first season

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-045.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-046.jpeg)

We now do an 8 minute clean. Hopefully these will end around the same time

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-047.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-048.jpeg)

### RTA

Calibration

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-049.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-050.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-051.jpeg)

### Loss test

We use edfa 10x main setup at 1570. Input power is 76 mW

Normal RTA die 2

Straight 1

5.9 mW

Straight 2

6.7 mW

Straight 3

5.3 mW

Straight 4

5.2 mW

Straight 5

5.3 mW

Large circle

2.3 mW

Large square

2 mW

Medium square

0.7 mW (weird output shape)

Medium circle

Could not find (might have cleave by accident)

Got a bit dangerously close to the edge on the previous chip



Die 2 of normal RTA

Straight 1 

6.5 mW

Straight 2

5.6 mW

Straight 3

6.7 mW

Straight 4

5.2 mW

Medium square

2.8 mW

Medium circle

2.5 mW

Large circle

2.4 mW

Large square

Could not find



Tapered 3 um RTA

Straight 1

6.3 mW

Straight 2

4.5 mW

Straight 3

7 mW

Straight 4

5.3 mW

Euler

3.2 mW

Short circle

2.7 mW

Long circle

2.1 mW



Die 2

Straight 1

5.5 mW

Straight 2

5.1 mW

Straight 3

5.1 mW

Long wide adiabatic

4.9 mW

Short wide adiabatic 

4.1 mW

Long narrow adiabatic

2 mW

Short narrow adiabatic 

2.6 mW

Euler

3.4 mW

Short circle

3 mW

Long circle

2.3 mW



Tapered 2um RTA

Straight 1

6.5 mW

Straight 2

5.7 mW

Straight 3

5.4 mW

Straight 4

6.4 mW

Euler

3.3 mW

Long wide adiabatic

4.8 mW

Short wide adiabatic

5.6 mW

Long narrow adiabatic

4.6 mW

Short narrow adiabatic

Low

Short Circle

2.2 mW

Long circle

1 mW 



Die 2 (use middle one)

Straight 1

5.8 mW

Straight 2

5 mW

Straight 3

5.8 mW

Straight 4

4.8 mW

Long wide adiabatic

4.4 mW

Short wide adiabatic

5 mW

Long narrow adiabatic

4.3 mW

Short narrow adiabatic

4.8 mW

Euler

2.8 mW

Short circle

2.8 mW

Long circle

1 mW



Below are the results.  We are going to use the circular spirals to calculate the loss.  I am going to do the brute force calculation of the euler and adiabatic waveguide averages to get a sense of the variability there

Average Euler:
(2.8 + 3.3 + 3.4 + 3.2) / 4 = 3.2 mW.  Fairly consistent across waveguides, where the difference can be a bad job on my end of bad cleaving



Average Long Wide adiabatic

(4.4 + 4.8 + 4.9) / 3 = 4.7 mW

Average Short Wide adiabatic

(5 + 5.6 + 4.1) / 3 = 4.9 mW

Average Long Narrow adiabatic

(4.3 + 4.6 + 2) / 3 = 3.6 mW

Average Short Narrow adiabatic

(4.8 + 2.6) / 2 = 3.7 mW



While there are not perfect calculations, the rough guess is that the width of the waveguide matters a lot more than the period of the taper (at least at the moment).  So we can make the tapered regions a bit shorter.

Now lets calculate the loss of each of the structures:

Normal RTA

![Image.png](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-052.png)

I just used the straight and long circle from both waveguide dies I tested

Tapered 3um using normal calculation

![Image.png](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-053.png)

Roughly in agreement, so we know the 3um taper using this exposure process is roughly lossless

Tapered 2um using normal calculation

![Image.png](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-054.png)

This case is a bit more tricky, as we do notice an increase (by quite a bit) for the loss from straight to spiral.  We see it a bit with 3um, but not as much.  Anyway, the key here is that we can now see the effect (which is decently substantial), from the taper.  With our lithography proceedure, we still expect that we have 2-2.5 um wide waveguide.  This is not that narrow, so I am not the happiest about this.  Lets try to redo the tapered calculations using the baseline loss from the 1 → 2 (which can treat the taper as some normal insertion loss).  We can guess the tapered region as roughly normal.

Using revised calculation method:

3um taper

![Image.png](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-055.png)

2um taper

![Image.png](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-056.png)

The taper length is probably causing a slight over estimate, as I am counting the full length of the tapered region plus the middle narrow region.  It is a lower bound for the loss in the narrow region, but it gives the useful impression.  It is nice to see that the losses for the linear regions are all incely in alignment.  It is also good that the 3um is roughly not noticing the narrowness.  But the 2um wide waveguides (which are in reality between 2 and 2.5 um because I am slightly underexposing).  