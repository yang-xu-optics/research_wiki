---
type: craft-export
title: "2024-9-24 ln dc device parameter sweep"
craft_document_id: 04D7E739-193F-44A0-B52A-337CD86B6117
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-9-24 ln dc device parameter sweep
We are almost ready to ship a wafer to nanoLN!!  This means we have to do a more detailed scan of the performance of my LN DC devices.  The hope is that we can figure out the following:

1. Optimal thickness of bottom cladding
2. Effects of changing cond0 of the bottom cladding
3. Optimal thickness of top cladding in three layer device

We would ideally create a prediction plot of delta_n in the process so we could report a FOM number to the group.  The plots I would like to create (in the following order) are

1. Modulation efficency for core thickness (just to get an idea of how suboptimal we are)
2. Loss via substrate loss (as sanity check)
3. Data sweep of bottom oxide thickness and cond0
4. Once we have something roughly optimal for 3, then sweep PC thickness

Optional:

1. Loss calcualtion (though these are very hairy)
2. Ansys maxwell electrostatic field calculator (for fringing)

Below are some preliminary results for modulation efficency (using SiH4 = 4 PC and B27 annealed bottom oxide)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-001.png)

And below is substrate loss for the same configuration

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-002.png)

I am pleasantly subrised that we get a modulation efficency of ~75%.  Substarte loss is a bit higher than I was expecting, but not unreasonable either.  We will just have to deposit longer is all.

The more suprising results are below.  It seems that the cladding thickness and conductivity does not matter a tonne (granted, I may have just picked an optimal SRN).  

For cladding thickness (cond0 is 1e-12)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-003.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-004.png)

For cladding conductivity (cond0 specifically, as exponent is roughly the same in general) (thickness is 1um)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-005.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-006.png)

It seems that, if you optimize your voltage correctly, you can basically get roughly optimal delta_n performance.  There seems to be a small trend for cladding thickness, but not cladding cond0.  either way, their trend is fairly minimal.  For refernce, below are the “Constant” factors for the rest of the device that I chose.

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-007.png)

Only issue is that RC time constant is a bit long (~0.5 seconds).  Again, I really think that hte most important variable here is the SRN, not the cladding.  I will now do a 2D plane sweep of both cladding thickness and conductivity.  I will continue to assume ideally photoconductor behavior.

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-008.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-009.png)

Below are constant parameters

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-010.png)

While the effect is not dramatic, it seems that we get a ~20% reduction for thicker or more resistive claddings.  It seems we were not near the peak voltage either.  It is possible that the RC constant in those regions is simply very long.  

So, after doing a quick simulation, it does seem that the RC constant in those regions is fairly bad (~2 seconds).  I am going to increase the N resolution and run the simulation again.  This being said, we should acknowledge that this type of performance is fairly bad.

After a longer parameter sweep

![Screenshot 2024-09-26 at 10.09.55 AM.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-011.png)

![Screenshot 2024-09-26 at 10.10.08 AM.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-012.png)

So it really does seem that more insulating and thicker are bad.  That is somewhat expected tbh.  Anyway, we now have some ideal of the loss, modulation efficency, and cladding parameters we want to use. While we could do a scan of the photoconductor, I don’t know how helpful it would be, as that is something we kinda figure out experimentally.  Other things we could look at is RC constant, but I would want a more finalized idea of what index I have so I know what the losses and efficencies will be

For SRN sweep

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-013.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-014.png)

So an interesting effect here is that, because the exponent of the SRN in bright state is less than the exponent of SRN dark state, it might be the case that this effect dominates.  It is a bit tough to tell though. 

Below is a simulation where both exponents are the same (top is bright, bottom is dark)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-015.png)

Below is simulation where the bright exponent is less (like I found in experiment)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-016.png)

In this case, the dark state is better.  

If you recall from electrical measurements, when we had field predictions base on DON, we got 

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-017.png)

When SRN was the layer we modelled after 

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-018.png)

So it is not inconceivable that these might be accurate results, but is hard to tell.

The idea here is that this is very hard to simulate

Using a bad x-axis (which is linear instead of logrithmic

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-019.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-020.png)

SRN thickness roughnly had the effect we thought.  Hard to tell for contrast though

Final plots:

cond0 dark = 2e-17

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-021.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-022.png)

cond0 dark = 2.e-16

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-023.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-024.png)

Cond0 dark = 2e-15

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-025.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-026.png)

Cond0 dark = 2e-14

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-027.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-028.png)

Cond0 dark = 2e-13

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-029.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-030.png)

Cond0 dark = 2e-12

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-031.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-032.png)

Cond0 dark = 2e-11

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-033.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-034.png)

Cond0 dark 2e-10

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-035.png)

![Image.png](../../assets/fab/2024-9-24-ln-dc-device-parameter-sweep-036.png)

This was actually quite useful.  It basically seems that more conductive SRN does NOT help for delta_n.  In fact, it gets worse at a certain point, with the only consistently good thing being a lower voltage requirement.  Higher switching is better and thicker is better if you are ok using higher voltage

The general conclusion here is that more system is very lenient on its requirements for DON and SRN