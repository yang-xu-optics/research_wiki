---
type: craft-export
title: "2024-7-29 srn dc device expected values"
craft_document_id: 24746401-5942-4C96-9F85-FA8937B4409E
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-7-29 srn dc device expected values
We have now done a tonne of characterizations of the delta_n of some of my SRN DC waveguides.  Now it would be nice to try to explain the results doing some conductivity sweeps.  The hope is that we can also do some conductivity characterizations of the SRN chips such that we have more data to work with (ie, data that is experimental), but we also have two data points and some rough estimates to get started with.  This might even help us estimate the chi3, as I genearlly trust our conductivity measurements.

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-001.png)

Above is our predicted indexes for the DONs.  As I will show below, I get very good fits for the SRN values and index of DON to predict the conductivity.  The fits are below

![Screenshot 2024-07-28 at 3.19.15 PM.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-002.png)

![Screenshot 2024-07-28 at 3.19.05 PM.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-003.png)

![Screenshot 2024-07-28 at 3.18.55 PM.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-004.png)

We can insert the index and/or silane flow to get the predicted conductivity fits.  FWIW, I am not certain if the bright fits are perfect, but we will start with them and tone down the cond0 in case the fields seem too high

Below are our predicted fits

Bottom Oxide

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-005.png)

Top Oxide

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-006.png)

I just updated the values in my simulation

Now doing 3.5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-007.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-008.png)

Below are the results after simulating Thickness = [3, 2.5, 3]

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-009.png)

Now for the experimental result

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-010.jpg)

Not totally dissimilar, though these are really though fits as we don’t know the size of chi3

SRN4

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-011.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-012.png)

Experimental Result

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-013.jpg)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-014.png)

SRN 4.5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-015.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-016.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-017.jpg)

Simluation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-018.png)

SRN 5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-019.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-020.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-021.jpg)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-022.png)

SRN 5.5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-023.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-024.png)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-025.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-026.png)

SRN 6

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-027.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-028.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-029.jpg)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-030.png)

SRN 6.5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-031.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-032.png)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-033.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-034.png)

SRN 7.5

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-035.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-036.png)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-037.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-038.png)

SRN8

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-039.png)

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-040.png)

Experiment

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-041.jpg)

Simulation

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-042.png)

Some basic take aways are as follows:

1. For almost all of these, the bright state conductivity is just too small.  while I think bright state chi3 increases, not by this much.  We were predicting 10000-100000 times more conductive, which is ridiculous.
2. Around SRN 5.5, our dark state conductivities seem to show annoying kinks that we could not otherwise explain.  Either our simulation does not run long enough or (more likely), our predictions are too resistive.  There is something to be said here for just using the raw values we expect

After playing around a bit, it does seem possible for hte bright state to get slightly more field into the core.  Granted, we could just have some numerical BS going on now, but it seems legit

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-043.png)

Conductivities that I used 

![Image.png](../../assets/fab/2024-7-29-srn-dc-device-expected-values-044.png)

And I plotted the fields as a function of time, and there was no shorting