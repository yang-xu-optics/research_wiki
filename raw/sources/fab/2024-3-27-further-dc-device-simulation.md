---
type: craft-export
title: "2024-3-27 further dc device simulation"
craft_document_id: C14D0783-8840-4D00-99A5-C6436FFEC208
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-3-27 further dc device simulation
The purpose of this document is to do some futher simulations of DC devices.  I am interested in seeing if there is anyway of tuning the conductivity of the top oxide (as it gets thicker) to try to preserve a working device.  The issue, as we noticed in previous simulations, is the thicker the top cladding, we losing a lot of E-field contrast.  We hope to see if there is anyway around this.

After that, I am going to simulate whether there is anyway to implement the 3-layer DC device Ryo and I conspired up.  I will also see if any additional top layers will help the device.  

For top cladding, we are first going to simulate the device with the following constant parameters

Core: cond = 1e-10, L = 1um

SRN_bright: cond = 1e-8, L = 2um

SRN_dark: cond = 1e-11, L = 2um

Bottom cladding: cond = 2e-10, L = 2um

For are going to scan over the ideal cladding conductivity values for L = 1um, 1.5 um, and 2 um for the top cladding.

For L = 1um, we scan over cond = 0.1e-10, 0.5e-10, 1e-10, 2e-10, 4e-10, 6e-10, 1e-9.

After a few simulations, we can clearly see that decreasing conductivity is helpful.  This means our new scan is 1e-13, 1e-12, 5e-12, 1e-11, 5e-11, 1e-10

Below is 1e-11 for 2um thick.  We get maximal contrast when the green curve goes through our middle.  This means we are not getting conductive flattening or resistive domination.

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-001.png)

The general trend seems to be that a facot rof ~10 decrase in conductivity for thicker films seems to work.  I am now going to do a sweep where the top and bottom claddings (which will be labelled with a BT) will have the same thickness (3um) and have the same conductivity.  I will sweep from 1e-10, 1e-11, 1e-12, 1e-13 to find the optimal spot.  The gist seems to be that we eliminate inwanted currents with more resistive films.

Below are results for my simulations

Bottom 1um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-002.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-003.png)

Middle 1um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-004.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-005.png)

Top 1um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-006.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-007.png)

Sorta what I expected.  Matched resistivity for the baseline 1um thick top oxide is the expected result (though I do wish I had looked at slightly higher conductivity numbers to make sure)

Top 1.5um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-008.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-009.png)

Middle 1.5um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-010.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-011.png)

Bottom 1.5um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-012.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-013.png)

So, once more, the matched conductivity works the best.  A bit suprising.

Bottom 2um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-014.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-015.png)

Middle 2um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-016.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-017.png)

Top 2um:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-018.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-019.png)

Lets do the three cases for 1e-10 for the different thicknesses

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-020.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-021.png)

We still confirm the same result from last time.  

Below are the results from the 3 layer devices

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-022.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-023.png)

These are for the 3um top and bottom claddings.  Notice the above plots are not quite linear

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-024.png)

Above is the more linear plot.  Lets try some higher conductivties for the 2um device.

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-025.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-026.png)

So ya, it bascially seems like there is no way to get around the problem of thicker top oxide.  We really do need to have the same resistivitiy.  

So this puts to bed the hope to get a useful device with a thicker cladding.  Lets now simulate the three layer device (possibly with an added fourth photoconductive layer ontop).

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-027.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-028.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-029.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-030.png)

Here are the parameters for the above device: 

Top oxide: cond = 1e-10, L = 2um, eps = 4

Core_dark: cond = 1e-12, L = 1um, eps = 8

Core_bright: cond = 1e-8, L = 1um, epes = 8

Bottom oxide: cond = 1e-10, L = 2um, eps = 4

I am overall very happy.  As DC devices go, this is really as good as the contrast will probably ever get.  There are still some werid corner effects and I can’t tell if they are numerical aberations or not.  Either way, I will try to export this to python so I can take more cross sections.  We are both interested in core and cladding field, as both will give some nonlinearity.  Thinking about it, if the claddings display some amount of DC linear behavior, I could also get effective delta =_n from cladding getting bigger instead of core getting bigger.  After all, both will push the effective index in the direction I want.  This is just such an optimal device.  I just hope no loss.

Below is what happens when we export this data to Python:

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-031.png)

So I pretty much match what I see above (we can disregard x and y parts of field, as they really don’t matter).  Below is the X field

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-032.png)

Below is Y field

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-033.png)

I think Y is a bit scuffed.  X does have a bit of field along the edges.  This might be important to share in the future. 

Below is X field where you can see the sign.  Z field is not effected

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-034.png)

I have defined the positive z direction as down, and positive x direction as to the left.  Just a notational thing

Below is the high resolution version

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-035.png)

Now lets take a few cross sections.  Please refer to the above image for the scale of each of the axes.  I am also going to ignore the bounaries between the layers, as that introduces difficulties.

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-036.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-037.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-038.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-039.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-040.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-041.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-042.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-043.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-044.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-045.png)

![Image.png](../../assets/fab/2024-3-27-further-dc-device-simulation-046.png)

The core has a very nice looking field.  It is about 100 times less in the middle, which makes sense, as that is the ratio between the cladding and bright state conductivity.  The contrast seems to flatten as we move further from the core.  We get some weird effects near the corners of the core which I am not sure I understand super well, but a lot of field seems to get there.