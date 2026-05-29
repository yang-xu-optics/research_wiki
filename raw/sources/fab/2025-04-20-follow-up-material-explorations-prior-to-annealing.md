---
type: craft-export
title: "2025-04-20 follow up material explorations prior to annealing"
craft_document_id: 6C9D1C56-4458-47D8-BDEC-3B7D43265757
craft_collections: [etching-sin-waveguides, fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-04-20 follow up material explorations prior to annealing
Prior annealing experiments did not seem to work.  They did not show substatially reduced losses as we had hoped.  Based on a literature review, I am hopefull that we can hew very closely to Lipson’s group’s annealing proceedure (which is 3 hrs at 1200 C in an Ar environment).  It would be great to see that we have removed NH bonds and loss at 1520.   Previously, we used 2um thick SVM waveguides and annealed them at 1100 C for 4 hours in an N2 and O2 environment.  We suspect the tempurature was not high enough.  We proved last night that we can etch pretty deep using normal photoresist, so we will do that.  This means we can use the 1200 C annealing tube.  We will likely only get one shot at this from Peter (given the cost), so we really want to pack as many material ideas in there as possible.  Another thing to note (when etching prior to annealing) is that we will need to etch ENTIRELY through any material that is not oxide to prevent any stress issues.  Additionally, I have already designed GDS files that will only protect the waveguides, so everything else will be etched away.  

As for the materials we want to put in (at a high level) are listed below:

1. SVM SiNx
2. Some slightly elevated index oxide (basically, reduce the N2O flow, but no B2H6).
3. PECVD SiNx using Ryo’s recipe with no NH3.  The hope is this will have less hydrogen.  Even better would be to try these recipes with no H2 flow either (though we may have uniformity issues there).  

SVM SiNx is obvious (we know we can buy thick wafers in bulk, which makes our lives easier).  

Elevated index oxide is simply just for us to see what the loss in the most extreme case is where we are must less likely to see NH bond losses (we are as close to an oxide as possible, which does not have loss here).  In the future, I don’t know how useful these will be in the sense that they will not be very nonlinear (and confinement will not be great either), but I want a baseline

Lastly, and the one I am most interested in, is PECVD SiNx.  The I am not sure how the SVM SiNx is deposited, so there is a chance that there is lots of NH3 in the deposition (and therefore H in the films).  Ryo’s recipes use N2 instead of NH3, so I suspect they have a lot less H.  This might give us lower total loss after annealing. So I would like to make a waveguide with SiH4 = 3 sccms and anneal that using Ryo’s baseline recipes.

Additionally, I would like to test Ryo’s recipes without flowing any H2.  He mentioned that flowing H2 helps to improve uniformity.  I would like to remove this from the recipe if possible because I susepct this will lead to less total hydrogen in the film.  This will require a bit of recipe characterization.  So there is the total possibility of four wafers in this anneal.  I will use the same etching pattern (hopefully the one I designed yesterday should it work ok with the bends).  

Before making the final wafers, I want to characterize the elevated index oxide and no H2 PECVD SiNx recipes.  For elevated index oxides, I have two options available:

1. Use some bastardized version of the high rate oxide recipe.  I did this once previously here: [https://tdwg.craft.me/Jf5QeffSGD3XqE](https://tdwg.craft.me/Jf5QeffSGD3XqE).  I was kinda bad back then, so this is not perfect, but it seems they had indexes of 1.65 around 1550 nm.  Deposition rate of around 400 nm/min, which is crazy fast.
2. Use doped oxynitride recipe, but with no boron.  I also did this once before here: [https://tdwg.craft.me/0mogTv0eyBxsRF](https://tdwg.craft.me/0mogTv0eyBxsRF).  Those were some fairly excessively low power and low N2O flow films.  They all showed higher indexes (1.88 at 1550 nm).  Depsition rate of around 30 nm/min, which is unfortunantely quite slow.

I am not sure what the advantage of each approuch is to be honest.  I suppose we could just test transmission of waveguides with similar index and thickness and use that as a baseline.  I say we shoot for an index around 1.75 at 1550nm, though lower is not exclusively worse.  While I will start by depositing stuff on Si wafers to get better index fits, I will eventually deposit on SiO2 pieces so I have waveguides.

For SiNx waveguides with no H2, lets just do a Silane of three and start on a Si quarter wafer.  We can then take mutliple ellipsometry measurements across the wafer to get a sense of variation.  Below is the recipe:

SiH4 flow = 3 sccms

N2 flow = 2000 sccms

Power = 200 W

Pressure = 1900 mTorr

Tempurature. = 350 C

For the high index oxide recipes, below is what I have in mind for the modified high rate oxide

We are also going to use the metricon to get the loss values.  I will start with a metricon measurement of SVM (as we already have a spare half wafer in the box)

I start by RCA cleaning 2 oxide wafers, so I can metricon at least 4 recipes

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-001.jpeg)

As I start the clean

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-002.jpeg)

---

### [`Fri, Apr 18`](day://2025.04.18) Metricon measurement of the bare loss of the SVM wafer

### 637 nm

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-003.jpeg)

![IMG_0612.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-004.png)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-006.jpeg)

### 1546 nm

We use oxide index of 1.44

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-007.jpeg)

Fit is good. The fundamental mode is at 127.

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-008.jpeg)

Ben got it, below is index for fund TE

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-009.jpeg)

Below are some loss fit

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-014.jpeg)

Now back to some simulation, as we are trying to design the optimal film thickness to get loss.  Below is a plot of radiative mode mode for SiNx films with different core thickness and height

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-015.png)

To put it mildly, this is not great.  This really shows we need films that are quite thick.  Below are some plots of the index at 1550 for different SiH4 flows, just to get a sense of the area we are working in

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-016.png)

It is also interesting that our index are already quite a bit lower than the SVM.  Below are the poling periods for 6um wide recipes using our previous fits for these recipes

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-017.png)

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-018.png)

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-019.png)

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-020.png)

It seems the recipe does not effect the poling period much.  An interesting point here is that even SRN3.5 is more silicon more than SVM.  I would really like to be below the 1 dB/cm loss value, as that would just make our life so much easier (in the sense that we can treat that loss value as negligable compared to material loss).  We are starting with two cleanish wafers (though they were cleaned 2 days ago, but still).  I am also going to do cut-back method with full wafer fabrication to characterie the loss of these films.  I feel like that is safer than metricon (and in some sense less destructive).

Looking above, it seems that depositing SRN 3.5 and SRN 2.8 would be the most time efficent path.  SRN 3.5 needs a core thickness of 1500 nm (at least) to have low substrate loss.  SRN 2.8 needs a core thickness of 1800 nm (at least) to have low substrate loss.  Long depositions ahead I guess.  From earlier depositions, we know SRN3.5 deposits at a rate of 38.2 nm/min.  SRN2.8 deposits at a rate of 32.2 nm/min.  So we must deposit **SRN 3.5 for 40 mins** and **SRN 2.8 for 56 mins**.  This is crazy.  

If we just want loss values, we can deposit thicker bottom oxides.  Below are plots of the radiative losses for thicker bottom oxides

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-021.png)

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-022.png)

![Image.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-023.png)

It seems that 1.75 is very safe.  We then only need 900 nm of the stuff to get working devices.  Lets do 775 nm as the base added oxide.  Given that smooth oxide deposits at 166.6 nm/min.  High rate is at 240 nm/min.  To avoid any type of loss, I feel like smooth will work better.  Lets deposit smooth oxide for 4 mins and 40 seconds per wafer.  Use 1 min season as well.  We will then do **23.5 mins of SRN3.5** and **28 mins of SRN2.8**.  This is mildly more reasonable.  I am going to leave depositions with no H2 to a later date.

Finally, we may want to attempt a hydex-type recipe.  I am still really of two minds about the best way to do this (the fast way, or the smooth way).  While I am not terribley confident of this, I feel like the smooth way is still best.  So we are in for another longish deposition.  We can also try the fast approuch if we have time and feel up to it as well.  I generally feel like the only arguement against this is that there is almost no parallelization to all of this.  Given that, I think to SiNx wafers are enough for now.  We can try hydex later.



### PECVD

I am running a 5 min pre clean of the chamber.  I will then season smooth oxide for 1 minute.  Something to keep in mind if the surface we are depositing on might not be perfectly smooth, and because our waveguides are not as tall, the mode will see the roughness a bit more.  So we will have slightly more scattering losses

Before smooth season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-024.jpeg)

Before dep 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-025.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-027.jpeg)

It seems we got the right amount

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-028.jpeg)

During dep 2

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-029.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-030.jpeg)

Before SRN 3 season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-031.jpeg)

During season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-033.jpeg)

Deposits at 34 nm per min

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-034.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-035.jpeg)

Will do an extra min accidently did 3. For 3.5, I will stick to my guns

Before dep

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-036.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-037.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-038.jpeg)

Front wafer in box is 3.5. One behind it is 2.7 (I am changing it down). 

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-040.jpeg)

Before 2.7 season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-041.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-042.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-043.jpeg)

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-044.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-045.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-046.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-047.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-048.jpeg)

Ellipsometery 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-049.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-050.jpeg)

I am skipping clean and moving to oxide dep with high rate

Before season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-051.jpeg)

I will do a 2 min oxide deposition

During season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-052.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-053.jpeg)

Before oxide on the 2.7 wafer

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-054.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-055.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-056.jpeg)

During deposition of 3.5 (same oxide wafer)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-057.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-058.jpeg)

Remember, 3.5 is in front of 2.7

### Takachi PECVD

In light of a few papers (specifically these [https://www.nature.com/articles/s41377-024-01503-4](https://www.nature.com/articles/s41377-024-01503-4), [https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.22.054027](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.22.054027)) it seems that ICP-RIE PECVD can give better results for waveguides.  So I will deposit a film with the takachi PECVD.  Below is the recipe Ryo used last (it is the nitride recipe)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-059.jpeg)

Here is the note from Ryo’s work: [https://tdwg.craft.me/SXRb1ydrxl1jwn](https://tdwg.craft.me/SXRb1ydrxl1jwn).  Based on his characterizations, I will run a 1 minute season and 9 minute deposition.  This should give me ~1um of film.

They do have other recipes

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-060.jpeg)

We might want to try the nitrogen rich one instead. I will season with it for one minute with a witness sample

Before season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-061.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-062.jpeg)

The difference with the normal recipe is less silane flow

Ellipsometer of witness

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-063.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-064.jpeg)

This is very low index. Maybe I will save this for another time 

I will go back to original plan for main wafer

Before depositing 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-065.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-066.jpeg)

Everything ended fine too

Ellipsometer 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-067.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-068.jpeg)

We probably want 4 more mins of dep

Before dep 2

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-069.jpeg)

This should still have high confirement and little leakage even over 1 um of oxide.  This will definately be the highest index film we test.  I still think testing the N2 rich one in the future owuld be good, but that index was insanely low.  After this dep, we will run the long clean.  I will also get the PECVD going for a top oxide cap

During 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-070.jpeg)

5 min clean on Pecvd is going. 

Before season

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-071.jpeg)

Ellipsometery after

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-072.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-073.jpeg)

Still more borderline on loss than I would love, but it’s ok

Before cap deposition

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-074.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-075.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-076.jpeg)

Wafer is now third back in front of the box. Should be pretty easy to see



Below are some dispersion curves: 

![Screenshot 2025-04-28 at 2.29.41 PM.png](../../assets/fab/2025-04-20-follow-up-material-explorations-prior-to-annealing-077.png)

This is all before annealing ofc.  The Lipson LPCVD data should be taken with a grain of salt, as their stuff is deposited at a higher tempurature (so it should start denser and get rid of any non-bonded hydrogen, both of which could supress index).  Below is the reference where I got that index data: [https://refractiveindex.info/?shelf=main&book=Si3N4&page=Luke](https://refractiveindex.info/?shelf=main&book=Si3N4&page=Luke).  

The takachi is not as high as I origonally thought it was