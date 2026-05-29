---
type: craft-export
title: "2025-03-01 1100c sinx annealing literature search"
craft_document_id: 652B85D3-083C-4666-8C02-7196EA8285DB
craft_collections: [etching-sin-waveguides, fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-03-01 1100c sinx annealing literature search
While Ryo and I previously showed 1100C to reduce loss at 1520, recently annealed SiNx devices with full packaging still showed loss.  There are a couple of differences between the devices, listed below:


1. The origonal device that showed minimal loss was ~1cm long, while the deviec that showed loss was 2cm long
2. The origonal device entered the furnace tube as a piece, NOT a wafer.  The device that showed loss entered the tube as a wafer
3. The origonal device that showed minimal was was air top clad, while the current device that showed loss had a PECVD TEOS top cladding. 
4. The device with more loss had a photoconductor.

Personally, my suspicision is that the TEOS layer is what increased our loss.  That is a PECVD layer which probably has plenty of Si-H and N-H bonds remaining.  We also should have pushed for the furance tube to go higher than 1100 C.  The last part is this is a diffusive process, so it is possible that 3 hrs was not long enough given how thick our waveguides are.  I personally don’t think the fact that we annealed on a full wafer matters too much, but that is just me.

[Optica Publishing Group](https://opg.optica.org/oe/fulltext.cfm?uri=oe-26-8-9645&id=385310)

This is the first paper Ryo sent me.  For reference, I am not really that interested in what they used the waveguides for, mostly the fabrication and film characterization.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-001.png)

They use our same trick of etch first, anneal second.  It seems they use fairly thick waveguides and observe nonlinear phenomina, meaning annealing should not totally screw up our ability to see E-Fish.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-002.png)

They mention using a thicker BOX, which is nice but we can’t do for electrical reasons.  They also use a smaller bend radius than us at the moment, meaning I am not yet worried about our spiral waveguides (and theirs are impressively long).  Other dimensions are actually more aggressive and I am surprised this worked with only contact lithography

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-003.png)

They now show my first hypothesis.  They do cladding BEFORE annealing.  They also use the PECVD for their top cladding

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-004.png)

Another important idea is somewhat confirmed here.  They anneal at 1150 C, not 1100 C.  I believe this would make a difference.  Their atmosphere is also a bit different, with the first part being O2 and the end being N2.  We do a mixture of the two.  I don’t think this matters a tonne, but I am not sure.  Their ramp is similar to ours.  Their anneal time is similar to ours.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-005.png)

Random: They use a very interesting spiral shape, but it would probably be easier to align to something like this because input and output overlap

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-006.png)

Tough to analyze what is being shown here.  They still have photoresist ontop, which makes me believe their waveguides were a bit thinner than ours.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-007.png)

Their transmission without annealing, which looks like ours

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-008.png)

This also kinda says our tempurature might have been too low

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-009.png)

After annealing, they see flat loss

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-010.png)

Just the effects of scattering loss, but they finally confirm their waveguide thickness of 580 nm

[Researchgate](https://www.researchgate.net/profile/Alfred-Driessen/publication/241875246_Characterization_of_thermally_treated_PECVD_SiON_layers/links/0f31752ebeffabc15e000000/Characterization-of-thermally-treated-PECVD-SiON-layers.pdf)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-011.png)

They use an N2 environment.  I truly doubt it matters much, but maybe I am wrong.  They also use a higher final annealing tempurature.  They seem to confirm the 3 hour annealing time as well, and they have some fairly thick films, so I think it transfers to us.  So I don’t think longer annealing is needed

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-012.png)

It is interesting to see that annealing at 1000 C really does not help much.  They mention crakcing, but given our etching trick, this is not relevant.  This reinforces the notion that 1150 C annealing is best.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-013.png)

Kinda as we expected.  The N-H bond is really the killer

[Laser annealing of SiO2 film deposited by ICPECVD for fabrication of silicon based low loss waveguide](https://link.springer.com/article/10.1007/s12200-016-0616-1)

These people seem to help confirm my intuition that PECVD SiO2 is lossy, though I can’t say they give the level of detail that I would like.  They test their waveguides with SiO2 claddings and Al2O3 cores.  They also use a laser annealing procedure instead of furnance annealing, so this is not a perfect apples to apples comparison.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-014.png)

This more confirms my idea that PECVD oxide != thermal oxide

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-015.png)

[Optica Publishing Group](https://opg.optica.org/oe/fulltext.cfm?uri=oe-19-24-24090&id=224301)

This paper again confirms the oxide intuition

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-016.png)

They also seem to do annealing of the oxides

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-017.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-018.png)

Below they report on losses

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-019.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-020.png)

An interesting feature here is this is still with waveguide annealing, though the losses are still very small.  I guess this goes to show that the photoconductor is probably causing some amount of loss, as there is obviously a bit of overlap

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-021.png)

Above is with no PECVD oxide, which is obviously better.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0925346703003513)

This seems to be a sorta “seminal” paper on the composition of PECVD films.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-022.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-023.png)

Above is for oxides

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-024.png)

Above is for oxynitride and nitride.  So obviously the effect of the N-H bond is weaker for a normal oxides, but it is definitely noticable.  SiON is easier to see.  So it is not clear how much it matters, but we see a lot in nitride.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-025.png)

An interesting observation is O-H bonds begin to dominate with more N2O flow than N-H bonds.  Our PECVD SiO2 is deposited with a huge abundance of N2O.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-026.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-027.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-028.png)

It is just tough looking at this to be convinced we are really seeing N-H bond issues with our oxides, as they at least have an order of magntiude less N-H bonds.  Then again, we did see less loss otday then normal.  This more convinces me of the need for higher tempurature

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-029.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-030.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-031.png)

They anneal the lowest index SiON (n = 1.5 at 1550) in an N2 environment.  This seems to get rid of most of the N-H.  

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-032.png)

It seems that O-H bonds are weaker, as they are gone by 800.  

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-033.png)

This is for the same SiON as before.  I still believe some loss is caused in the oxide, but it is clearly not a tonne

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-034.png)

They probably use recipe 3 or 2.  Interesting that this is definately on the order of the oxides, so maybe I think this loss is the issue

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-035.png)

This seems to confirm that even this small amount of N-H can still cause some loss.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-036.png)

They seem to also use 1150 C as the tempurature.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-037.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-038.png)

Despite the whole conversation, it seems that they don’t anneal the device as one, but rather use a normal PECVD cladding at the top.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-039.png)

They at least acknowledge this fact, so it might still be possible.  I think the most important thing is annealing at 1150 C

[Optica Publishing Group](https://opg.optica.org/ao/fulltext.cfm?uri=ao-30-31-4560&id=39335)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-040.png)

This says it all.  It is also interesting that they use think 5um waveguides and only do annealing at 1100 C (instead of higher).  

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-041.png)

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-042.png)

It seems that 1100 C does not remove the peak around 1.51 um, which would also confirm our recentl annealing results

[Optica Publishing Group](https://opg.optica.org/ol/fulltext.cfm?uri=ol-40-21-4823&id=331311)

A Lipson paper, so we know its good

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-043.png)

Interesting that they comment that H has a hard time diffusing out of SiNx

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-044.png)

They also annealing their PECVD oxides, which is a bit interesting

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-045.png)

They are serious about getting resiudal hydrogen out of their films.  I don’t think we will do that extreme

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-046.png)

This paper really makes the point that you want to anneal thinner films to allow the hydrogen to leave the film.  The above graph is without annealing cycling, which is evidently worse

[Arxiv](https://arxiv.org/pdf/2301.03053)

This is the old paper that Martin and I got excited about for using SiNx from the PECVD as a waveguiding layer.  As we are learning now, processing SiNx is not so trivial.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-047.png)

They annealed at 1150 for 3 hrs in N2 environment for PECVD SiNx.  They had top cladding on, and things seemed to work.  I am sure the loss would have been better if they used cycled annealing (based on the above paper), but for our means, it looks ok.

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-048.png)

Above shows how loss goes down

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-049.png)

It seems RTA helps reduce loss, so we should be able to observe some imporvement over the RTA devices with furnace annealing (at least that is the hope).

![Image.png](../../assets/fab/2025-03-01-1100c-sinx-annealing-literature-search-050.png)

Interesting that reactively sputtering SiNx could also be good.



Email quesitons for the last paper:



(Some greeting), 



(Some introduction).  We are emailing to inqiure about your work reducing loss in PECVD SiNx in [https://arxiv.org/pdf/2301.03053](https://arxiv.org/pdf/2301.03053), which was performed in the CNF like our current work.  We previously demonstrated programmable E-Fish on a slab waveguide (reference to one of your conference talks or attach paper manuscript).  We are interested in expanding this work to etched SiNx waveguides to take advantage of the higher propagation lengths, confinement, and dispersion engineering capabilities.  Additionally, we would like to eliminate loss at 1520 caused by N-H bonds so we can do spectral engineering over a larger range of the C-band.  Because we are using etched waveguides, our structures can survive annealing at high tempuratures without stress-induced cracks.



Recently, we fabricated SiNx waveguides and, after annealing, we did not observe any drop in the loss at 1520.  We measure loss by coupling into our etched waveguides using an aphserical objective lens and use a power meter to see the transmission spectrum from 1500 nm to 1630 nm.  After annealing, we still see a distinctive transmission drop at 1520 nm with greater transmission at 1500 nm and 1550 nm.  Our fabrication procedure follows the following procedure.  Starting with 2um thick SiNx wafers from Silicon Valley Microelectronics (inlcude link to wafers), we deposit 300 nm of PECVD oxide followed by sputtering 150 nm of Cr.  We pattern the Cr and then use the Cr as a hard mask to etch the SiNx so we have waveguides with widths between 3 um and 9 um.  We wet etch the Cr mask away and then anneal at 1100 C for 3 hrs in an N2 and O2 environment.  After annealing, we deposit an additional 1um oxide cladding in the PECVD using TEOS, deposit a 6um silicon-rich ntiride layer in the PECVD (which gives us programmability), and sputter 30 nm of ITO.  



Our questions for you on how to minimize loss are below:
1. We saw in your paper that you anneal at 1150 C.  Do you believe this 50 C tempurature difference is critical to removing more N-H bonds?  Do you believe annealing at 1200 C would be even better?
2. We saw that your waveguides are only 730 nm tall and 1500 nm wide, meaning ours are much larger.  Do you think that larger waveguides require longer annealing times?  

3. If we had to keep the annealing tempurature at 1100 C because of CNF material resistructions, would longer anneals help decrease loss?
4. Is waveguide loss performance effected by annealing with or without the PECVD cladding on the device.
5. Do you expect that PECVD SiNx’s provided by different sources (ie, one from the CNF’s PECVD and the other from SVM) to have different annealing conditions to remove loss?
6. Is sidewall roughness effected by annealing, and if so, how?



(Closing statement and thank you for his time)