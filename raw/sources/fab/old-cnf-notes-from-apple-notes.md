---
type: craft-export
title: "old cnf notes from apple notes"
craft_document_id: 5850C67F-9776-4FCA-862A-7FECE2B08116
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# old cnf notes from apple notes
CNF Notebook (2D waveguide):

April 19 2022

Today I processed the chips I made on Monday (which have 4 um of 40/10 SRN on top and 1550 nm of Sio2 between that an a p-type substrate)

I picked apart the wafer, and then placed three batches of pieces in the cleaners for 15 in the first two and let the rinse cycle go.  I then dried off all the pieces.  For 12, I also spin cleaned with acetone and IPA and then put them in the YES oven.

I spun everything at 3500 rpm at a 5000 ramp for 45 seconds.  Then heated at 115 C for 1 min Here are the results

I could not characterize depth, so today will be uniformity.

1. 4 drops of poorly placed 1805 then heated a little too long, I got good uniformity in the middle (though the corner problems were annoying large).  (Top right)
2. Dropping a third of the pipet onto the chip had an almost identical uniformity upon observation.  (One below top right)
3. 3 well placed drops of 1805.  Could be better, but it is tough to tell by observation.  Could be that it was not centered properly (though it really looked to be centered right) (two down from top right)
4. This one had three drops a bit off center at 6500 rpm/second ramp.  It seemed to bite a bit more into the corners with less problems, which is certainly progress (three down from top right)
5. This one had three drops in the center at 8000 rpm/second ramp.  It looks the same as above (I also had hard time taking off heater, so that does not help).  I don’t think going higher than 6500 helps much. (Five down in right-most column)
6. Back down to 6500, but with 4 drops around the chip.  Looks basically the same.  There was too much air as I dropped.  Try to do it continuously (like you did at Pitt).

The chips are put away as follow.  Good but needs cleaning (3).  Has primer on it (2).  Has baked resist or extra pieces (1)

April 20 2023

I had lots of trainings today, the summary and important notes are below.  For chips, I need to enlarge my klayout stuff.  It is currently 10X too small.  Next, I need to plan to see Roberto tomorrow.  I have settled on the following spin recipe

3500 rpm, 6500 rpm /sec ramp, and 45 seconds total.  Can’t get more uniformity, but I can adjust the speed if I want different thickness.  I bake at 115 C for 1 min after.  Get special tweezers from box to make picking up chips easier.

Chips are in boxes as follow

1. 5 resist coated chips and spare pieces
2. Four primer chips on the left and 3 bare (but clean) ones on the right)
3. Same as before

April 21 2023

Today, my objective is to get either a mask writing procedure done (retrain on Heidelberg) and or figure out the best yilmetrics or ellipsometry procedure to measure Photoresist thickness.  If I am able to get Heidelberg working, we need to start perfecting the recipe to get best resolution possible

If I really want, I can give sputtering my first try.  I would also cleave a wafer to get a few chips to start getting a chrome mask on.  Figure out chromium thickness.

What I actually got done.  I got training on the DWL 66.  My detailed instructions are in my recipe guide.  I got filMetrics to work as well.  I know my spinning recipe produces films between 520 and 5353 nm thick, which seems acceptable.  I did not hear back from Jeremy or Tom.  I did hear back from Chris.  We need to make several cad files where we can see the different size of different squares.  We should not need to adjust dosage, just the size of the squares on the cad file.  We want to be able to leave a quick space to tell how deep we have developed so we can use yilmetrics to measure.  To do this, create large rectangles.

Objectives over the weekend:

1. Confirm time of Tuesday meeting.
2. Design Cad files.
3. Follow up with Jeremy and Tom about sputtering tool and whatnot.  I want to get the stepper tuned on Monday or Tuesday and get the recipe for the chrome sputtering down too.

Ideally, I now know the development and spinning parts of my process.  Once I get sputtering and stepping down, which should come soon, I can etch the chrome.  I hope to have this finished by the end of next week and possibly do my first silicon etch.

Tentative schedule.

Monday/Tuesday:  Hopefully I will know the ideal thickness for my chrome.  Do a practice run with Tom and perfect that part.  While that is running, get the stepper going too.  These will likely be some longer runs.  Characterize my resists using either FilMetrics or the optical microscope.

Wednesday: Now that your process is perfect up to etching, create a few samples to do a chrome etch on.  Then do your first chrome etch.

Thursday:  Hopefully, we can get training on Silicon etcher by now.  During training, get your first silicon etch in with some of the good samples from chrome.

Friday: Characterize your silicon etches.  Learn the best way to remove Chrome mask.  Make more samples to test.

May 1 2022

Here are my objectives for tmrw in the cleanroom.  I ran the etch last time for 6 minutes and 5 seconds.  I first want to characterize my last Chrome sputter.  I will then figure out best time, do one last chrome sputter, and characterize that to makes sure I like my time.  I will need to remove the extra photoresist from my chrome with 30 minutes in each bath.  I also want to etch my new exposure.

Here is what I want to do, in order:

1. Put Chrome etched sample in photoresist removal tubs, 30 mins in each tub.  During this time, do a liftoff for the characterization sample for chrome sputter.  Profilometer this sample, and see what we get.
2. Characterize the chrome etch we did to figure out etch rate.  Then do another chrome etch with our newly exposed sample from last time.  Characterize this etch.
3. At the same time, set up one extra exposure, and see how large we can make it.  I want some long stuff.

11:40 chrome etch

Here are the known rates

We would expect Cr to etch at 38 nm/sec, and Cr to deposit at 0.95 A/sec.

Here is what we observed.

For a 2420 deposit, we saw, on the characterization chip, a height of 2156 A.  That means rate of 0.89 A/sec

For a 4840 deposit, we saw, on the shadow left by the clips, a height of 3500 A.  That means a rate of 0.72 A/sec

For a 6600 deposit, we saw, on the characterization chip, a height of 5908 A.  That means a rate of 0.89 A/sec

Using rate of 0.89 A/sec, and wanting a height of 4400 angstroms, we should deposit for 4943 seconds.  Rounding, we will use 4950.

For etching, when we etched the 215.6 nm Cr for 6:10, we got height of 92 nm.  That means etch rate of 0.24 nm per sec.

Here are some comments on what Tom said.

1. It will be very hard to do a lift off of a 5 um mask of SiO2 for ion implantation.  We can try, but that is really not what these masks are built for.
2. We need to add a descry step after development.  This will remove residue photoresist.  90 seconds in the Oxford 80 is what Tom suggested
3. For characterization, I have a few considerations.  First, I should deposit for 4950 with the new etch rate that I found.  We can ONLY characterize these chrome depositions using the liftoff samples.  Anything else is not reliable.
4. I should leave the photoresist mask on the chrome after I do a chrome etch.  It is hard to remove right now, and it will probably be easier to burn it off in the Oxford 100.
5. Characterization etch will regime the use of the zygo.  While the use of larger features is not a bad idea to get a ball park for the time it takes to etch the chrome, we should over etch.  Etching finer structure will always be harder than big structures.  We can tell if chrome is still on surface by using the point filmetrics.  The readout from chrome will be a flat line, as chrome is reflective.  We can tell if we are on a Silicon layer if there is periodicity.
6. Roberto suggested I spin coat my samples when we mount the chip on the silicon carrier wafer with the four edge pieces around it.  I am concerned about this approach, as the side pieces may fly off.  That being said, it would give me a more even coating, which is currently a problem.  This is a low priority test for me.
7. We will need LONG cooling step for our samples when we do silicon etch.  This is because SiO2 is a thermal insulator

May 9 2022

Here are the two resist thicknesses after discus.  364.1 nm and 355.8 nm.  Fairly close, but ~100 nm of error.  Before descum there was about 430 nm of resist, so discus shaves of about 70 nm

After 13 min Cr etch, I observed side profile of 445 nm (including resist).  After stripping resist, I observed side profile of 428 nm.  This means my resist accounted for 23 nm of what remained

Using Zygo, I observed trench depth of about 380 nm (including resist).  Factoring in resist thickness (and assuming it etched the same everywhere) I observed Cr trench etch distance of 357 nm.

I etched through 337 nm of resist.  So I etch resist at a rate of 25 nm/min.

This means the etch rate is 27 nm/min and I will want resist of at least 450 nm thick.  The ratio of side etch to trench etch is 1.19:1  and observed selectivity in the trenches is ~1

After leaving my sample in the strip baths for 10 minutes each, The surface did not show any residual resist.  This could be because I stripped it all off, or etched through it.  I the surface texture also looks fairly similar.

As a side note, 4840 seconds in sputtering does consistently give 450 nm.  Another test chip confirms that

I want to etch, therefore, for 16.66 minutes, but we can make that 18 just to leave some wiggle room.  Based on that calculation, we want 475 of resist when we etch.  Since discus removed 70 nm, we want 545 resist going into descum.  Basically, we need 100 nm more resist after spinning

May 15 2022

Etch depth of 320 nm for 18 min etch.  This means an etch rate of 17 um per minute.  So we would want 28 minute etch.  That means we need a mask of

We get side wall height of 412 nm

June 2 2022:

We are trying to address the variable etch rate we observed before break.  The current thesis, which I agree with, is that the descum was not good enough, leading to a bad etch.  Basically, the photoresist mask was not cleared.  To address this problem, I am testing two different chips today.  Both are starting in box 2.  The bottom one (closer to where the lid meets the base) was exposed with a dose of 60 in DWL and was descumed for 1 minute with Ar.  The other one was exposed with a power of 60 in DWL and will be descumed for 90 seconds with mild descum (O2).  This one is in top of case.  I descumed with Ar before break and O2 today.  I don’t think the three weeks of no activity matters much.

I should also note that box 1 and 2 probably have a few samples that should be tossed or cleaned.  I will take stock of what I have by the end of the day.

530 nm resist height for Ar chip

The O2 chip was 430

An odd thing I noticed was that it did not seem that the color of the O2 resist changed much.  I thought color was indicative of height, but it might just be the way the Ar reacts with the surface of the resist.  While I still believe the O2 chip started with the thicker resist (given the sizes of the edge beads) I would double check it just in case when the process is over.  Go for repeatability, basically.  When I looked into the depths of both of these chips, the trenches looked cleared.  Some of the other, older, chips did not look cleared (probably why I had problems etching).  I am going to etch the chips one at a time just for my own sanity.

Stock of what I have left:

Box1: Far right: plain chips with resist coating (unsure what thickness, but probably around 500), middle-right: 250 Cr, some etched, some pattern, some not.  These should be put into storage in box 3.  Middle-left:  Etched 450 Cr, 450 cr with thin ~300 resist mask.  450 Cr with thick Pr mask.  Far-left: Descumed thick mask, but lower dose.  Not descum but mask with lower dose.  Both 450 nm Cr.  The ones with masks should be stripped.

Box2: Far-Left: Thicker Cr mask (~520 nm), primed normal chips, and testing pieces for thickness of 450 cr sputter)

Box3: Bottom left: Etched through thinner resist, and bed etch thicker resist.  The one with normal looked Cr on edges is bad etch with thicker resist.  Everything else are virgin chips.

I put the 1 minute Ar with 60 dose in first.  I did 18 minute etch.  I also seasoned the chamber for 10 minutes before.

After 18 minute Ar, no resist removal, I observed a side profile of 540.  While some IPA got on the top corner of the chip, this part still had intact resist.  Under the microscope, it seemed like I still had resist in tact, but the edges the trenches in the middle did not seem to Clear.  The ones in the middle seemed ok though.

After 18 minutes O2, no resist removal, I observed a side profile of 460.

If Zygo is to be believed, I got 325 nm deep etch.  That being said, the image the zygote gave me was not great.  I believe it would be better to leave resist on the chip in the future. My resist was definitely still on chip for this one.

Zygo worked much better on the O2 chip (which definitely etched through my resist).  Here, I got an etch depth of 390.

After stripping resist from Ar chip, I observed a sidewall profile of 360.

After stripped for O2 chip, I observed sidewall profile of 450. This means, in reality, the Ar chip must have had 180 more resist, which just does not make sense.

I primed the extra 4 450 nm chips, which are in box 2.  After retesting the chip I etched before break (which had a dose of 50 instead of 60), I observed a sidewall profile of 360.  This is highly interesting.

June 4

Based on some of our results, we know that 390 nm trenches with a resist of 430 nm.  Before, I got a 357 for a resist thickness of 360.  While these are not perfect matches, it basically says that I need ~500 nm of resist.  Which, btw, I had.  These results are close enough that I can consider them consistent.  Now comes the problem.  I had that much resist, and did not etch far enough.

I think the strangest result is from yesterday and before break.  In these cases, I had an etch depth (with no resist) of 325 despite having a resist of 530 before hand.  Moreover, the result I have would imply I stripped 215 nm of resist, which is not possible.  So this begs two questions:  Is the Zygo broken (which we have reason to suspect) or is the Cr lifting off as well.  While both seem to be the case, I would go with the former case.  I don’t love the strategy of using filmetrics.  I feel like the optical microscope is good enough to see the grey of Cr.  Given the pealing I have seen, I suspect the core problem is the Cr.  I will probably need longer etching times too.

Other hypothesis include problems with clearing my resist.  There are three solutions: chemical of descum (Ar or O2), time of descum, or dosage of DWL.  With dosage of 60 and Ar descum of 60 seconds, I got bad results.  These, clearly, are not it.

June 5

I did a quick measurement under the filmetrics just to get a taste of how the system works.  Firstly, I would not use the one in the photolithography room.  I can’t change the recipe.  I would then go to the one that acts like a microscope.  It measured my photoresist, with a cr substate, to be 700 nm thick.  It is hard to read the charts for the photoresist, but this is not inconceivable.  I think the key, after descum, is to observe Cr in the large open regions under the filmetrics.  While Photoresist has squiggles under the filmetrics, Cr is just a logarithmic line.  Likewise, I observed squiggles for the SiO2 for my overreached sample.  For under etched one, I saw squiggles in the large exposed regions, but not in the thinner grating area.  I was able to see squiggles in the grating area for over etched.

My basic conclusion is that I should see some flat lining in the grating area (squiggles reduced) and none in the large open areas.  I was surprised by the goodness of my fit when I got 700 nm thick, so I may need to descum longer than I thought I would.  Recall that O2 etches the resist at 50 nm by minute.

On Zygo, I measured thickness trench depth of 380 nm before descum.   Though, if I am going to be honest, I am not sure how much I would trust this measurement.  I got several readings of 90 nm with the zygo (using the same settings that got me reasonable measurements with the over etched chip) so this is not helpful.

Let’s think for a moment: we have two samples with unknown resist thickness.  Two things I would do; coat the mounting wafers with 1815 at 2000 rpm. I think the filmetrics would have a better chance on these.  Then use filmetrics and profilometer to get a range of measurements about the big features.  This will at least tell us how much photoresist we have.  When we do descum, I would do another 90 second mild descum.  The other chip I would save and see what we get.  We may want to ask Roberto about the zygo readings and what he thinks is reasonable.

Just to reiterate (before descum), I saw squiggles for larger features and none for the open large areas.  This indicates I have very little resist.  Unfortunately, it could not measure how much resist I had.

After washing, priming, spin coating, and baking for 1 minute, I found that I start with 670 nm of resist.  With surface profilometry, I got big feature step size of 600 nm and I got 620 on the other chip.  Basically, I lost 60 nm.  We have to descum for a minute in a half, and then I say we are good.

On the under etched sample from yesterday, shiny regions have step height of 360 nm, while broken regions have step height of 390 nm.  I admit, not what I expected.  For the lighter flake regions next to broken areas have height of 20 nm.  Maybe that stuff got around?

Purple area (large cr flake) shows height of 417.  Interesting.

The purple stuff has height of 25 nm.  No broken Cr shows step height of 410.

I confirmed that the current process, when exposed to a 90 second O2 descum, goes to resist height of 430.  This is simply too low.  If that number is to be trusted, which I do trust, that means I lost ~180 nm of resist.  That is a lot.  I only need to lose around 100 nm, so half the time (50 seconds) is ideal.  Let’s try that.  I should also note that, after descum, you see fine lines of red and the greens look a bit more like lime green (brighter and less dull).

After 50 second descum, I get a resist height of 500 nm.  I also took a picture of the trenches, and it is pretty clear that it is Cr in the middle.  I am not sure this is much better than Ar, but if it works, it works.  I should note that the filmetrics seems to be off by ~200 nm each time.  This confirmed by suspicion that the O2 descum etches resist at 2 nm per second.  After all, I started with about 600 nm or resist, and after 50 seconds, ended with about 100.  Given that I have 70 nm of unaccounted for resist, this is fine for me.

Because the 90 second descum chip does not have enough resist, I only etched it for 10 minutes.  I figured this could help me better understand the etching rates, as I hope to see how much resist/Cr is left.  I am not sure how to strip the resist, but we can figure that out eventually.  I observed step height for a large feature of 430 nm.  I admit, a bit odd.  The filmetrics guessed a range of numbers (none of which were close) so it was not helpful.

Things to send to Giovanni:

Pictures of filmetrics with his recommended stack (and the settings)

Picture was restricted wavelength.

Question about etched photoresist behaving differently

Pictures of cracked parts of Cr, both large cracks and smaller features.

After using Zygo on the 10 minute etch chip, I got a feature depth of: ~410.  These were taken near the edges, as that is the only place where I could get the thing working.  Still, the plot looked fairly accurate, so it may be that I get, in my trenches, almost the same that I get on my big features.  Once more, all quite surprising.

June 6:

Using the SEM the other day, I observed the following (this chip had 430 nm of resist, 450 nm of Cr, and was etched for 10 minutes):  203.5 nm of Cr (though error in the recording could mean there is a bit more), 181.8 nm of resist.  That means, in 10 minutes, I etched away ~247 (possibly a bit lower) nm of Cr and 249 nm of resist.  Basically, it is a 1:1 etch selectivity for the trenches.  So 500 nm is for sure enough.  While I should technically say I etch Cr at about 25 nm per minute, in reality, it is probably more like 22.5 nm per minute.  So, if I want to over etch by 10 nm, 460/22.5 = 20.5 minutes.  Likewise, that will leave me with no resist left.  Let’s try 20 minutes and see what we get.

After doing a 20 minute etch, I observed my resist, which I do still believe to be on my sample, to be blue.  The reason I believe I have resist is over etched samples have grey stripes, while mine look blue.  There are also a few fews where my resist was a bit thinner, and these areas look grey.  I suspect 20 minutes is optimal.  It also seems that areas where the DWL went out of focus still have a small amount of resist left, which surprises me.  I see some blue and a bit of grey.  The point, I guess, is that those areas should still be usable.  I will do a filmetrics, zygo, and p7 characterization later.

On a basic note, I am doing another 4840 second sputter this afternoon.  I just want these additional chips.  I will look at test sample tmrw.

Using P7, I observed 513 sidewall.  This means I have a lot more resist left than I thought.  Using the filmetrics, I was not able to get a usable measurement of thickness.  That being said, I saw only three squiggles for the rectangles, and lots of squiggles in a complicated way over the main part of the sample.  Because few squiggles if indicative of thin transitive material (like photoresist) and lots of squiggles gives thick transitive material (like SiNx and SiO2), I think this shows that I have some resist left and cleared Cr in the larger areas.  As a further analysis of the sidewall reading (which I implicitly trust), it would seem that Cr does etch a bit faster than photoresist.  It is also possible, given how light the photoresist appeared on the SEM, that we did not accurately measure that distance.  This does seem to slightly contradict my data for the feature depth from the 10 minute etch, but not by a horrible margin.

Not saying I should trust Zygo reading, but in the middle, it says ~280 nm.  Near the edge it claims 280 as well.  It even claims the side walls (for large rectangles) are 280.  Clearly a bit off, but at least consistent in its error.

After SEM imaging, I can confirm that we did in fact clear Cr, and most likely did not over etch.  Technically, I did not see much of an indent into the SiNx layer, but this is to be expected, as I was barely etching through the Cr.  I would have seen 10 nm max, which is within the error limits of the bars of the SEM.  What is more interesting is that the gaps between my features are closer to 1.6 um while the stripes are only 4.4 um wide.  To be fair, this is not totally unexpected, as I was using a manual measurement and I did notice in that past that the gaps were very perfect in their alignment with the ticks in the iris.  A bit unfortunate, but otherwise not a big deal (which Martin confirmed)

June 7:

When I measured the 10 minute etched sample using Giovanni’s improved filmetrics recipe, I got 225 nm with a 99% fit.  Recall it started with a mask that was 430 nm thick, so about 200 nm per 10 minutes.  For the 20 minute sample, I got 106.39 nm with 89% fit.  Recall that the started with a mask that was about 500 nm thick, so this measurement agrees.  This means the filmetrics is not a bad tool.  The way I did this, though, was using the one in the bright hall on the right and looking at a large area of resist that was not apart of my pattern.

As an additional check, my Cr is indeed 450 nm thick.  In addition, It seems that the step height for one of the new four samples I made is 617 nm.  Our expectation value for post development is a bit greater than 600, and after descum is a bit greater than 500.  Both give us plenty of space in the Cr etcher.

So far, everything looks good.  While Tom said I could put all four samples on the same sapphire wafer, I am only going to put two on at a time.  I am cutting my etch close, so I would rather keep everything close to the middle.  This means two, 20 minute runs.

Now that the four chips are done, I can’t tell if the trenches fully cleared.  It may be worth trying for another minute.  I currently see that I have about 515 nm step height, so that means, if there is 450 nm of Cr, I have 65 nm of resist.  We could even do a minute and a half.  To an extent, I just sorta need to trust that I am through.  If I am not, the beginning of my SiNx etch should clear both the resist and Cr remaining (as there is no way there is more than 10 nm left if any).  The new samples also look like the previous one that worked.

June 25:

Ya, it’s been a while, I am aware.  Suffice to say, things in the cleanroom have been broken/unavailable for a while.  Also, given that the imaging project is coming to a wrap, I am being assigned a small new waveguide core development project, specifically for SiN.

Here is what we have in the works and some helpful notes for us as we move forward:

1. Etching the SiN layer.  We want to shoot for a 3 um etch (or at least know our etch rate well enough that we can do something longer as well).  We got trained on the Oxford 100 the other day
2. Filling the holes and polishing.  While I can’t do this right now, I merely wanted to place this here as a todo
3. SiN thin film deposition

For 1. Here are the basic things we ought to note: We can pretty much put as many pieces on the sapphire carrier wafer as we need.  Because this is at a lower pressure than the PT770, there should be less decrease in etch rate in our small features.  More like 5-10%, but 20-30% as we saw on the PT.  There are three possible recipes that work for us.  The two that Hiro sent, and the one at the back of the book.  While Tom said we ought to add an extra long cooling step, Jeremy did not think that would be necessary.  Because the machine is a bit tough to light, don’t mess with the recipe parameters.  Just leave them be, or the gas won’t light.  All that we can adjust is the time for each step.  The software runs similar to that of the PECVD.  Before we use the machine, we should do a 10 minute oxygen clean, and then a 5 minute season with whatever etch recipe we plan on using.  Make sure there is ALWAYS a wafer in the machine when we are using it.  If a wafer has a flat edge, align it with the two knobs at the bottom of the machine.

June 26:

We are going to do out first Oxford 100 etch using the sample that is cut in half.  Just to get some basic measurements, the step height of a large feature is about 600nm.  Maybe a little less.  Thing don’t look as flat as I would like.

While filmetrics is not the most useful measurement, we saw 3500 nm of SiN with that.  Not helpful.  I should note that there is some dust on the sample that I can’t get rid of.

I did ten minute oxygen clean, then a five minute season.  I am using the “CH2F2/high He Nitride Etch” recipe.  The book claims a 244 nm/min etch rate with a resist selectivity of 4.5:1 for nitride.  Let’s assume that Cr is closer to 7.  We are going to try etching for 8.5 minutes and see what we get.  This is to characterize our rate.

The filmetrics is giving me useless readings.  That being said, there does seem to be a lost of dust on my sample.  I should not have made my test samples when I did.  Using Zygo, top height was 0.35 um, and bottom height was -1.6 um.  This is actually what we expect.  Optical microscope does not show anything unexpected, besides confirming that there was a lot of dust.  In the future, if we need new test samples, make those on Monday.  We don’t want any samples sitting for longer than a week.  Profilometer gives agreement with zygo.  1.9 um.  We need flat surfaces to make the zygo work

Look under SEM:  ~400 nm of Cr remaining.  1.65 um etched.  1.361 um of SiN remaining.  2.9 um total.  It seems like

June 27:

I gave the three full samples an extra two minutes in the PT770.  I want to make sure the Cr is completely cleared before I try my finishing recipe on the Oxford 100.

Yesterday, here is likely what I observed.  50 nm of Cr etched, 1.65 um of SiN etched, and probably ~100 nm of resist etched.  While I don’t need to worry about selectivity, assuming the book is right that resist has a selectivity of 4.5, that means resist got me through 450 nm.  So Cr got me through about 1 um.  So 50 nm to 1 um gives me 20:1.  This also tells me that my etch rate of SiN is 194 nm per minute.  So if I want to over etch a bit, say go to 3.15 um, this means I should etch for 16 mins.  We will make it 16.5 minutes just to be safe.

After Cr etch, I did notice that there seemed to be some residual Cr left in the trenches.  I did not confirm this, but the optical microscope seemed to show it.  After doing P7, I measured sidewall of 3050 nm, so about 3um.  I probably did not clear, but this depends on how much Cr is left.  For once, the Filmetrics was not useless.  The best fit I got was 50%, and the machine gave me 1400 nm of SiO2 and no SiN.  This would seem to imply that I cleared.  Under the microscope, I saw a lot of dust in the open areas (no surprise there).  The color definitely looked different in the stripe vs non stripe areas.  The focal plane was also slightly off.  This seems to imply that I did not clear in the trenches.

After looking under SEM, we etched through 2.3 um in 16.5 mins.  That gives etch rate of 140 nm / min, which is quite a bit lower than 194 nm per min.  We saw 512 nm remaining, so that means we should etch for an additional 3.65 mins, but I say make that 4.  So let’s do a 22 minute etch just to be safe.  Lastly, we observed 348 nm of Cr remaining.  This means Cr etches at a rate of 6 nm per minute.  From before, we saw 50 nm gone in 8.5 mins, which would imply an etch rate there of 6 nm/min.  That rate has been reproduced, and since we over etched a bit on our last sample, I believe this is quite accurate.  Resist is not doing much.

There are two explanations for this result:

1. There was some Cr left in the trenches.  This is somewhat supported by the fact that the trenches did not quite look clear, though I must admit, given previous etch rates, should not be the case.  Another data point in support of a thinner Cr mask, to make clearing easier.
2. Etch rate is not stable.  The machine is just back up, or I did not have enough cool grease, or the chip got a lot hotter as time went on, lowering etch rate.

Along with testing our new sample, I am also going to take a cross section of a prepped sample to look for Cr where it should not be.  This will at least give me my rate.  After all, given previous findings, even a small amount of Cr can really do damage to my process (given the etch time of Cr).

June 28:

We are going to try thinner Cr masks to get things working.  I also think it would be a good idea to do our etches in two steps, with a clean and seasoning in the middle.  These two changes should make everything better.  We are running the sputtering machine for 2420 seconds, which gives a mask thickness of 215 nm.  We don’t have a test sample, but this result was shown earlier.  We are using pressure of 7 mTorr.  We have 4 chips going.  I say we develop 2 of these chips and quickly etch them.  If we assume we etch Cr at 22.5 nm per minute, 10 mins should be more than enough.  That being said, I am taking no chances.  We etch for 13 minutes, just to make sure we clear.

I still say we use the thicker photoresist mask, as it seems to be working well.  That being said, we should do a minute and a half oxygen descum.

Here, in total, is what we are going today:

1. 2420 Cr sputter
2. Vapor prime
3. 2000-8000-45 1805 resist spin
4. 1 minute soft bake
5. Use of DWL66 with power of 60
6. 1 minute development in AZ720
7. 10 minute oxygen plasma clean on the Oxford 81 and then 1:30 oxygen descum (mild descum)
8. 10 minute season on the PT770 and then a 13.5 minute etch
9. Two 8.5 minute etches on the Oxford 100.  In the etch, do a 10 minute oxygen clean and then a 5 minute season. (Edit, three 5 minute runs, with zygo in between

This will hopefully clear with the pattern we want.  While I could use a faster spin on, I don’t think I need to.  We already know the current system works, and I would lose 100 nm.  That would cause me to be cutting it close once more, which I have no desire to do.  We will likely be etching around 325 nm of resist, so if we start with 430 nm of resist, I don’t want to cut this close.

After 1:30 descum, we observed a sidewall height of 500.  This is greater than I remember

After first etch, I saw Zygo bottom of 0.637 um and Zygo top of 0.27 um.  This means it etched 900 nm.  That gives etch rate of 181 nm per min.  That is much higher than what I saw on the longer samples, and more in line with what I saw earlier with a 194 nm / min etch rate.  I am starting to think that I did clear Cr on these samples.  The microscope does not help, but the results are consistent.  If I had not cleared Cr, then I would not have got this far down.  Granted 200 nm of this is likely Cr, so that actually put my rate closer to 140.  That is the slow rate rate, which seems, unfortunately, to still dominate.  I did see resist left over, so I likely have all my Cr left.  This does leave the possibility that a bit of Cr was remaining.  Lets see what the next five gives us:

Etch rate 1: 140 nm/min.  Etch depth (excluding 200 nm of Cr): 700 um

After second etch, Zygo said top was 0.38 um and bottom was - 1.4 um.  That means there was a total trench depth of 1.7 um.  If we get rid of the likely 150 nm of cr remaining, we likely have 1.55 um of SiN removed.  This means we etched 850 nm.  This gives etch rate of 170 nm per minute.  We will likely want to run two more five minute processes.  20 Minutes total.  P7 gives side wall of 1.8 um.  If we think back a little, recall that 8.5 gave us 1.9 with 400 of Cr, so 1.5 really.  This rate is 176.  Basically, assume rate of 170 nm/min (except the first run.  I should also note that you can open Oxford 100 chamber at 126 seconds to speed things up

Etch rate 2: 170 nm/min Etch depth (excluding 150 nm of Cr): 850 um

After third etch, P7 gives sidewall of 2.56 um.  Zygo claims the top is 0.27 um.  Bottom it claims is -1.99 um.   On the side, it claims top is 1.3 um and bottom is -0.85 um.  It also claims sidewall of 2.5.  So it seems that the Zygo is accurate (it also visually looked accurate, though we are approaching its limit).  We basically have a trench that is 2.27 um deep.  If we assume that 100 nm of that is Cr, then we etched 2.17 um of SiN.  Previously, we etched 1.55 um of Cr, so this third etch got rid of 602 nm of SiN.  Not exactly the most speedy.  We still have 800 nm of SiN we would like to get through.  I say we do 9 minute final etch to punch through the bottom.  We are trying to account for the likely drop in etch rate as we go.  Small chance that we are getting a bit greedy, but whatever.

Etch rate 3: 124 nm / min Etch depth (excluding 100 nm of Cr): 602 um.

Note for etch four (only seasoned for 2 minutes instead of 5).  P7 gives side wall of 3.8 um.  Zygo seems accurate near edge.  Top is 0.7 um, bottom is -2.23 um.  This gives etch depth of 2.97.  While I am not totally sure whether the side is accurate, it did seem to show the flat regions with an extra 1um etched.  This means, if I eliminate 100 nm of Cr, I have 2.87 nm of SiN etched.  This is technically enough, though not quite as much as I would have liked.  I would like to run another 5 minutes etching.  We etched, in this go, 600 nm of SiN.  Etch time of 9 mins.

Etch rate 4: 66.6 nm/min Etch depth (excluding 100 nm of Cr) 600 um.

Note for etch five (only seasoned for 2 minutes instead of 5).

July 5:

Some comments about LPCVD.  First, Phil is impossible to get ahold of.  Yes, he is away and all, but really quite challenging.  No one else is this hard.

Aaron recommends using three baffle wafers on each side.  This is counter to Phil’s recommendation of 1.  As it would happen, if you increase the ratio of silicon to nitrogen flowing into the chamber, you will get a higher index.  The plots stop with an index of 2.5 with a ratio of 10.  It seems that we start to get negative stress (meaning in it wants to contract instead of expand).  The magnitude of stress is still a lot lower than that of stoichiometric SiN (800 to -200) but still.  It seems that annealing makes stress more negative, so it may increase our stress.  This could be an issue if we want to do annealing to reduce loss.

For etching, I am going to do a 6 minute etch.  This will bring total etching time to 30 minutes.  Since last etch gave me a depth of 2.97, and I am ok over etching by a few hundred um, I would say this is best.  I only want to etch, presumably, another 300 um.  That will confirm that I cleared (3.2 is target depth, as it would confirm that I am totally through even if Cr is the same).  Given the dropping rate, this seems right to me.  Granted, Cr is not still 200 nm thick, but I want to be safe rather than sorry.

For this fifth etch, I am going to season for 5 minutes, and then do 6 minute etch.  All my other samples are left in storage.

I was unable to characterize my fifth etch.  The trenches are too deep for Zygo.  I am going to do one last 5 minute etch just to be safe.  I can always eliminate etch time later.  The only interesting observation is that one of the areas with the large rectangles is a yellow color while the other is a lea color.  I suspect I broke through the SiO2 layer.

Some physical observations after this last etch.  The blue area is gone. Press is lost at 128 seconds remaining

July 6:

After looking under SEM, we etched a distance of 4.3 um.  We want a micron fewer.  We also etched an additional 400 nm on the large outside area.  Assume we have 1 um of SiO2 and 3.1 um of SiN.  We also had 150 nm of Cr remaining.  If we etched for 35 minutes with an etch rate of 6 nm/min, that would mean we started with closer to 350 nm of Cr.  It seems Cr etch rate also decreases with time.  My guess is 26 minutes (Because I am paranoid) should get us through.  This is because we observed sidewalk of 3.8 last time with 24, and there seems to be, at max, a 500 nm difference.  I increased it a bit because Zygo showed 2.97 um etch depth, which is a tad short.  Granted, that could be wrong, but who knows.  The risk we are running is that the extra 1.1 um was not all etched in the final 10 minutes last time.  This would mean the etch rate went down more than we expected.  I also know the SiO2 breaks around 30, so 26 should be fine.  So I say we do 6:30 minute etch with 5 minute season four times.  This also means 11:30 minute cleans.  I just don’t think Zygo gave us something accurate for the fourth etch, as the rate decreased too much.  What kinds cool about looking at the long etch SEM pictures is that you can see where each etch stopped by the sidewalls.  Clearly the final etch did not go super far, but the 6 minute etch made decent headway.  It seems that the 24 minutes before got very very close.  While I think we are going to clear, I say we make the last leg 7 minutes just to make sure.  I don’t think we are going to clear near the edges given that 30 minutes is when we observed that.  We can always look at color too.

After first etch, we saw sidewall with P7 of 1.35 um.  If we assume 200 nm of that is Cr, then we etched 1.15 um of SiN.  That gives etch rate of 176 nm/min.  This is in line with what we normally see.  Looking back, it also seems that I did not quite measure the thickness of the SiO2 properly.  That means I have a bit extra.  It is weird though that I had arcing behavior below it.  This means we etch slightly faster than last time.

After second etch, we saw sidewall of 2.4 um.  If we assume 200 nm of that is Cr, then we etched abbot 1.1 um of SiN.  This is super consistent.  This means we should see depth of 4.4 when done.  This is a tad high in my opinion.  But if we subtract the likely 200 nm of Cr left, then we still have 4.2, which makes sense given the depth last time.  This feels fine to me.  This puts me right where I want to be.  If anything we can reduce last etch by 30 seconds.  I am just trying to trust  my previous measurements.

After third etch, we saw sidewall of 3.4 nm.  After Zygo,

For LPCVD today, we would ideally like two wafers with oxide and two without oxide.  I put in two wafers which filmetrics said had 1 um of oxide (which are facing toward cleanroom), a double polished one (one what conductive), and then a very conductive one since polished wafer (furthest from exit).  I used percentages of 86 for silicon and 5 for nitrogen.  Everything else was left the same.  I put them in the tube for 200 mins.  Phil guessed that the deposition rate is 20-23 angstroms per minutes, so 400 nm on low end, and 4600 nm on the high end.  We likely don’t have to worry about stress.  If 800 stress breaks at 400 nm, and we are dealing with 200 stress, we are fine.  Same stress as a thermal oxide.  We are interested in the following values:

Index of refraction at light of lambda = 1500nm and 1064 nm, Loss, stress, delta_n, breakdown of the film.

We got our films out of the LPCVD.  No visible cracks or anything of the sort.  Using filmetrics, I saw a thickness of ~330 with a goodness of fit of 80%.  On the Woollam, I saw a thickness of 340.  The plus and minuses were all within a small range.  It gave an index of 2.513, or more precisely, using the Cauchy equation, A = 2.513, B = 0.08203, C=0.00335.

After fourth etch, blue regions on big sample show height of 4.5 um. Light regions show depth of 4.3 um.

On other sample, red is height of 4000.

Harsh grey is 4300. Blue means over etch

Middle is 26 min etch, right is nitride, left is red etch

July 10:

It seems the two step etch worked best.  Past of this reason is that the sidewalls look the best.  It seems that whatever polymer coats the sidewall to preserve an isotropic etch goes away after multiple etches.  While it is a bit hard to tell exactly how deep we got (the dust left in these old samples is dreadfully annoying), it seems, at max, we etched 3.3 um.  Considered that our photoconductors are somewhere between 2.9 and 3 um thick, this seems pretty good.  On the side, it etches a distance of 3.9 um.  This is pretty much consistent with what profilometry says.  This means, for this etching technique, there is 600 nm of distance between first and final.  Not unheard of.  We will have 300 nm of SiO2 left, which is fine.  For four goes of 6:30, we over etch on the wide (though not in the middle).  We etched 3.9 um deep in the middle, and 4.5 on the outside.  Once more, a 600 nm distance difference, so the other result makes sense.  This does show etch saturation though.

It seems the red sample was the one that I previously etched for a shorter period of time.  I etched that one for 16.5 minutes. I had ~500 nm left in trenches and 0 left (very little over etch) on the sides.  That means I etched for 23 minutes.  I believe 22.5 should do.  Let’s do a 16.5 minutes etch, stop, then a 6 minute etch.  What is intersection is this also gives us the etch rate in the trenches at this point.  We etched ~ another 800 nm, which means we have an etch rate of 123 nm / minute.  While it would be nice if I could do the “soft” landing recipe, I just don’t think it’s worth it.  Our twenty minutes etch is the one that shows etch saturation.  I also think it would be good to blow down samples between etches.  We did five minute seasons in the past, so we should do that again.

For PECVD, we had loss of 4.66.  Loss of 11.9 first.  24.5 was second.  The Metricon said we should expect a loss of ~20.  This makes me believe we did get coupling, but only for very short chips.  This also makes me believe that the Metricon is accurate.  Our next batch will be a little less silicon rich, and a lot more thick.  At this point, I am most concerned about suing 1550 nm light (which silicon does not absorb) and making sure we have small radiation loss.  Given the thickness of our oxides (1um) we really want thicker cores for the moment.

July 12:

It seems, from chat GPT and a few papers online, the breakdown voltage of silicon dioxide is somewhere between 400 to 700 V / um.  If we use 1000 V (as I think the high voltage thing does), then we need the higher end of this to get our trenches not to breakdown.  Granted, I am assuming worst case scenario here, which I am not sure if the actual case, but let’s run with it.  Our trenches are 1.5 um wide, so we want at least 666 V/um.  It seems defect centers are the main avenue for breakdown, so we would like to limit those.  This means we don’t have a lot of room to wiggle around here.  I suspect that evaporated oxide won’t do because it is to oxygen poor.  I am not certain what other nonlinearities might come into play.  Do thicker films have larger breakdowns than thinner ones? It also seems that the substrate oxides were grown on matters, though this seems to apply for dry and wet oxides, not deposited oxides.

July 13:

Today, I am etching my remaining samples.  This means a 5 minute season, 16.5 minute etch, 21.5 minute clean, 5 minute season, 6 minute (I am shaving off 30 seconds) etch, and 11 minute clean.  We should see the side areas have a depth of 4000 nm (possibly a tad less) with a yellow or red color.  The resist on 225 nm of Cr with 13.5 minute etch on the PT770 is orange.  After descum it should have a brighter green with small red lines near the top.

Also, if you recall, I observed in the past that the two open areas of my chips sometimes had different colors.  I believe this is a result of putting down too much cool grease, which causes one side to be lifted.  I guess that would affect the etch rate.  The effect is marginal in a minute or two, but not over a longer period of time (~100 nm is my guess).

Blue turquoise region is 3.8 um.  I was not able to look at the other side.  I will say this, one side was more dark blue, the other turquoise.  This was evident on all the chips.  I still think my previous theory around the cool grease is the most likely to be right.

Regarding LPCVD, I know 84% DCS gives 126 scms, and 11% NH3 gives 22 Scms.  This means percentage of Ammonia gives twice that number of scms, and percentage of DCS gives 1.5 times as means scms.  If we think back to our recipe, we used 86 DCS, which means 129 scms, and 5 scms of NH3, which means 10 scms of ammonia.  This means we had a gas ratio closer to thirteen.  Tmrw, we are using 118.5 DCS, and 14 ammonia.  This gives ratio of 8.5, which predicts index around 2.35.  Remember you can’t use decimal place percentage points.

July 14:

I loaded a full 1 um thermal oxide, 1/2 5 um thermal oxide, and 2 side polished full conductive wafer.  The useable side is facing away from the cleanroom (into the furnace) and the 1 um oxide is closest to the cleanroom, followed by 5 um oxide, followed by 2 polished.  There are two baffle wafers on each side.  I ran 79 DGS and 7 NH3 for 396 minutes.  This should give us an index of 2.35 at 633 and ~550 nm thick film.  These were grown on E4.

Green regions from yesterday’s etch have height of 3.85 um.  The sidewall looks decent, but it seems to go down over the force of a few microns.  Granted, considering we are dealing with the large open areas, the smaller ones probably have better sidewalls.  The turquoise blue areas have depth of 3.79 um.  If there is 150 nm of Cr remaining, that means 3.64 um of Silicon stuff gone.  So height difference of 600 nm is what we expect, so this is good.  Funny how only 50 extra nm can cause such a notable height difference.  Brighter (really closer to red on visible spectrum) the color, deeper the trench (less stuff remaining)

For PECVD, we should use the CNF’s recipe.  It gives better conformality and is a generally higher quality fill.  Jeremy says it deposits at 47 nm/min, which means 20 minutes should give a micron.  We also says the deposition rate speeds up as you put more down.  We clean for deposition time plus ten minutes.  I am doing 5 minute seasons.  I am going to do the following order four times.

Season five minutes, run with samples for 20 minutes, clean with inner and outer at 25 minutes each.  We are also putting in Martin’s BTO sample for 2 um (so half the process time).  Recall to blow stuff off before you put in (blow lightly) and put in the center of the big wafer that is provided for you.

Edit, first run we season for five minutes, but on future runs lets season for two.  Five in not necessary.

For LPCVD, I did 396 min at 79/7. We got 770 nm out

July 17:

The TEOS deposition did not work nearly as well as I (or for that matter any of the CNF staff) thought it would.  Only 1.026 um was deposited, which means the deposition rate is about 25.5.  Almost half that Jeremy claimed it would be.  The trenches were not as deep as I would expect (only 2.6 um) but let’s assume we etched to at least 3.5 (which is what we would expect from this etch).  Official measurement shows closer to 866 nm of oxide down, though other areas show ~1 um.  I will admit, I have a hard time differentiating the oxide from the deposition months ago and that from today.  Keep in mind I used the older sample that I etched 20 mins on first, but that should not matter (as the trenches were the same depth due to etch saturation).  The side walls had about 530 nm of oxide on them, which means, for a 1.35 um wide trench, we probably only have 200 nm left before the thing pinches.  More concerning is that the deposition rate seems to vary from trench to trench.  This could be because of the residual effects from dust.  That make be the cause, though I find it a bit hard to believe.

Here is what google shows to be the best way of doing things:  It seems that this is very possible.  I have seen images of higher aspect ratios done in 2002.  Something that was mentioned was an oxide liner.  I think In may case, it would be a very good idea to use an ALD layer that is about 10 nm thick before the TEOS deposition.  Images online seem to show depositions that one can get more deposited in one direction of mostly in the trench.  These people seem to use Ozone and Teos instead of O2 and TEOS.  There is something called sub atmospherical chemical vapor deposition.  SACVD.  This seems to be mostly descriptive of the pressure, as it was still a PECVD process. It really seems that adding Ozone is key.

July 18:

Firstly, when looking at SEM images of TEOS depositions, you should always cleave far away from any exposed edges.  Elsewise, you will think something is wrong when there is nothing wrong.  TEOS (using the CNF recipe) does work and deposits at a rate of 1 um per 20 mins in the trench and 1 um per 40 mins outside of the trench.  While the SEM image is not perfect, I am concerned that I etched the SIN for too short of a time.  If you recall, I did 22.5 minutes of etching last time.  I think the extra half minute that I shaved off is important, so in the future, let’s do 16.5 mins of etching with 6.5 mins after that.  Looking at the SEM images, it is not clear to me if I actually cleared the SIN perfectly, and the extra half minute will not kill anyone.  If anything, we can add an extra 45 seconds and I don’t think that should be a big deal.

Also, for etching Cr in the liquid etchant to avoid polishing it off, but it in Cr etchant for 12 minutes.  It should look red when the etch is done (not hard to see).  Also, when cleaning baffle wafers, use one of the half wafer boxes and put your wafers at the end.  Leave them in a shallow HF mixture for 3-4 hours.  At the end, the HF should easily slide off instead of sticking to the wafers.  Make sure to only use Teflon containers, and NOT glass.  Rinse everything multiple times, and then put your rinsed wafers in a new box so you can put them in the spin drying machines.

Aug 1:

Instead of 5 minute seasons for the letter oxide, here is what I am doing.  3 min season, 2 quarter wafers for 6:30, 10 min clean, repeat.

Aug 2:

The v3 recipe broke down at 4 volts peak to peak.  We did not push the v5 recipe past 2 volts.  I would imagine both should then be operated at 3 vpp.  The v5 recipe generally showed little response.  Either it was moving super fast, or not much at all.  We did both experiments at an exposure time of 2000 us.  For v3, we did see a response at both higher and lower frequencies.  I did not noticed much of a difference.  For higher frequencies at v5, I did notice that the image seemed to blur.  It would have been nice if voltage had been pushed up more, as we then could have seen whether the blurred areas grew or not.

We pushed the v5 recipe as high as 200 Hz.  I don’t recall how large we made the frequency on the v3 chips.  Keep in mind one of the v3 chips is broken and can no longer go above 2 vpp.

Aug 29:

With the filters at 50% (by accident) on the DWL, I get trenches that were a little under 4 um wide.  My point is to say we have to make sure we are working with 10% filter in the future.  I am still doing a 15 minute heat TEOS run just to see what happens.  We will see how long I am awake to continue the fight with this stuff, but my hope is to get two rounds of 20 minutes done.  In the machine, I presently have one quarter wafer of nova 0.01 Ohm*cm wafer, a small part of an edge electrode device, and two of the large trench pieces.  We are putting a shadow region on the edge electrode device.

When I do the evaporator, I am doing 10 nm of ti, 5 nm of au, on a PECVD sio2 tantala chip with 1 cm features and on the quarter wafer to test breakdown and delta_n.

Sept 21:

After doing the mechanical polishing on the chip with no Chrome, we observed a thickness of 1.536 um.  Before polishing, we observed a thickness of 1.631 um.  We polished the sample for 5:30 minutes with an applied pressure of 0.04 and a speed of 50 rpm with oscillations on.  This means we get about 100 nm in 5:30 minutes.  We should definitely do mechanical polishing with Cr, as that would make it super easy to see when things start to peel off.  We will likely need to do mechanical polishing for an hour.

For testing new photoconductors, here is the ideal plan:  Lets do alpha = 2, alpha = 4, alpha = 6, alpha = 8, and potentially alpha = 10.  I am not sure if we should go with less of more silicon.  Intervals of two seems pretty good to get a solid sense of how things vary.  For thickness, I was thinking 1 um, but I would like to get the collective take on this.  From Martin’s Data, I get the following:

50/5 after 6:30 gives 470 nm (72 nm/min).  40/10 after 6:30 gives 430 nm (66.15), 48/8 gives 68 nm/min.

Sept 23:

Wd did alpha 2 (40/20), alpha 4 (40/10), alpha 6 (48/8), alpha 8 (48/6), alpha 10 (50/5) for 6:30 each.  I seasoned for two minutes before and did 15 minute clean in between.

For the tantalum wafer, we will deposit for 5:33.

Sept 25:

Final_3 is top period of 2 um.  Final_4 has the correction factor reduced to 300 nm instead of 500.  Roberto did not believe it was the height of the pattern that was causing the issues.  We will also need the fin wafers (and possibly the carrier beneath, to do edge alignment, which is highly annoying.

Sept 29:

In the past, we noticed that 3500 rpm gives 430 nm of resist after development.  The current resist gives about 600 after development.  Given that we are going to be taking a good bit of resist off during descum (and the fact that descum does not really etch oxide), I say we still with our current resist recipe and etch away any unwanted resist in the 81 after using the same descum recipe as normal