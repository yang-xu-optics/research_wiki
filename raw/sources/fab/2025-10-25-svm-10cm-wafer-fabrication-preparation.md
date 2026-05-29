---
type: craft-export
title: "2025-10-25 svm 10cm wafer fabrication preparation"
craft_document_id: 2C998262-A302-4551-A135-EBED0CEF2E82
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-10-25 svm 10cm wafer fabrication preparation
While SRN3 has lower propagation loss, we know SVM has higher conversion efficiency because it has more Si.  We would like to get an SVM wafer ready such that we can test higher conversion efficiencies on it.  

We will put oxide on SVM wafers (which will be used as a hard mask).  We will do this for two wafers just in case something happens to the first.  In the past, we followed this proceedure: [https://tdwg.craft.me/idzUWVVxdYBYsl](https://tdwg.craft.me/idzUWVVxdYBYsl).  We will use 6:35 as the oxide deposition time.

The first part below as done on 9-28

During RCA

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-001.jpeg)

### PECVD Cap Deposition

We run 8 min pre clean, and will run 1 minute season after.

Before 1 min season

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-002.jpeg)

Before first dep

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-003.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-004.jpeg)

Ellipsometery of first

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-006.jpeg)

SiN is a bit thicker than I remember, but Pecvd is good

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-007.jpeg)

First is 800 nm SRN3. Back two are today’s SVM

### Remaining Plan

This part was picked back up on October 25.  The Oxford 100 was down for a whlie, so we were not able to get doing on this for a month.  How clean the top oxide is does not really matter, but we can do a quick spin clean just to be sure.  Below is the process we are going to follow to pattern a wafer (and we only need to make one.  Nice to have the other in reserve in case something strange happens).  We currently have 1um of bottom oxide, 2.1 um of SVM (suppose to be 2um, but I guess they were generous), and 1.1 um of top oxide.  Obviously fits with this much film are not perfect, but it gives us a starting point.

1. Spin coat ARC on gamma (recipe 1002) and 800 nm of DUV resist (recipe 1206)
2. Expose in ASML using defocus of zero and dose of 18.  Do edge clear first
3. Develop in gamma using recipe 2010
4. Descum in Oxford 81/82 for 1:20
5. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe (it seems we raised this time slightly from 7-1 to the 7-30 deposition)
6. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
7. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
8. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition
9. Thin top cap oxide (while preserving thick side oxide) using CHF3/O2 etch recipe.  Run this recipe for 9:30.
10. Cleave wafer (so the bulk SiN parts are as sliced up as possible)
11. Run RTA at 800 C for 5 mins.  I would ramp at 5 C/s.  Hopefully this will help prevent explosion
12. Deposit SRN8 for 48 mins to get 3 um.  Do this 4 times to get 12 um of photoconductor with 25 minute cleans and 1 minute seasons between.
13. Sputter ~35 nm of ITO (including the material sputtered beforethe shutter is fully opened). Be extra sure not to put electrode over any exploded SRN.
14. Cleave facets at this point and potentially polish facets.  If possible, try not to leave too much propagative room after the end of the poling region.

From intuition, given the losses of SVM, I doubt anything longer than 10cm will be useful.  Given the plateauing effect of SHG power near the peak, I don’t think 10cm will be that destrictive.  I think we sohuld just expose the 5um and 6um 10cm long spirals.  I think the poling condition for SVM will bias towards 6um, but we will see.

Below is the distribution of our images

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-008.jpeg)

I accidentally overwrote the old job.  We should probably shoot an Si wafer beforehand just to check

Double check that we have right wafer

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-009.jpeg)

We will spin clean and get started 

## Photolithography

Before ARC

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-010.jpeg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-011.jpeg)

During edge clear

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-012.jpeg)

During main

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-014.jpeg)

Before developing 

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-015.jpeg)

After exposure 

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-016.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-018.jpeg)

## Etching

We do 5 minute pre clean on 81 and 100

Before season on 100

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-019.jpeg)

Before descum

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-020.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-021.jpeg)

Before oxide etch

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-022.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-023.jpeg)

We run 8 minute clean

Ellipsometer

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-025.jpeg)

During eco clean

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-026.jpeg)

Before season

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-027.jpeg)

Before piranha

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-028.jpeg)

We have a lot more oxide than we expected.  Lets do 6 mins nitride etch.

Before nitride etch

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-029.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-030.jpeg)

we run 13 minute clean

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-031.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-033.jpeg)

We now run piranha clean



## Top Cap Deposition and Thinning

We start 10 minute clean of PECVD

Before season 1

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-034.jpeg)

We are going to skip BOE dip

Before first dep

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-035.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-036.jpeg)

Before season 2

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-037.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-038.jpeg)

During second dep

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-039.jpeg)

Before thinning season

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-040.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-041.jpeg)

After deposition

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-042.jpeg)

We know this recipe etches at 168 nm per min.  We want to get rid of 1800 nm.  So I say we etch for 11 mins, and slightly over etch (as we do have slightly too much to oxide anyway

Before etching

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-043.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-044.jpeg)

We aer going to jump at **10.5**, I think 11 is a bit much.  Afterall, we know we really only need a minute extra of etching.  Besides, given the time and cost of making this wafer, lets do it right

After

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-045.jpeg)

Ya, probably needed the extra time lol. Either way, I don’t think this makes a tremendous difference. Given the risk of radiative losses anyway, this is probably fine for longer waveguides 

Now we run RTA.  We do 5 mins at 800 C.  Lets ramp at 5 C/s, just in the hope that this somehow reduced film explosion.  We will cleave first, and then we will spin clean after RTA.  Lets hope cleaving goes well, as that is the hardest step to control.  Technically, we should test loss before doing marathon PECVD depositions, but I just don’t think I see any reason this won’t work.  We are going for 12um, as a reminder, so 4 runs of 3um each. 

Our recipe

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-046.jpeg)

After calibration

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-047.jpeg)

We are going two at a time. During first two

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-048.jpeg)

During second two

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-049.jpeg)

Small dip and then recovers

After spin cleaning

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-050.jpeg)

Minimal explosions compared to before 

## SRN deposition

Before season 1

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-051.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-052.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-053.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-054.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-055.jpeg)

Fit is a bit bs, but we got the right amount of film

We now clean for 25 mins

Before season 2

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-056.jpeg)

Before dep 2

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-057.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-058.jpeg)

We are now resuming on the following day, so we get a 5 minute clean going.

Before season 3

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-059.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-060.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-061.jpeg)

We now run 24 minute clean (we will keep ramping this down lol). In future, we do 25 min clean

Before season 4

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-062.jpeg)

Before dep 4

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-063.jpeg)

During dep 4

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-064.jpeg)

Before loading for Ito

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-065.jpeg)

Before ITO

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-066.jpeg)

At end of Ito 

We started normal sputter with almost 10 nm. Will stop a bit under 35

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-067.jpeg)

At very end

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-068.jpeg)

At very very end

![Photo from Library.jpeg](../../assets/fab/2025-10-25-svm-10cm-wafer-fabrication-preparation-069.jpeg)