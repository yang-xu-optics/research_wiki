---
type: craft-export
title: "2025-05-21 loss reduction recipe design"
craft_document_id: 2B7B0D94-448E-416D-B92A-D007047CD369
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-05-21 loss reduction recipe design
Looking to future, we still have a great interest in reducing the loss of our waveguides.  We are soon going to try this using the ASML stepper, which should be great for sidewall roughness.  Other ideas include:

1. Use dry etching of Cr instead of wet etching
2. Use e-beam to write ASML mask or try re-flowing resist 
3. Use in-house SiNx instead of SVM
4. Use oxide hard mask instead of Cr hard mask (include RCA clean after etch step)

The first idea is more simple and probably has less science behind it.  The hope is that dry etching simply causes less roughness.  It “feels” more professional.  Looking at how masks develop however, I am not sure how true this is.  

E-beam to write mask is mostly a roughness thing.  Even though we reduce roughness by 4x using the ASML, photolithography always introduces some roughness.  But e-beam should truly have no roughness whatsoever.  So we could always try that. Re-flowing feeling a little more practical.  I would have to look for recipes online, but this is definately something that reduces roughness.  The downside is you don’t get nice and straight sidewalls, but to be honestly, we don’t need nice and straight sidewalls.

In-house SiNx instead of SVM is a cool idea at a high level, but it will take a while to test.  It is mostly just an iteration time issue.  In the past, we tested SRN2.7, SRN3.5, and baseline Takachi.  Basline Takachi failed, so no need to do that (non-annealed was not bad, but annealed was trash).  We should probably try 3, 4, or 4.5 in the future.  I am generally biased against 3, but who knows, I could be very wrong about this.  I think Takachi will be too hard for the time being.  We probably can’t go too much higher than 4.5 for fear of loss.  I am also kinda under the impression that 800 C RTA is basically the best RTA recipe.  Anything higher seems to have marginal effect (if anything, the effect has usually been negative).  It is kinda annoying we have to make full wafers when we only need a few working dies, but whatever.  Maybe this is the place to test the oxide hard mask.

The last one is the hardest to judge.  On the one hand, removing anything that is lossy from the process (like Cr) is always nice.  We could be getting redeposition or who knows what by using a Cr hard mask.  This is just what the big boys do.  The other main advantage of an oxide hard mask is that we can try a higher temp (1150 C or 1200 C) anneal.  I am still a bit suspicious if this will work because of past results (1100 C waveguides sucked, and RTA at higher temps seems to break structures).  Nonetheless, this is the professional way to reduce loss. 

For oxide hard mask, we already have some data to get started with.  We used the oxide thinning recipe for 14.5 mins on a full wafer and went from 3.2 um of top oxide to 725 nm.  This means we have an etch rate on full wafers of 171 nm/min.  Below is what the book says

![Photo from Library.jpeg](../../assets/fab/2025-05-21-loss-reduction-recipe-design-001.jpeg)

It claims to have 2.5:1 selectivity to resist.  So if we use 600 nm of resist, we could have 1200 nm mask.  

Next, lets think about the CHF3/N2/O2 etch recipe we use for the SiNx.  We can figure out, by comparison, what we think the etch rate is to get an idea of the feasiblity.  For SVM nitride, we always start with 225 nm of Cr, 500 nm of oxide (except on one), and 2 um of SiNx (ignoring bottom cladding layers).  

After 3 mins of etching, we say 1.1 um of depth.  This one has 300 nm of oxide.  After an additional 3 mins, we had 2.4 um of depth.  Of course, this is not a perfect comparison, as we probably touched the bottom oxide, but from this, we guess we etch oxide at 433 nm/min, and oxide at 260 nm/min.

Using 7 mins and 500 nm of pad oxide, we etch 2.5 um down.  If we apply the numbers above, we expect to get down 2208 nm into SRN.  So we are overestimating SRN dep rate, or under estimating oxide etch rate.  

Using the material exploration is very reliable.

For SRN2.7, we used 445 nm of pad, 830 nm of SRN

For SRN3.5, we used 445 nm of pad, 840 nm of SRN

For Takachi, we used 445 nm of pad, 1200 nm of SRN

For SRN3.5, we etched for 5 mins, and saw 1600 nm dip.  Shaving 250 nm for Cr mask, we went 1350 nm deep.  This means 840 nm of SRN was etched, and 510 nm of oxide. 

For Takachi, we etched for 5.5 mins, and saw 1900 nm dip.  Shaving 250 nm for Cr mask, we went 1650 nm deep.  This means 500 nm of oxide was etched, and 1150 nm of SiNx.  Lets round and say we want all the way down in both.  The math above does not work out.  It predicts way too low of an SiNx rate.  The book in the CNF did not really have many useful comments.

I would start with my first rough calculation.  It is not perfect, but we roughly predict a 1.6:1 selectivity.  To etch 2 um down into SiNx, we would need 1250 nm of oxide hard mask.  In theory, this is possible, so long as we use a 600 nm thick photoresist mask.  The etch rate of resist could depend a bit on the type of resist (we can also try some post-bake tricks to harden the resist).  The main idea is we need to use the thicker recipe.  So if we use 600 nm of resist, we should be able to etch down at least 1200 nm of oxide.  Given the etch rate found above, that means etching for 7 mins using the above recipe with CHF3/O2.  Next, we use the CHF3/O2/N2 recipe for 5 minutes.  This should etch most of the way down.  My hope is that we will have minimal top oxide mask left after the second etch, and minimal resist after the first etch.  

For the trial of this recipe (for characterization), we need to use in-hosue PECVD (mostly because of the delays with SVM).  This gives us the chance to try some new PECVD recipes out for loss.  4.5 is probably a bit high. We can try SRN 3 and SRN 4 on for size and see how they work.  It would be nice to double this experiment as a way of seeing (with ASML) what minimum losses we can achieve without high temp annealing.  For that reason, I am avoiding Takachi.  Below is the Cauchy fit for SRN 4

![Photo from Library.jpeg](../../assets/fab/2025-05-21-loss-reduction-recipe-design-002.jpeg)

We can then calculate the index as 

![Screenshot 2025-05-22 at 12.16.27 PM.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-003.png)

![Image.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-004.png)

4 seems to give us an in-house recipe that is pretty close to the SVM performance.  Honestly, I am a but less interested in 3 at the moment than 4.5.  If I extend these plots, we get

4.5 Cauchy

![Photo from Library.jpeg](../../assets/fab/2025-05-21-loss-reduction-recipe-design-005.jpeg)

![Image.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-006.png)

It seems 4.5 is a bit high.  There is no huge parallelization between doing one or two waferse minus getting more information.  There may be a fair argument though for doing 3.8 and 4.2.  Eh, I am going to trust my gut and do 3 and 4.  This should give a strong answer as to whether higher or lower index is better, or whether 3.5 already hit the goldi-locks zone.  For now, we will still flow hydrogen, though I am certain this is not ideal for device performance.  



Below is leakage

![Screenshot 2025-05-22 at 12.21.48 PM.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-007.png)

![Image.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-008.png)

![Image.png](../../assets/fab/2025-05-21-loss-reduction-recipe-design-009.png)

SRN 4 roughly has an index of 1.96 at 1550.  So 1.5 bottom is good, but just to be safe (and because oxide deposition is so much faster), we shall do 4:40 mins bottom oxide to get 1.75 um.  This should allow us to get away with 800 nm in both cases.  Keep in mind, this comparison is not perfeclly comparable, as the lower index has lower confinement, but it is a heuristic to get started with.  We know SRN 4 has a deposition rate of 41.6 nm/min and SRN 3 has a depsition rate of 34 nm/min.  So we deposit **SRN 4 for 20 mins, and SRN 3 for 24 mins.**  