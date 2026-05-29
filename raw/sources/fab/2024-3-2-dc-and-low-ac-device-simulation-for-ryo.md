---
type: craft-export
title: "2024-3-2 dc and low ac device simulation for ryo"
craft_document_id: 1828F793-9300-41B2-BAB7-5583A2C10A8B
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-3-2 dc and low ac device simulation for ryo
The purpose of this note/simulation is to documnet my work on Ansys simulations investigating the ideal DC device (bascially, does our field contrast reduce as we have better conductivity, and to investigate Ryo’s device and to see the index contrast he achieves..  This will hopefully help us get a better intution for how our devices work.

The inital values I am using for a flat SRN device for Ryo are:

SRN_bright: eps = 8, cond = 1e-7

SRN_dark: eps = 8, cond = 1e-10

oxide: eps = 4, cond = 1e-12

Ta2O5: eps = 27, cond = 1e-12

Cr as high voltage and Si as ground, but choice really does not matter anyway.

Note Si substrate was cond = 0, but should not matter because it is ground.  Below is what I see

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-001.png)

Above is full device, but this is clearly useless as we can’t see into the core.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-002.png)

Above is freq = 0 (DC)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-003.png)

Above is freq = 2.  So we get better magnitude of contrast here, though the high contrast regions have shrunck a bit.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-004.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-005.png)

The files are saved as Pos1_Ryo, where pos is top, bottom, or middle.  Bascially, we have not observed any saturating effect yet. My best guess is that the conducitvty of dark state SRN is too high.  Lets make it closer to 5e-12.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-006.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-007.png)

So, evidently, that was too low (it bascially behaves like DC).  On the bright side, this already shows DC devices are useful even without etching.  We don’t see any cut-off effect.  We should restrict ourselves to 0-4 hertz with 0.2 intervals.  Lets try 1e-11 next for dark.  Above data is 2

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-008.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-009.png)

We are very close.  If we zoom in a bit on the frequecny graph (Exclude the first few points) we get

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-010.png)

So zooming in, we can see that there is a prefered freuqency.  This data is 3

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-011.png)

Above is what Ryo observed.  So we are not quite in the right range, as he used miliihertz.  So we really want something closer to DC to make this all work.  I think dark state and core/clad conductivity matter the most.  I am going to redo data 2 with cond = 5e-12 and see if that gives us a small hump.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-012.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-013.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-014.png)

So we still see this rounding effect, though obvously at a lower frequecny.  What we do not see, however, is the decaying off as much.  The plot is not going down a lot.  This does not feel a lot like our first 5e-12 simulation, so lets try with a greater frequecny range and check stuff.  What is super interesting is DC just does not have a continuous behavior.  So smaller frequecny does not really converge to DC solution is this is to be trusted.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-015.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-016.png)

Zoomed in



![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-017.png)

The hump is in the same spot and we qualitiatively agree with before (both the first time will did the simulation and hump placement).  So this fifth simulation confirms the results from 2 and 4.  I am still really nervous about the DC solution, just because it looks so discontinuous.  While I could try to get something higher resolution there, I am not sure it is worth it yet. To confirm Ryo’s results of a peak of about 1/10 of what we have in frequnecy (about 15 mHz), we probably just decrease all of our conductivities by a factor of 10.  Lets give that a quick try.

I reduced SRN_bright, oxide, Ta, and SRN_Dark all by 1/10

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-018.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-019.png)

Zoomed

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-020.png)

So ya, under 0.1, which is in the range we are looking for.  We should have run higher resolution here.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-021.png)

Also, the blue line aboe is 60hz.  Evidently, not much contrast.  We will do one more simultion with much better resolution to try to find this frequency.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-022.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-023.png)

Above is zoomed in.  So the peak is between 50 and 100 mHz.  So maybe hack another factor of 10 off conductivity, but we bascially get the ideal.  Ta is super insulating if it is dominating the resistivity of the waveguide (which it should be because LN does not observe this effect).

I reduced SRN_bright, oxide, Ta, and SRN_Dark all by 1/10

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-024.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-025.png)

Ok, so we definatley have found a way to get the ideal frequency into the correct range.  It is a tad small, but we can adust our conductivities up a bit to deal with this.  Now lets see if we can use the values Ryo found for conductivity.  Above is 8.  Below, for 9, I am going to use:

Ta: 5e-14 (8 uses 1e-14)

oxide: 5e-14 (8 uses 1e-14)

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-026.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-027.png)

So, evidently, we have not hit the right frequency yet.  It seems like something is off in Ryo’s measurements.  Let me quickly try to get the oxide and Ta much closer to SRN.  Here is what I plan on using

Ta: 8e-11

oxide: 8e-11

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-028.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-029.png)

This is really cool!  So it really seems that, if we get near DC, the conductivty does not matter much.  The above curve is not even zoomed in.  So we are really close!  Lets quickly make the oxide conductivity a factor of 10 lower (to 8e-12) and see if that effects this frequency.  The above device is 10.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-030.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-031.png)

So it bascially seems like lower oxide conductivity causes the corner frequency to move.  So we don’t want lower oxide conductivity.  So it really seems like the device is 10 is the best!

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-032.png)

The above graph shows device 10 with square field.  So it might be possible that there is a bit more contrast then I am showing.  The next device will be:

Ta: 2e-11

oxide: 2e-11

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-033.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-034.png)

So this still did not quite move the corner frequncy.  Maybe I need some asymmetry between oxide and (based on result 11).  For now, I am going to leave this here and design an etched device.

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-035.png)

Above is the chi2 (not chi3) graph for device 12.  One of the key trends we notice is that DC devices have a higher mangitude of field in the guiding layer, even if that field might have slightly less absolute value of contrast.

Below’s images are for etched structures, like the image shows

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-036.png)

The width of the towers is p_etch (presently 4) and the period of each structure (which the above showing 2 period) is 6.  Below is what I see using the same values as I did in 12.

![Screenshot 2024-03-03 at 2.41.09 PM.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-037.png)

![Image.png](../../assets/fab/2024-3-2-dc-and-low-ac-device-simulation-for-ryo-038.png)

This file is save as 1_Etched.  What is suprising here is that etching does not give us any better contrast than the normal flat SRN structure.  And this is with smaller features than Ryo is working with.  So this makes me pretty convinces that they will not be helpful for Ryo.  This, on its own, is a pretty cool find.  It also makes me susepct our field contrast was already saturated with the period of 6 with the flat electrod (and a bright width of 2um).  