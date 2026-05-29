---
type: craft-export
title: "2024-7-26 ansys simulations for sinx etching 1"
craft_document_id: 97869937-2FB4-4CE9-9F8F-87BF45AC5AEB
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-7-26 ansys simulations for sinx etching 1
The goal of this document is to learn a little bit of Ansys Lumerical and then try to find the dispersion of an etched SiN waveguide 

Below are some preliminary sweeps I was able to do

Frequency sweep for waveguide that is Si and 0.22 by 0.5

![Screenshot 2024-07-29 at 9.33.12 AM.png](../../assets/fab/2024-7-26-ansys-simulations-for-sinx-etching-1-001.png)

waveguide height sweep for a waveguide that is 0.5 wide at 1550 nm

![Screenshot 2024-07-29 at 9.32.25 AM.png](../../assets/fab/2024-7-26-ansys-simulations-for-sinx-etching-1-002.png)

So we can evidently do some basic sweeps, though it would be nice to combine these into one 2D plot.  I am also not totally sure what exactly Ryo is looking for at the moment, so it might be best to ask him what type of plot specifically he is interested in

Phase mismatch. We want piling period above 10um but not too large

Walk of. Find difference in group velocity. Also derivative of delta k (though it is the same thing)

You either want this to be very small or very large

If this number is small, then we can do super continuum generation 

Group velocity dispersion (just dispersion) either very large or very small

Plot width vs height and then the values we care about

![Photo from Library.jpeg](../../assets/fab/2024-7-26-ansys-simulations-for-sinx-etching-1-003.jpeg)

