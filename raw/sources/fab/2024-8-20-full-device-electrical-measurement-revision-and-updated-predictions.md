---
type: craft-export
title: "2024-8-20 full device electrical measurement revision and updated predictions"
craft_document_id: 45C40FE4-EDC9-4929-A9FE-651F4EE60600
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-8-20 full device electrical measurement revision and updated predictions
Previously, I took data on the full device resistances of SRN DC linear waveguides.  My model was a tad flawed, and tried to fit for ht efield in the SRN instad of the cladding.  Because the claddings were thicker, they ultimately effected this nunmber more in the bright state.  The first thing I am going to show below is new fits with updated paremeters of the conductivity fits.  I am going to plot these new parameters as well.  

After that, I am going to use these bright state characterizations nad previous dark state characteriationg (along with standard DON characterizations) to see if I can roughly predict the shape of my delta_n optical measurements.  The hope is that this entire process will allow us to verify our model.

SRN 4.0 (0.9 by 0.4)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-001.png)

Recall Sigma 1 is for SRN and Sigma 2 is for cladding.  Conversion factor is for field in the cladding

SRN 4.5 (0.3 by 0.7)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-002.png)

SRN 5.0 (0.4 by 0.8)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-003.png)

SRN 5.5 (0.7 by 0.5 triangle)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-004.png)

SRN 6.5 (0.4 by 1)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-005.png)

SRN 7.5 (0.4 by 1)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-006.png)

Now that we have all of these numbers, lets compare the graphs from this time to last time.

With the cladding as the reference (this time)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-007.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-008.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-009.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-010.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-011.png)

Last time (with core as the reference)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-012.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-013.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-014.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-015.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-016.png)

Now for comparison:

- The SRN cond0 graphs look mostly the same, though the ones from last time are about 10X smaller
- The DON cond0 graphs look fairly similar too, but again with a factor of 10 differnece.  Interesting that we just predicted something 10 larger from last time.
- SRN expo this time is a bit smaller (not quite factor of 10 though, but this could be the entire difference)
- DON expo of last time is a bit larger (like factor of 2-10).  
- For last time, we expected less field in the core as the silane went up.  We sorta got this.  This time, we expected more field in the cladding as the silane went up, which we mostly got

Given when I have written above, it is unclear which fit is better.  I guess there is a believability issue here, and I just don’t know what to expect. Maybe compare to previous understanding of the DON conductivity?

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-017.png)

So it does seem like last time is closer, as we really do expect something in the 1e-11 to 1e-12 range.  We will go forward with those numbers then (but I will say this much, we see no clear exponential trends here, which is kinda sad for cond0).  I think half the issue here is where the simulation is sensitive.  It is not sensitive to SRN cond0 for high silane flow, and it not sensitive to DON cond0 for low silane flow.

Now lets do some new voltage sweep simulations

SRN 4.5

![SRN4.5_delta_n.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-018.png)

Simulation

![SRN4.5 Theory.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-019.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-020.png)

I used DON values from fitting, SRN dark from previous characterizations, and SRN bright from fitting

SRN 5.0

![SRN5_delta_n.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-021.png)

Simulation

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-022.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-023.png)

Getting agreement here is going to be tough, though the shapes have not been that off yet.

SRN 6.5

![SRN6.5_delta_n.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-024.png)

Simulation

![SRN6.5 Theory.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-025.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-026.png)

Again, with the correct chi3 scaling, this might work, but it is hard to tell

SRN 7.5

![SRN7.5_delta_n.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-027.png)

Simulation

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-028.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-029.png)

This graphy looks very good.  We finally have some agreemnet.  The thing seems to be that we no longer observe this huge change in the chi3 in bright state.  I think SRN6.5 had a messed up coefficent in front, so let me correct it

SRN 6.5 2.0

![SRN6.5_delta_n.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-030.png)

Simulation 2.0

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-031.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-032.png)

Ok, so more reasonable.  Now lets try our best to fit for the chi3 coefficent using these field graphs and the delta_n and see what we get

As a warning to the future reader, the plots below were fitted by hand.  I have not yet figured out a way to make the fit function automated, so these are rough guesses to get me going

SRN 4.5

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-033.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-034.png)

SRN 5.0

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-035.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-036.png)

SRN 6.5

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-037.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-038.png)

SRN 7.5

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-039.png)

![Image.png](../../assets/fab/2024-8-20-full-device-electrical-measurement-revision-and-updated-predictions-040.png)

So there are a few issues here.  One, I seem incapable of fitting the dark states even remotely close (and the bright states are only marginarlly better).  There is also no noticable trend for the chi3 of the bright state, but a noticable trend for the chi3 of the dark state.  It seems that the bright dark gap disappears for higher silane flows, which is also a bit mysterious.  It feels like we need a more general quadratic function to understand how the field translates into delta_n (basically, a chi2 term as well).  But I am still a bit spooked by the lack of a fit function.  It would be nice if, for all these delta_n curves, I could get that.  I just wonder if I have enough data points for it to be useful