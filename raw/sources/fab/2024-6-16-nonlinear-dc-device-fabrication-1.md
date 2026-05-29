---
type: craft-export
title: "2024-6-16 nonlinear dc device fabrication 1"
craft_document_id: D4B79F0D-E4FA-46D1-A865-90790BC20B96
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-6-16 nonlinear dc device fabrication 1
The purpose of this document is to detaily my first Nonlinear DC Device fabricaiton.  Below are two design documents that help understand the device

[Nonlinear Waveguide DC Design (1e-12).pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/8ACD3252-9FB6-468B-B292-0CE6337B5FCF_2/PZ3YyxlH219ssQPBxMCV3AxZMwGcNlCeZYG1zUxVTbYz/Nonlinear%20Waveguide%20DC%20Design%201e-12.pdf)

[Nonlinear Waveguide DC Design (1e-11).pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F2CAADE5-3AFA-4C51-900C-3F1DDBFAC66D_2/XNxTaYeJBw3fFxhx7Cjg6ltyPdF2rqXrzg10rwzFGfQz/Nonlinear%20Waveguide%20DC%20Design%201e-11.pdf)

These are guesses at the conductivity of the SRN layers.  I ended up deciding that the SRNs probably have nearly constant conductivity in the high field, as that is what Ryo’s data seems to show.  At the very minimum, these seem like genuinly good results.  I am going to keep the claddings thick just in case of substrate loss for low index contrast and, if the core’s have some dependance on field for conductivity, it would be useful to compensate for that.  

I am going to deposit 3um of the following film:

B8:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 475 sccms

Power: 10W

N2O flow: 160 sccms

It is kinda silly, looking at the deposition code and the fact that I made this recipe 2 months ago, that I spent 2 extra months refining recipes to not learn a lot for the nonlinear device.  These simulations are quite helpful it seems.  FWIW, my refined reicpes (B12 basically) is the future for linear devices (or honestly even something done at 350 degrees).  It did not help that I was believing constant conductivity to be possible, when exponential conductivity is the reality.  The nice thing about the above recipe is that they will also have high breakdown.  

I am going to do 1 min season before hand, stop deposition at 1.5um clean, season, deposit (plus a 10 min anneal in-chamber at 350) and clean.  The previous dep rate we found was 62.2 nm/min.  This means we want to deposit for 48 mins.  We will do two depositions for 24 mins.  I will clean for 25 mins as well.

The Si wafer

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-001.jpeg)

Before season 1

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-002.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-003.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-004.jpeg)

Before dep 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-005.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-006.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-007.jpeg)

I think, for the conductivity pad, I will do a 350 C anneal. I will use RTA for that. I will do it for five mins and ramp at 5 C/s 

Before annealing

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-009.jpeg)

Calibration run of RTA

Temp sensor is a bit weird 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-010.jpeg)

Honestly, I don’t really care, as we just want calibration 

During anneal

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-011.jpeg)

Ellipsometee after annealing

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-012.jpeg)

To be honest, that feels excessive, based on previous measurements. I think the temp probe is just broken, so we will analyze this again later. I was also applying a shit ton of energy, so that might have been an issue too

Side quest, conducitivity characterization 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-013.jpeg)

From left to right, B22, B8, B21

Life is good

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-014.jpeg)

For Ti

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-015.jpeg)

The gate is closed, so I will just kinda get a bit of Gold onto my samples and call it quits 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-016.jpeg)

Jeremy thinks we should be fine to anneal in the chamber (though he recommends Yes oven for the future).  I would say 15 mins at 375 would be ideal, as I am worried about any outgassing.  

Earlier index results for similar anneals

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-017.png)

I would expect index to go up by 0.01, which is totally fine.  Jeremy says we will notice the difference when we see outgassing.  It is not hard to observe.

Before season 2

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-018.jpeg)

During first season

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-020.jpeg)

What anneal should look like

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-021.jpeg)

Before rep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-023.jpeg)

Let’s hope this works

During dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-025.jpeg)

Anneal started at low temp

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-026.jpeg)

I should still get ~10 mins of high temp, which is fine 

This is when we arrived at 375

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-027.jpeg)

Was above 350 for 10 mins tho 

Ellipsomtery (tough to get good fit)

1550 fit

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-028.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-029.jpeg)

Another possible that seems more legit

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-031.jpeg)

780 fit (not possible)



It is a bummer that these fits did not work, nonetheless, below are the indexes of not annealed to 3.5 core

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-032.png)

At 1550, our gap is 0.05, and at 780, the gap is 0.03.  Not small gaps, but not huge either.  Put simply, we should next expect the index to go up by that much.  I also have futher evidence that we over annealed in RTA because I can see some stress issues at the edges of my films.  While it is concerning that I don’t know the exact indexes, I am not panicked either.

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-033.png)

Loss (as shown above) should be managable too

Below is what Ryo’s screen looked like for SRN dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-034.jpeg)

His dep rate was 38.25.  Pretty decent.  This means, to get a 2.5 um film, I want at least 66 mins of dep.  I say we do two 33 mins dep, with 1 min seasons, and 35 min cleans.  I will also do a 10 min extra anneal before first dep just to make sure stuff works.  

Before season 1

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-035.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-037.jpeg)

I am going to deposit on three of my six cleaved pieces and do 10 min anneal

Before depositing 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-039.jpeg)

During anneal

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-040.jpeg)

During dep 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-042.jpeg)

After dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-043.jpeg)

No evidence of out gasing 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-044.jpeg)

Left side of box. My dumbass forgot a witness sample, but I will add it in next. Plasma was on, so we def got something

Before season 2

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-045.jpeg)

During season 2

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-046.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-047.jpeg)

In the future, click the pump to pressure button if the pump step stalls

Film on right is Si witness

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-048.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-049.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-050.jpeg)

No annealing

During dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-051.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-052.jpeg)

Ellipsometry on witness 

Short range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-053.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-054.jpeg)

Long range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-055.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-056.jpeg)

Retake of substrate

Ultra short range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-057.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-058.jpeg)

Short range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-059.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-060.jpeg)

Long range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-061.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-062.jpeg)

We can def see that k is higher here. 

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-063.jpeg)

Left side has SRN

Index of SRN looks very similar to before (maybe a bit lower).  But our characterization seems to indicate that the indexes should be ok.  We will confirm tmrw in the lab

Below are the characterized losses

1550

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-064.png)

1064

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-065.png)

780

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-066.png)

Before top cladding season 1

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-067.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-068.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-069.jpeg)

During deposition 1 top cladding

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-070.jpeg)

Witness on right

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-071.jpeg)

During dep 1

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-072.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-073.jpeg)

After dep 1

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-074.jpeg)

No evidence of cracking or anything like that

Ellipsometer

Short range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-075.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-076.jpeg)

Long range

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-077.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-078.jpeg)

Before season 2

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-079.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-080.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-081.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-082.jpeg)

During second dep

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-083.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-084.jpeg)

Tapes pieces

![Photo from Library.jpeg](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-085.jpeg)

Top is device, right SRN, left DON

Side note: Ryo’s direction 1 is the shorter propagation distance

Full stack at 780

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-086.png)

Keep in mind, the light had to travel 2cm in my device, so the fact that we saturated is not a huge deal

Ryo stack (short direction at 780)

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-087.png)

Ryo stack (long direction at 780)

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-088.png)

Ryo Stack (short direction for 1550)

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-089.png)

Ryo stack (long direction for 1550)

![Image.png](../../assets/fab/2024-6-16-nonlinear-dc-device-fabrication-1-090.png)

So my stack is probably 2-3 dB/cm at 780, which is much lower than I expected.  The only weird thing I find about Ryo’s stack is that he has a grating structure

