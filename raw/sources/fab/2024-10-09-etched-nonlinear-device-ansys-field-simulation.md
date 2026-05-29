---
type: craft-export
title: "2024-10-09 etched nonlinear device ansys field simulation"
craft_document_id: 3F751882-D91D-44AF-9CBF-99F4626669CC
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-10-09 etched nonlinear device ansys field simulation
Below is the device before I put the ITO electrodes ontop

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/D922936E-2447-4A9C-9FB7-45B6091D8A57_2/QVynOsuAUOuyXxuqyRgR35QZ7NlE8wEnGTkb4zlclc8z/Image.png)

I assumed conformal deposition for TEOS and directional deposition for SRN (though I don’t think the distinction matters much).

Now with ITO electrodes ontop (as we can’t see the bright and dark state now)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/64CF2412-EC13-4100-81B7-7AD5719001C6_2/57f6PIL4qK6796CW30YFqvO1IhZzVj9IZuuM3BjWcIgz/Image.png)

I now applied symettries and put ground and high voltage plane on

With everything as complete capacitor in DC

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/2F4108B0-B69F-47B7-8572-06CE99BBB374_2/xxHIaYA8itg7QMyDPtFUk4TaEmIrTikK1Gt2awc9PNEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/94D298E6-AC34-4C9D-B18A-230FBCFBB98F_2/z4913iRfFFypfuGPhXkl3SMvZ6SyscEtFpxg8DiEquoz/Image.png)

This is to be expected.  Now lets get some bisection lines in each of these planes and try to see what the fields look like for different frequencies

We seem to be stuck in place where I can’t get the region between total capacitcence and resistance. 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/7BAB8494-BA83-4804-8FA7-70D3BC84DC88_2/eWbnmjKuzJAfetqp7nZLTdNTbuAyc5Ilzpu7kV7BpoAz/Image.png)

I am going to raise the SRN conductivity.  Below are the plots to reference:

![Screenshot 2024-07-28 at 3.18.55 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/c120ae1b-a1e9-9c63-8ed4-76f6dba94f5b/dPf9SGWy2Ni7oY22we5s8bx8FwAopvDZnDqAWsEXomwz/Screenshot%202024-07-28%20at%203.18.55PM.png)

![Screenshot 2024-07-28 at 3.19.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/52e9b13a-605e-69b1-368a-cc7152fd65e0/kkHDAGyyl8kiuPtMoJmMWOZETb6y6Bnatp9SB8Ucm74z/Screenshot%202024-07-28%20at%203.19.05PM.png)

Ryo uses SRN 8.  I am going to guess dark state is 1e-9 and bright state is 1e-6

Next, I am going to say SiNx waveguide is 1e-17 and SiO2 is 1e-19

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/EF1F0013-BABB-4D6F-A21B-2D3555442E4A_2/6qiSx8eRSLj5RRq1qBxpEFXz6XmYW6RR2eYhxhIzEXgz/Image.png)

This seemed to help, but an interesting effect is that higher freuqnecy is lower on the dense section and lower frequency is higher (though DC at bottom is still useless).  I will start scan lower

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/19AEDF46-3596-40CA-ABB9-9FCD4EE89379_2/OVfn1aDcmOt4tQIBY7c5EVAKTKEy7DLxAfbXwfQ1xr8z/Image.png)

It turns out that lower really was not nessesary.  It is a bit annoying that I can’t access the very lower freuqnecies, as there must be a point when the thin moves from DC to AC

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/5FF68A6A-792A-4DCA-A933-B8CF95E5E2DC_2/7Wx7xGWg1COyfH6QD1wjJRBkULbVyzGgpkXD5DS5LXYz/Image.png)

Still impossible to resolve.  At this point, I say we do a 50 point sweep from 0 to 50 (Step size is 1).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/D3299C80-701A-43D8-BA37-6CFD40E3A89A_2/MzS4yIbxYmYfrrf2cHxbmOzWtYGOcXs5xlZe5Ms322oz/Image.png)

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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/98B2EF67-5822-4F65-B069-AA571CF347A6_2/nxEdC13Qc69egR5vox3K5xLzzcmqQy7H4yCk1I2T2iIz/Image.png)

A quick feuqnecy dependance for the base device is below:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/07ABA203-C883-40DE-95E0-E1A47197BE0F_2/PWVTiSD80zjWwy74gx4yJSGJXWbxC1ghNbClBpSPPiYz/Image.png)

Take this with a heavy grain of salt, as I really did not probe musch below the lowest frequency shown above

All of my results are below (Take them with a pinch of salt, as these are qualitative measures of performance)

Middle TEOS

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/4F428232-E3DD-4F63-A94F-01B0C577C45B_2/KkR6YMbHtjcslHxhxcdLs6qxty1kIhlI5bVySILoe98z/Image.png)

Middle SRN Thickness

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/D18226AA-83E7-49AC-8B5A-8BF5D93CEC37_2/jarYQKyKFnXxtK7nPgqDHwgPIIoB3pzlNqJXDRMXkpsz/Image.png)

Middle Pad Oxide:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/53CA798E-ECA7-481F-9A4D-192AD8DB632B_2/bsLkQAaAxSmAizrRfnIsrCJpRkP2vyeUE2C53rr5iG4z/Image.png)

Sidewall Height Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F751882-D91D-44AF-9CBF-99F4626669CC/25C766CA-97B7-4B23-ADFF-AF85351C07E6_2/oxQrpfXWIfOyX5W3WDL5VxGIJYXwyPpqZSNwFYta7Xoz/Image.png)

This is not all of the data, but it is good enough to understand the general idea.  My conclusions are as follows:

1. A deeper sidewall moves you get more fields into the core for the same applied voltage.  The net contrast seems to remain the same.
2. The thinner your pad oxide, the better
3. It is unclear if a thicker SRN matters a tonne, but it definately reduces the magnitude of field.  The contrast seems to be the same.
4. The thinner your TEOS, the better