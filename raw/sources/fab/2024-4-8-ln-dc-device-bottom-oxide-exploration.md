---
type: craft-export
title: "2024-4-8 ln dc device bottom oxide exploration"
craft_document_id: 1E788CFD-48E9-4B57-874F-1D2CBD3F7086
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-4-8 ln dc device bottom oxide exploration
Given my simulation results today, I am interested in developing as conductive of an oxide as possible.  This film must have an index at 1550 below 2.2 (to be a useful cladding for LN).  We also need low optical loss.  



As a summary of out previous results, we found that B6 (N2O = 110 and power = 5W) had a conductivity of around 1e-7 and index of ~2.05.  While my fabrication technique (3 intervals) was stupid for the optical loss measurement, my B7 results do make me susepct this really did have onerous loss.  B7 (N2O = 135 and power = 5W) had a loss of 5 dB/cm and an index of ~1.94.  No conductivity data.  This loss makes be suspect that having oxygen concentrations below this might be a problem.  Given the trend (minus the B4 outlier) I suspect this film have a conductivity of ~1e-8.  This is already fairly close to where we want to be.  This makes me a bit nervous.  B8 (N2O = 160 and power = 10), I saw really low loss of 1 dB/cm, but I was not able to take conductivity data.  Index data was also hard to get.  The higher power might have screwed up my conductivity, but we had great loss.  I think, given the lower loss that the high power film achieve, we should try B6 and B7 with power = 10.  I think B7 is the upper bound of 5W perfomance regardless because the gas becomes hard to light above that.  Maybe we can try small scans of power and N2O flow in the future, but I would prefer not to do that if possible.  We can also take smaller N2O jumps in the future as well.



Given the conclusion above to stay within the B6 → B8 N2O range (because of conductivity concerns), B9 is probably overkill.  I want to use 10W because of loss concerns.  I might also want to anneal at a low temp (800 already broke my films so below that) in case I want an extra degree of freedom in the future.  Below are the recipes:



Recipe B6*:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 110 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Recipe B7*:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 135 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Recipe B8:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 160 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Ryo said he was able to see good signal with chips that were 1.5 um thick and 1e-9 and 1e-10 cond.  Because I want waveguides (these are also slightly higher index), I probably want to deposit B6* and B7* for 20 mins on thermal and vanilla.  B8, because I already have it on thermal and have characterized it (those wafers are also in short supply), I will just do 5 mins on vanilla to measure conductivity.  So 3 quarters vanilla and 2 quarters thermal are needed.  Check wafer boxes to see if there are any bare vanilla or thermal quarters floating around.

Below is characterization of vanilla silicon wafer

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-001.jpeg)

And for oxide

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-002.jpeg)

We spin cleaned the quarter wafers and are doing a 5 min preclean on the PECVD because the carrier wafer was left out.

Below are the boxes the samples are stored in

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-003.jpeg)

We are going to do B8 first, so we can do ellipsometry during the last longer clean.

Here is the recipe before we get started

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-004.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-006.jpeg)

The gas is lit and everything is within parameters, so I say we should be good to do real deposition for 5 mins

Blue color we are used to

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-007.jpeg)

During the actual deposition 

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-009.jpeg)

After deposition 

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-010.jpeg)

The orange color is a bit new. Before we had purple. Probably higher power causing this more than more oxygen

After  B6* seasoning (forgot to take picture during)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-011.jpeg)

Normal blue we are used to. I am going to put oxide wafer on left and vanilla wafer on right

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-012.jpeg)

Screen before dep

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-013.jpeg)

20 min dep starting. During dep:

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-015.jpeg)

After deposition 

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-016.jpeg)

Uniformity is really good. 25 min clean is now running

Before B7* season:

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-017.jpeg)

During season:

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-018.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-019.jpeg)

After season

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-020.jpeg)

Nice and blue. Let’s do 20 min dep. once more vanilla on the right

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-021.jpeg)

During dep:

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-023.jpeg)

After dep:

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-024.jpeg)

Now time for some ellipsometry:

B8

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-025.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-026.jpeg)

B7*

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-028.jpeg)

Only a small hiccup at 45

B6*

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-030.jpeg)

Now onto the even-hour evaporator, where we will deposit 10 nm of ti and 5 nm of au.  The indexes above are about 0.05 less than their 5W equivalent, so power does not seem be have a huge effect on what compounds are in the film.  My worry is still might not be conductive.

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-031.jpeg)

B6 is top left, B7 is top right, B8 is bottom middle 

After taping

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-032.jpeg)

They did not seem to have the small tapes available unfortunately 

Life is ok

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-033.jpeg)

Samples are in

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-034.jpeg)

Our pressure is low enough that we are good to go

The Ti seems to have a somewhat stocastic dep rate. But it is coming so I say we continue

Seems to be between 1 and 1.2 A/s. Power is also 10 for Ti, which is a bit high

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-035.jpeg)

Now for au

![Photo from Library.jpeg](../../assets/fab/2024-4-8-ln-dc-device-bottom-oxide-exploration-036.jpeg)

Gold had a normal power and the electrodes look fine to me.  We will see sheet resistance when we get into the lab.   Everything is unpacked and ready to be tested!!

