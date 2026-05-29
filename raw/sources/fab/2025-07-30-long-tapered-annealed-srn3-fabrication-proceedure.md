---
type: craft-export
title: "2025-07-30 long tapered annealed srn3 fabrication proceedure"
craft_document_id: 6038A08D-2D03-4A1D-A6B7-982B8F08DC0C
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-07-30 long tapered annealed srn3 fabrication proceedure
Winter is coming.  It seems we have finally gotten to the point where we can make 10cm spirals!  We are going to exactly copy the proceedure shown here for one wafer: [https://tdwg.craft.me/fqaECr3nRcY0Bj](https://tdwg.craft.me/fqaECr3nRcY0Bj).  When we measured the stress on the SRN3 wafers we deposited here: [https://tdwg.craft.me/idzUWVVxdYBYsl](https://tdwg.craft.me/idzUWVVxdYBYsl), it seems to be neutral.  We can check the stress again and do another 3 minute, 400 C RTA if needed.  That seemed to work in the past.  I suspect that stress is some type of transient thing.  

The one thing we might want to change is whether we put a cap oxide onto the wafer or not.  The reason to put a cap oxide onto the wafer is we know that process works and a warped wafer might not be good in the 100.  There could be He leakage and bad cooling.  In theory, this would only effect the oxide, but still.  The reason to do this is it might allow the SiN to reflow and outgass better, further reducing loss.  The Lipson guy also made it sound like this is the better approuch.  At the very minimum, we should put a thermal oxide wafer into the furnace anneal just to see if it warps, as it would be nice to know whether this is going to be a common problem in the future.

Below is the proceedure we are going to follow (I list it out for easy reference in the future, including the SRN3 deposition steps):

1. RCA clean of 1um thick SiO2 wafer
2. Deposition of SRN3 for 65 minutes.  This gives 2um
3. Deposition of top cap oxide using smooth recipe for 6:35 mins.  This gives 1100 nm of film
4. If needed to account for wafer bow, 3 minutes RTA at 400 C
5. Spin coat ARC on gamma (recipe 1002) and 800 nm of DUV resist (recipe 1206)
6. Expose in ASML using defocus of zero and dose of 18.  Do edge clear first
7. Develop in gamma using recipe 2010
8. Descum in Oxford 81/82 for 1:20
9. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe
10. Run 5 minutes in YES ecoclean and then run piranha clean
11. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
12. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
13. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition
14. Thin top cap oxide (while preserving thick side oxide) using CHF3/O2 etch recipe.  Run this recipe for 9:30.
15. Perform RCA clean, and then anneal in 1200 C B2 tube for 5 hours in Argon.  Load at 300C, ramp for 2 hours, and cool over night.
16. Once annealing is done, cleave chips into their respective rows
17. Deposit SRN8 for 32 mins to get 2 um.  Do this 4 times to get 8 um of photoconductor with 19 minute cleans and 1 minute seasons between.
18. Sputter ~30 nm of ITO (including the material sputtered beforethe shutter is fully opened.  Cleave facets at this point and potentially polish facets

### Lithography

Stress before

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-001.jpeg)

Good there

Ellipsometer 

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-002.jpeg)

Other wafer

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-003.jpeg)

Before arc

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-004.jpeg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-005.jpeg)

Before edge clear

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-006.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-007.jpeg)

During each wafer

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-009.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-010.jpeg)

During each wafer

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-012.jpeg)

Before developing

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-013.jpeg)

### Etching

We start 5 min pre clean on 82 and 10 min clean on 100

Before descum

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-014.jpeg)

Before oxide season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-015.jpeg)

During etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-016.jpeg)

He flow is a bit high, but not catastrophically high. 8 or 9 is where I worry.  Lets see if the main wafer has this issue.  

Before oxide etch on wafer 1

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-017.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-018.jpeg)

He flow is good again

Lets now run an 8 minute clean

Before Ecoclean

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-019.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-020.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-022.jpeg)

Microscope

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-024.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-025.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-026.jpeg)

We now run piranha clean

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-027.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-028.jpeg)

Before second etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-029.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-030.jpeg)

Run 10 min clean

During eco clean

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-031.jpeg)

We now run piranha clean

Before nitride season on 1

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-032.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-033.jpeg)

Before nitride etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-034.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-035.jpeg)

My wafer got stuck in the tool after this, so I have to stop the process here.  It does not seem that it will be damaged by being left in an inert chamber, however.  Roughly 24 hours later, we resume.  Start 8 minute pre clean on chamber

we pirnaha clean the second wafer again.  After etch data below

We over etch a bit

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-036.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-037.jpeg)

Let’s do 5:20 next time. We are running piranha on water now and will move to BOE soon

BOE is done. We now piranha again

During second nitride season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-038.jpeg)

He is high. Hopefully it is just bad mounting. 

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-039.jpeg)

During 

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-040.jpeg)

A bit later

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-041.jpeg)

We now run piranha

BOE is done too. After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-043.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-044.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-045.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-046.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-047.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-048.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-049.jpeg)

Piranha again and we are good 

### Top Capping

We start 10 minute season on the PECVD

Before first season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-050.jpeg)

Before first dep

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-051.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-052.jpeg)

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-053.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-054.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-055.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-056.jpeg)

We now want to etch to 1800 nm, so we want to get rid of 1600 nm

Before 100 season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-057.jpeg)

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-058.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-059.jpeg)

I am not in love with this He flow, but this step is less critical. Also, I don’t have 8, so evidently there is some seal

After, we got it spot on

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-060.jpeg)

Before first season wafer 2

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-061.jpeg)

Before first dep

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-062.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-063.jpeg)

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-064.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-065.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-066.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-067.jpeg)

100 season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-068.jpeg)

Before etch

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-069.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-070.jpeg)

Did not etch as deep, but we also had more oxide left

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-071.jpeg)

### Annealing

While I don’t think it would be a useless test to do something without top cap, given the uncertainty around warping, I am going to put top cap on both wafers and etch both.  I will throw a thermal oxide wafer into the anneal just to see what happens, and this wafer can become a carrier for ITO later.

We have our oxide wafer ready

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-072.jpeg)

During rca, we started at a lower temp

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-073.jpeg)

Anneal is ready

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-074.jpeg)

We are loading at a slightly higher temp than ideal

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-075.jpeg)

Either way, I don’t think this is an issue. These wafers can survive RTA after all 

We are ramping

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-076.jpeg)

Our Ar flow is a bit low, but so be it.

Near end

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-077.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-078.jpeg)

Ar flow seems good now

We now let it cool

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-079.jpeg)

After cool down

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-080.jpeg)

After pull out

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-081.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-082.jpeg)

Oxide has no warp. Our devices look fine.  I think most of the warp comes from the remaning SiN on the device wafers

After on wafer 1

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-083.jpeg)

Microscope

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-084.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-085.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-086.jpeg)

After cleaving, 3 very longs, 2 good widths. 



### Top electrical layers 



Before season 1

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-087.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-088.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-089.jpeg)

No plasma issues today

We can only fit 4 strips, so two of each

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-090.jpeg)

Before main 1

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-091.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-092.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-093.jpeg)

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-094.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-095.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-096.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-097.jpeg)

Before third season. 18 is probably minimum clean time too.

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-098.jpeg)

Before main

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-099.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-100.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-101.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-102.jpeg)

Before fourth season

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-103.jpeg)

Before fourth main

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-104.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-105.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-106.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-107.jpeg)

We now run 18 minute clean

Before season 5

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-108.jpeg)

Before dep 5

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-109.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-110.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-111.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-112.jpeg)

Before sputter 

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-113.jpeg)

We are pumping

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-114.jpeg)

At end of sputter

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-115.jpeg)

After cool down

![Photo from Library.jpeg](../../assets/fab/2025-07-30-long-tapered-annealed-srn3-fabrication-proceedure-116.jpeg)

Perhaps a bit more than ideal, but I don’t think this is going to matter much

