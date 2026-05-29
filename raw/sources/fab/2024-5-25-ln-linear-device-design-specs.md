---
type: craft-export
title: "2024-5-25 ln linear device design specs"
craft_document_id: 8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-5-25 ln linear device design specs
The purpose of this document is to lay out the optimal design parameters for a LN linear DC device.  A lot of these principals can be transferred to the SRN nonlinear device as well.  I want to figure out what thickness for the middle would be best, along with what thicknesses for the claddings would work to keep the mode confined.  At some level, the thicker the core, the better, so long as we are NOT multimode.  We would ideally like the device to also work at multiple frequencies, so we probably want to design the device to work well at our desired telecome wavelenghts, namely 1064, 1300, and 1550.  Below are the relevant LN indexes of refraction

1550: 2.1376

1300: 2.1455

1064: 2.1555

[Refractive index of LiNbO3 (Lithium niobate) - Zelmon-e](https://refractiveindex.info/?shelf=main&book=LiNbO3&page=Zelmon-e)

For our bottom oxide, lets use B12 data, as that is most likely going to be what I use

1550: 1.8886

1300: 1.8926

1064: 1.9019

These films are about equally dispersive, each showing an additional 0.01 for each wavelength jump here.  This means dispersion should not be too pronounced here.

Ryo seems to show good results with SiH4 = 6 sccms, from the following measurement

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-001.png)

I am going to use my ellipsometry for this film.

![Photo from Library.jpeg](../../assets/fab/2024-5-25-ln-linear-device-design-specs-002.jpeg)

1550: 2.1732

1300: 2.1818

1064: 2.1952

Welp, we can’t use that film, the index is just a bit too high.  Tbh, this is a huge pain, as that film really did have ideal operating conditions.  But we are using the extraordinary index of refraction, so we must trudge on like this.

Lets instead do SiH4 = 5 sccms.

![Photo from Library.jpeg](../../assets/fab/2024-5-25-ln-linear-device-design-specs-003.jpeg)

1550: 2.0963

1300: 2.1035

1064: 2.1143

These are lower than LN.  Hopefully, with a bit of silane decimal scanning, we can slip the recipe like SiH4=6 just below the index of LN.  We are now going to plug into our model solver

For d_LN = 0.67, d_DON = 2um, and d_SRN, we get the plot below.  At the begining, we definitely know we will need a thick core.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-004.png)

I am going to do a parameter sweep and see what I get.  This is for 1064 nm by the way and using a delta_n of 1e-2

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-005.png)

As we kinda expected, the thicker the core, the better.  We would prefer not to loose 20% of our programmable delta_n, so 3um seems like the play.  We will have to tell nanoLN this information.  At the very least a micron is needed.  One obvious way to reduce this issue is to use an SRN with a lower index.  This might eventually be the play, but let me simulate through and see what I get.

Below is the plot for 2um of LN as the core

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-006.png)

Below is 1um of LN as the core

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-007.png)

Below is 1.5um of LN as the core

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-008.png)

1.5 might do, but it is annoying that I take this hit. The only reason why a thicker core will be annoying is circular loops of current might kill us with a non-photoconductive bottom cladding.

From here, it seems fairly obvious that this device will confine our mode and not lead to loss of the mode.  We could probably even use a thinner bottom oxide, though based on previous ansys simulations, that is not nessesary.  Some questions that follow now:

1. What are the design advantages of using a thicker or thinner core.  
2. Should we try to insert a doped oxynitride “seed” layer, above the waveguide.  While could cause frindging issues, but if a thicker core is really anissue, this would help shift the mode up a bit.
3. What happens if we use an SRN with a slightly lower index

In theory, if we can easily get a thicker core and it shows no issues, we have a possible device.  The continual issue with a device like this will be multimode behavior, which I imagine will be quite pronounced.  We will also need to simulate how the other wavelengths are efffected.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-009.png)

I was actually quite wrong.  We don’t have a multimode problem, as we can see that the first order mode is quite leaky.  This is probably because our index contrast with the SRN is sooooo low.

Lets do Ansys simulation then

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-010.png)

Above is the device we are going to simulate in Ansys, and we are going to vary the thickness of the middle layer. I am also going to simulate with the following parameters

I am also going to set the following stack layer constants as:

SRN: cond_bright = 1e-8, cond_dark = 1e-10, eps = 8, d = 2um.

DON: cond = 1e-8, eps = 5, d = 2um

LN: cond = 1e-9, eps = 27

I am going to scan d_LN as follows:

3um, 2.5um, 2um, 1.5um, 1um, 0.5um.

I am using a period of 6um and a duty ratio of 2um of bright SRN.  In reality, this might be stupid, as I likely won’t be writing features this small anytime soon.  That being said, if we ever have the ambition of etching these devices, that is not a crazy period anymore.  I am also setting applied voltage to 1.

After 2um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-011.png)

After 2.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-012.png)

3um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-013.png)

1.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-014.png)

1um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-015.png)

0.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-016.png)

By pure observation, we can see that the contrast is greater when the core is thinner.  This might have something to do with the fact that the thickness of our capacitors is on the order of the width of the capacitors.  I think it would be better to simulate these devices for a period of 20 um with a duuty (bright state width) of 10um.  I will simulate 3um → 1.5um for that (not as many points are needed).

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-017.png)

3.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-018.png)

3um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-019.png)

2.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-020.png)

2um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-021.png)

1.5um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-022.png)

It seems, in the approximation where the width >> thickness, then all my previous simulations work.  The issue here is resolution, and a thicker core will limit the resolution we can achieve because of frindging.

Below are the results for a period of 6um

Bottom

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-023.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-024.png)

Middle

![Screenshot 2024-05-24 at 6.45.05 PM.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-025.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-026.png)

Top

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-027.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-028.png)

Now for a period of 20um with a duty cycle of 10um

Middle

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-029.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-030.png)

Top

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-031.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-032.png)

Bottom

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-033.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-034.png)

Something to note.  While it looks like the thickness is bad, this is highly deceptive, 

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-035.png)

As this plot shows (which is not in log-log scale), I decrease with 1/thickness.  So a key draw back is that as the film gets thicker, we just don’t need to put as much field in.  It still looks like some smearing effect is happening, but it is hard to tell.  I don’t think this is the most important parameter, and even if it were, it would be hard to make this thinner.  We will just have to apply more voltage to make this work.  Lets quickly cross check with what our step derivative code has to say.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-036.png)

Quantitative agreement for bright state for bottom and middle of the 20um period, 10um duty cycle simulations.  Top for 20-10 seems to actually be a bit higher interestingly.

For a 6um device, the middle graph agrees with this, top is a bit higher, and bottom is a bit lower.  I think the bottom being lower if the fringing effect.  So it seems that fringing matters at the bottom of thicker devices.  It is intersting though that the top effect to hav extra contrast.  This might be due to some weird horizontal effects?

For Dark state:

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-037.png)

So things should go down to 0.45 v/um.  All of the 20-10 agree with this, but none of the 6um period agree with this.  Looking at it, what is kinda crazy is that the shorter periods get better contrast.  Interesting effect.  For 20-10, the contrast is basically constant.  For 6um, while the contrast does vary (this is fringing effect), it is still impressively big. It does seem to prefer thinner films, but I also did not simulate that thin for 20-10.  My take I think it that we have no huge reason to worry here.

Actually, taking a look, it seems that the shorter periods are just inflated on the left side because they are thinner.  There is NO actual difference.  Overall, the difference in contrast is not super bad, meaning that the only fringing effect is from the field spreading at the bottom of a thick core.

We still prefer the effects of a thinner core.  Lets see the simulations we get for adding a seed layer.

Below is the simulation with a seed layer that is 500 nm thick

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-038.png)

Ignore the weird peak, we verified that this was somehow simulating a leaky mode.  I am going to do a sweep for LN_thickness = 1um

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-039.png)

Anything above 1 is likely some weird numerical issue.  Basically, a small seed layer will do

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-040.png)

This is an example of this weird leaky mode shit

Lets do a quick round of ansys simulations for different seed layer thicknesses in what technically is a DC device

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-041.png)

Here are the constants I am going to put into the simulation

Bottom oxide: Conductivity = 1e-8, eps = 5, L = 2um

Core: Conductivity = 1e-9, eps = 27, L = 1um

Seed: Conductivty = 1e-8, eps = 5

SRN: Cond_bright = 1e-8, Cond_dark = 1e-10, eps = 8, L = 2um

I am using 20 um wide and a period of 10 um

We want to do a scan of the seed layer thickness.  I am going to do the following thicknesses:

0.1, 0.3, 0.5, 0.7, 0.9

0.1

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-042.png)

0.3

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-043.png)

0.5

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-044.png)

0.7

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-045.png)

0.9

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-046.png)

Below are the results:

Bottom:

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-047.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-048.png)

Middle:

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-049.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-050.png)

Top:

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-051.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-052.png)

FWIW, I wish I had used this ratio and linear plot in the past.  It is far more helpful to visualize.  The most obvious result is that there does seem to be reall fringing concerns.  Of course, we should use the transient solutions as our best measure, as they account for non-constant conductivtivty and we can tune voltage to the best possible value.  This simulation is obviously going to suffer from the fact that a thicker top oxide is going to absorb more field.  Still, given that it is 10X more conductive and usually 10X → 2X thinner, I can’t imagine that is the dominating effect.  But, at baseline, this fringing should be concerning, as we definatley want to keep the DON seed layer around 200 nm if possible.

Something that is a bit tough for me to see looking at these simulations is what our expected value should be with a thicker or thinner core.  I think it would be best to overplot on the core and seed layer thickness simulations a quick plot of what ideal resistors in series would do.  This would allow us to see how big of an effect fringing is having.  Below is for seed layer

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-053.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-054.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-055.png)

So, we basically see that we are exceeding the theoretrical maximum.  The reason for this is likely quite simple.  Near the top of the waveguide we are getting a small horizontal component.  The field becomes totally vertical near the bottom.  Basically, I am not concerned about fringing that much from the seed layer here as long as we are only a few hundred thick.  

Now for no seed layer, period of 6 with pertubration of 2

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-056.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-057.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-058.png)

Now for a period of 20 and perturbation of 10

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-059.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-060.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-061.png)

These plots are actually super helpful.  Here is what we learn:

1. There is definatley a notable difference between our results for a smaller or larger period.  This confirms our intuition that the smaller periods will have less contrast (this still assumes block like conductivity profiles)
2. For thicker cores, we do get more fringing.  This is most notable in seeing how the bottom contrast diverges more from the ideal solutionas it gets thicker compared to the top cross section.
3. The effect of the seed layer is a bit harder to understand.  We do have some substantial horizontal fields from that film.  I think that is inflating the values we see.  Nonetheless, it is pretty clear that making the seed layer thicker definately causes field to flatten. I think the bottom case is most compelling, and it seems to indicate that thinner is better.  I would go for 200-300 nm, as that seems to give us a factor of 10X contrast at the bottom, which means higher everywhere else

I would like to improve our ansys simulations such that we only report the verticle field.  This will give me a lot more confidence in my results.  It seems achievable for us to get a factor of 10X index contrast, but I just want to confirm it.  At this point, I think it is better to prioritze delta_n over applied voltage.  We will probably still be around European wall plug anyway when it comes time for us to find the ideal operating voltage.

Below is Ansys result when I pick just the Z-axis (ignore the negative sign, it is just a scale factor for direction)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-062.png)

Below is Ansys result when I JUST plot magnitude

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-063.png)

It does not seem like there is a huge differnce between the bottom and the edges.  It truly might just be the case that a thin seed layer beats ideal case?  This is weird though.  Lets check our previous calculations for top.  FWIW, running the numbers, it seems that we were not wrong.  This is very weird.  Maybe lets look at field overlay?

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-064.png)

This is indeed quite interesting.  The seed layer helps throw field horizontally quite fast.

When we print out the field strength in the bright and dark parts of the device for different seed thicknesses, we get:

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-065.png)

What is most interesting is the bright state is really not effected, but the dark one is.  Back of the envelope calculations don’t reveal much, so there must be some type of interseting divergence from nice behaviour here.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-066.png)

These are not quite the same, as the seed_layer film is 1um core and the other is 1.5um.  It is really quite interesting for the Top.  Lets do the middle and bottom

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-067.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-068.png)

This effect generalizes, showing it is not limited to the top.  This really is quite strange.  Lets see what the ratios are

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-069.png)

For reference, 1 in the above plot is with seed layer.  2 has no seed layer.  I really can’t understany this to be honest.  I am going to do a quick additional simulation of a 1um thick core and 0 seed layer to see what I get, as I just can’t pick out a trend.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-070.png)

I found the issue.  The middle conductivity is 1e-8 by accident

BELOW ARE REAL RESULTS FOR SEED LAYERS

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-071.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-072.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-073.png)

A few interesting take aways.  Firstly, it seems that we get better contrast when the core is more conductive.  Or at least, when the photoconductor is skewed to more insulating compared to the core.  I kinda wonder why.  Lastly is that seed layers do dramatically.  It is suprising that there is still such a huge gap between the ideal and real case.  We can at least see the effects of frindging clearly.  It is just very strange that this more conductive core is better.

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-074.png)

Above is a quick back of the envelope calculation.  Roughly, it seems like a more conductive core (or at least a more insulating SRN) gets better switching ratio.  This does make a lot of sense, as the SRN will totally dominate the resistiance, so the total resistance swing will be entirely dominated by SRN impedance swing.  Still, the issue with this setup is that we also need to use a LOT more voltage to get voltage swing in LN.  And again, a factor of 10 is really all we need.  We should think more in terms of percentages here, and realize that we are trying to go grom 90→95% with a bigger swing.  Kinda not nessesary.

Including with zero thickness

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-075.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-076.png)

![Image.png](../../assets/fab/2024-5-25-ln-linear-device-design-specs-077.png)

Zero (besides for potentially Top) does not substantially increase contrast.  Really not important.  100-200 nm is fine.