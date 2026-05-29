---
type: craft-export
title: "2024-10-09 etched nonlinear device ansys field simulation"
craft_document_id: 3F751882-D91D-44AF-9CBF-99F4626669CC
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-10-09 etched nonlinear device ansys field simulation
Below is the device before I put the ITO electrodes ontop

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-001.png)

I assumed conformal deposition for TEOS and directional deposition for SRN (though I don’t think the distinction matters much).

Now with ITO electrodes ontop (as we can’t see the bright and dark state now)

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-002.png)

I now applied symettries and put ground and high voltage plane on

With everything as complete capacitor in DC

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-003.png)

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-004.png)

This is to be expected.  Now lets get some bisection lines in each of these planes and try to see what the fields look like for different frequencies

We seem to be stuck in place where I can’t get the region between total capacitcence and resistance. 

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-005.png)

I am going to raise the SRN conductivity.  Below are the plots to reference:

![Screenshot 2024-07-28 at 3.18.55 PM.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-006.png)

![Screenshot 2024-07-28 at 3.19.05 PM.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-007.png)

Ryo uses SRN 8.  I am going to guess dark state is 1e-9 and bright state is 1e-6

Next, I am going to say SiNx waveguide is 1e-17 and SiO2 is 1e-19

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-008.png)

This seemed to help, but an interesting effect is that higher freuqnecy is lower on the dense section and lower frequency is higher (though DC at bottom is still useless).  I will start scan lower

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-009.png)

It turns out that lower really was not nessesary.  It is a bit annoying that I can’t access the very lower freuqnecies, as there must be a point when the thin moves from DC to AC

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-010.png)

Still impossible to resolve.  At this point, I say we do a 50 point sweep from 0 to 50 (Step size is 1).

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-011.png)

We now have a useable plot.  I say that we try sweeping the following:

1. TEOS thickness
2. SRN thickness
3. Pad Oxide thickness

We could also try some waveguide dimensions as:

1. Sidewall height
2. Period

Lets do TEOS first, with a scan over 0.6 to 2um (0.6, 0.8, 1, 1.2, 1.4, 1.6, 1.8, 2).  I think I will just take Top, Middle, and Bottom cross sections in YZ.

I used 0.3 pad oxide for TEOS simulations and 3um SRN.  

For SRN thickness, lets do 1, 1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5, 5.5.  I am using 0.3 pad and 1 um TEOS.

For pad oxide, lets do 0.1, 0.2, 0.3, 0.4, 0.5, 0.6.  1um TEOS and 3um SRN

For the above simulations, I used a sidewall height of 1um and a period of 10 with a bright spacing of 5um.  

For sidewall height, lets do 0, 0.25, 0.5, 0.75, 1, 1.25, 1.5, 1.75, and 2.  I will still keep core thickness at 2, as that is what the SVM is.

Interesting that we see a big contrast between the area with the pad and no pad oxide.  

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-012.png)

A quick feuqnecy dependance for the base device is below:

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-013.png)

Take this with a heavy grain of salt, as I really did not probe musch below the lowest frequency shown above

All of my results are below (Take them with a pinch of salt, as these are qualitative measures of performance)

Middle TEOS

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-014.png)

Middle SRN Thickness

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-015.png)

Middle Pad Oxide:

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-016.png)

Sidewall Height Middle:

![Image.png](../../assets/fab/2024-10-09-etched-nonlinear-device-ansys-field-simulation-017.png)

This is not all of the data, but it is good enough to understand the general idea.  My conclusions are as follows:

1. A deeper sidewall moves you get more fields into the core for the same applied voltage.  The net contrast seems to remain the same.
2. The thinner your pad oxide, the better
3. It is unclear if a thicker SRN matters a tonne, but it definately reduces the magnitude of field.  The contrast seems to be the same.
4. The thinner your TEOS, the better