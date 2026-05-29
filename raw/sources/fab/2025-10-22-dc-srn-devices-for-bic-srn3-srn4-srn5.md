---
type: craft-export
title: "2025-10-22 dc srn devices for bic srn3, srn4, srn5"
craft_document_id: 0AF0C8B1-DA6A-433B-8735-00B088C914B6
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2025-10-22 dc srn devices for bic srn3, srn4, srn5
We are interested in making new DC devices for BIC, with my design note here: [https://tdwg.craft.me/dPebxM2j0fb4ZQ](https://tdwg.craft.me/dPebxM2j0fb4ZQ).  We hope for devices with slightly higher delta_n than the existing one, and we are basically trying to see if the low-Si, or high-Si approaches are better.  

## High Level DON recalibration

We know our starting recipe for DON is 

Temp: 350 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 475 sccms

Power: 10W

N2O flow: 250 sccms

Lets do a quick deposition of this film and see what we get.  Will do 3 mins.  I don’t think seasoning is nessesary

Before deposition 

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-001.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-002.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-003.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-004.jpeg)

We got no film, which is weird 

When I look after, the chip does seem to have nothing, even though the carrier wafer has somthing.  Lets perhaps just check the SiN recipe real fast.

Before dep (no clean or season in between)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-005.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-006.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-007.jpeg)

You can see where the oxide was

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-009.jpeg)

ok, we know that works.  Lets do oxide again, but perhaps make the N20 160 scccms

Before dep (Again, no cleaning or seasoning quite yet)

I realized I set N20 incorrectly before hand.  I set O2 by accident instead

Try again

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-010.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-012.jpeg)

There is plasma, it is just hard to see

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-015.jpeg)

Good, we got something.  Now we just want the index to be 0.05 higher, so lets run with 200 sccms

Before 

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-016.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-017.jpeg)

Technically the plate is heating up a bit, so index might be slightly low

Temp seems to drop a bit

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-018.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-020.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-021.jpeg)

Let’s make it 175 now

Before

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-022.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-023.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-025.jpeg)



So we know 175 sccms is 1.845, 250 is 1.74.  So the average is 215, but we found that 200 gave 1.79.  I think that 200 one was a bit off because of temurature though.  I stay we stick wtih our guns and do 205.  We have more flexibity here than we realize.  

I am doing a 10 min post clean, and I will put a witness sample in for characterization purposes during the season.

Before test

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-026.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-027.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-028.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-029.jpeg)

We should probably use 215 or 210 for SRN3, and we can call quits there. Either way, we are very close.  It does seem we were a bit hurt earlier by the low dep temp

For SRN4, we want an index of 1.89.  So lets try 140 sccms of N2O for that

Before 140

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-030.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-031.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-033.jpeg)

We want an index of 1.89 for SRN 4 device, so this is a bit high.  175 sccms gives 1.845.  140 sccms gives 1.935.  We roughly want to be in the middle, so 155 sccms seems right.  I think 110 is going to be best for SRN5

Before

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-034.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-035.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-037.jpeg)

Perfect!!

Now, last but not least, 110

Before

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-038.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-039.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-040.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-041.jpeg)

Lets plot our results, ignoring the one weird low-temp film.

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-042.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-043.png)

## Device Design Confirmation

Below are the indexes we are shooting for with the anticipated N2O flow.

SRN3, 1.8 → N2O flow of 205 sccms

SRN4, 1.89 → N2O flow of 155 sccms

SRN5, 1.98 → N2O flow of 125 sccms

I don’t have an exact film for the last one, but for the others, we have the simulations below (with our understood core index)

SRN3 

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-044.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-045.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-046.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-047.png)

Only have 2 modes.  Length of tails tells me we have nothing to worry about.  This looks good to me!!!

3um bottom cladding (dep time of 44.5 mins) 32 minute clean

2um of SRN3 core (dep time of 65 mins) 23 minute clean

1.5um top cladding (22.5 mins) 18 minute clean

205 mins of deposition and clean.  We probs have 30 more mins of bs, so basically 4 hours to get this done



SRN4

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-048.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-049.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-050.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-051.png)

Only 2 modes, and again, I suspect the 2nd one will have a lot of substrate loss.

3um bottom cladding (dep time of 46 mins) 32 minute clean

2um of SRN4 core (dep time of 48 mins assuming rate of 41.6 nm/min) 23 minute clean

1.5um top cladding (23 mins) 18 minute clean

N2O flow is 155.  We will probably reduce N2O flow to 150, as higher inedx is generally better..  We will increase bottom clad dep time to 50 mins.

SRN5

I will simulate the mode shapes later once I know the exact index.  Eitherway, I can surmise the approximate deposition times below

2um bottom cladding (dep time of 31.5 mins) 23 minute clean

2um of SRN5 core (dep time of 44 mins assuming rate of 45 nm/min) 23 minute clean

1.5um top cladding (16 mins) 10 minute clean

Below are the confirmed stats after testing out the DON recipe

![Screenshot 2025-10-31 at 2.23.11 PM.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-052.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-053.png)

![Image.png](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-054.png)

## SRN3 Device Fab

We start 10 minute clean on PECVD.  We RCA cleaned wafer yesterday, so we should be fine.  Everything will be full wafer processing.

Before bottom clad season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-055.jpeg)

Before main deposition

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-056.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-057.jpeg)

We use carrier wafer for everything just to be consistent.  Came out ok.  I am now startined 34 minute clean

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-058.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-059.jpeg)

Index is a touch low, but not a huge deal

Before SiN season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-060.jpeg)

Before deposition

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-061.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-062.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-063.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-064.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-065.jpeg)

Looks good to me

Season before top cladding

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-066.jpeg)

We now do 23 mins of DON205

Before deposition 

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-067.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-068.jpeg)

Wafer is stored below

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-069.jpeg)

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-070.jpeg)

Index fits are bs, but I trust thickness more

## SRN5 Device Fab

We are RCA cleaning the next two wafers a day or two in advance.  This should be good enough (considering it is what we did above).

We are doing a 5 min pre clean, and we use N2O flow of 125 sccms.  We will test that the index looks ok after a 2 minute season on a witness sample

Before test season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-071.jpeg)

After season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-072.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-073.jpeg)

Deposits at 63.5 nm/min.  So for 2um, we want 32 mins.

Before main dep

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-074.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-075.jpeg)

We now do 20 minute clean

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-076.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-077.jpeg)

The trials and tribulations of getting consistency.  We will do a 45 minute deposition for SRN5 next

Before 5 season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-078.jpeg)

Before main dep

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-079.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-080.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-081.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-082.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-083.jpeg)

Before top season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-084.jpeg)

We want 1.5 um.  We deposited for 32 minutes to get 2um, so now we do 24 mins

Before main

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-085.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-086.jpeg)

## SRN4 Device Fab

I am running a 5 minute preclean

We will do 150 N2O.  We will do 50 mins deposition.  We RCA cleaned a week ago, but it is probably fine.

Before bot clad season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-087.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-088.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-089.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-090.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-091.jpeg)

Next day we come back for the SRN4 layer.  We run a 5 min preclean, and we will also do a quick check on the index of SRN4 after the season

Before 4 season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-092.jpeg)

We deposited an AR coating. Either way, we should be fine to continue. Dep for 65 mins

Before main dep

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-093.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-094.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-095.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-096.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-097.jpeg)

I will season for a minute using the DON recipe. I will dep for 23.5 mins

Before season

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-098.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-099.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-22-dc-srn-devices-for-bic-srn3-srn4-srn5-100.jpeg)