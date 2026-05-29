---
type: craft-export
title: "2024-1-25 optimal 3 layer dc device parameters"
craft_document_id: EA65A635-7FC4-4440-858D-9409EA76774C
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-1-25 optimal 3 layer dc device parameters
As of yesterday, I figured out the RC constants I get with a 3 layer DC device.  For one, we were able to show that our symoblic predictions could match up with Ansys simultions.  So, in general, I can always confirm things in Ansys.  At the moment, it is best to see what the RC constant solutions are, then, once I have found a system with the minimal RC constant, check Ansys to see which term dominates.  

Below is my new code (which I checked worked) for a 3 Layer device in python

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-001.png)

I could not get good code for a four layer device as the solution is a bit more complex…

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-002.png)

For reference, above is just one solution, and it uses notation that I am not knowledgeable enough with to transfer into python.  It would be nice at some point to analyze these devices better.

The hope, presently, is to build a 3 Layer device with conductive oxides ([https://tdwg.craft.me/LzHOG0KpfE126m](https://tdwg.craft.me/LzHOG0KpfE126m)) that has the claddings act as the photoconductors.  I am going to simulate the dark state (which should have a slower RC constant).  The constraints from materials and device performance are below:

epsA = epsC = 4.5 (My guess for the permitivity of the oxides, which could be higher or lower)

epsB = 27 (This is the permitivtiy of LN and Ta2O5, which are pretty similar)

LA/condA +LC/condC = LB/condB (The voltage divider works to remove field from layer B)

For LN, I am guessing condB = 1 *10^(-9) and for Ta2O5, condB = 1* 10^(-10).  We will probably use the same recipe for condA and condC, so condA = condB.  It is also reasonable to say that I can't make the devices super different in height, so I am going to start with this guess, even if it is not actually nessasary.

Lastly, we will probably want LB = 800 nm, as this would give us a single mode waveguide.  So our parameters are below:

epsA, epsB, epsC, and condB (up to material choice) are locked in.

LB and condA=condC are relations or constants that I have set but could be tweaked

LC, LA, and the exact value of condA are free parameters.  

Because I need fewer parameters at the moment (I only want to sweep 2 parameters to start with) I am going to say LC=LA

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-003.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-004.png)

Above are our first results.  Basically, as long as we keep our conductivities arond 10^-10, we are getting RC constants which are still less than 1 second.  I am a bit perplexed how some easrlier solutions with Ansys four layer devices showed such short RC constants, but we will get back to that later.  Right now, because there is no difference between the conductivity of layers A and C, the thickness of one layer versus the other really does not matter.  This is also because the permitivities of both layers A and C are the same, so there is symettry.  Lets try to make the conductivity of one of the layers a bit larger and see what we get.  I made condA = condC * 10

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-005.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-006.png)

So the problem here is that, while there is a direction that is favored, it seems that we can’t really get must substantial improvement, as the thickness of the other film is soooo small (far too much so).  That being said, we could just assume we have a very conductive bottom cladding and potentially use the top cladding as the one we modulate.  So we should maybe try in that direction?

As a side note, I tried to test our 4 layer stack, it does seem that Ansys gets results that approximately make sense.  Notice how the first eigenvalue is very large and drops by 10X as the conductivity drops by the same amount.  It may be possible to use this as a device, but I would then need to figure out how to get that mode to dominate.  I will review that later this weekend

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-007.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-008.png)

Below are the results for the conductive bottom oxide (which we presume to have a thickness of at least 1 um). 

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-009.png)

So it seems we can get a really good part to the transient solution.   My question is whether the transient solution we want dominates the expression as time goes on.  I am currently doing an ansys simulation of our previous results to see.  If the smallest RC constant dominates, then I would almost always be able to avoid the RC constant problem by just adding a conductive layer.  If it does not dominate, then we really can’t avoid the issues inherent in using certain films in our stack. 

![Screenshot 2024-01-25 at 9.19.03 PM.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-010.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-011.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-012.png)

So it seems like the long solution dominates in the long run, but it should be noted that the LN layer does start high and only ends a bit less high.  The result could be worse, but it means the device is kinda useless for a bit as the fields adjust.  So we really want to minimize the long time constant.

Let’s check if the oxides are following the same long term change as the rest of the stack.  But otherwise, it seems this result is pretty conclusive.



![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-013.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-014.png)

Basically, the long time constant dominates for a while.  The last question here is whether there are many limits on the conductivity of the guiding layer.

For this last investigation, I am going to assume Layer A is 2 um thick and have a conductivty of 1e-8 (basically, pretty low), and assume layer C has a conductive that is half of Layer B.  Layer B will be 1 um thick, and layer C will be 700 nm thick.  We want to see if Ta2O5 can also work, in addition to LN.  After this, we bascially know our stack.  We want RC constants that are < 1second, but pretty much anything under that is fine with me.

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-015.png)

So it definately seems that LN should be fine.  Lets limit our search area a bit more…

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-016.png)

![Image.png](../../assets/fab/2024-1-25-optimal-3-layer-dc-device-parameters-017.png)

So, bascially, we really can’t use something much more insulating than LN, as the time constant would take a while.  10-10 is approximately the cut off point.  10-11 would take on the order of 10 seconds to refresh, which is a bit slow.  Fortunantely, this is not hours, but it is not great either.  

After playing around with the numbers a bit more, here are some things I notice:

A lower epsB gets a better tau

EpsA and EpsC really don’t matter

A thicker core gives a slight benifit

Higher condA, at a certain point, stops mattering (as long as it is a factor of 10 smaller than the core)

My end conclusions are as follows: Using LN (or some similarly conductive) material as the core would be great.  We can probably stomach up to 10-11 for conductivity, as that will only take 10 seconds to update.  Anything lower would be a problem.  We are really limited by the core conductivity, and there are not many ways to substantially improve the stack’s performance as we are limited by the largest tau.