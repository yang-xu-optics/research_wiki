---
type: craft-export
title: "2023-11-1 etching oxide"
craft_document_id: 999329CA-EE5A-4863-9151-FD970E2C4052
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2023-11-1 etching oxide
Start

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-001.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-002.jpeg)

I would like 3 um of oxide in case I over etch.  I used acetone and ipa to clean the wafer, and will deposit 1.5 um more oxide on the wafer.  I pre-clean the PECVD for 10 mins, season at high rate for 2 mins, run the machine for 6:30 mins, and clean for 18:30 mins after.



![Image.heic](../../assets/fab/2023-11-1-etching-oxide-003.heic)

![Image.heic](../../assets/fab/2023-11-1-etching-oxide-004.heic)

These are the characterizations of etch rates from the PECVD.  Most likely I will want to use the “CH2F2/high He Oxide etch” recipe.  This is the same chemistry I use for etching SRN, and I believe in the past that it does not murder photoresist.  I never clocked the exact rate, but I know that after a 8:30 min etch photoresist that was spun at 2000 rpm, descum for 90 seconds, and PT770 Cr etched for 13:30 mins was not totally gone.  That means the characterized selectivity is probably a bit low.  My guess is 300 nm of resist took that long to etch.  In theory a thick photoresist should get the job done (and save the money and effort of Cr sputtering and etching).  If we have ~500 nm of resist at the start, we should be able to get 2um done and burn the resist off in an 81 or 82.  The 170 nm/min rate for nitirde I found to be accurate for larger regions.  This dropped off as I got deeper or with narrower trenches.  The guessed oxide rate is 155 nm/min.  I would trust this.  Therefore, if I want 2um deep, I want 13 mins.  To make sure I get through, lets do 16 mins.  



The trouble with 16 mins is I know this is what I do with Cr, so at the end of the day, a Cr layer probably will not hurt.  I don’t need a lot (probably 100 nm will do).  Better safe than sorry I suppose.  



I noticed the wafer had a few bits of dust on it when I took it out after 6:30 dep.  While they did blow off, I am a tad worried there might have been some flakling from the top of the chamber.  8:30 total mins of deposition is certainly a bit on the high end.

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-005.jpeg)

We have plenty of oxide

After developing 

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-006.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-009.jpeg)

We will want to descum for extra long (given that we are not etching for very long anyway). I say descum for 2 mins



I have decided on a 2 min descum to make sure I clear those trenches.  I will also etch in the pt770 for 8:30 mins (as I normally over etch by 3.5 mins anyway



![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-011.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-012.jpeg)

Since descuming did not seem to get rid of as much photoresist as I would like (and I am worried much more desucming will ruin my mask, I am going to etch for 10 mins in the PT770 and do a quick wet etch (~30 seconds) at the end just to make sure I clear.  I will confirm this step once I see what things look like under the microscope.  I would be suprised if I burn through the mask as it has made it to 20 min Pt770 etch before.  We will see.  A simple way of doing this is to look through the top of the machine and check as we go (stopping when I see the layer disappear).



In the future, this experiment should at least help at weight to the idea of using the 4mm head.  Maybe contact lithography is worth a try too once we know our pattern. If needed, we can also use a thinner resist (as we are not etched super deep into the Cr anyway).  Whenever we switch resist thicknesses however, we may need to recalibrate the dose.

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-013.jpeg)

There is likely a bit of Cr reminding

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-014.jpeg)

Let’s go forward with wet etch



After 25 seconds of wet etch, here is what we see



![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-016.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-017.jpeg)

I am going to leave the resist on (just in case I want to Cr etch again and to give me a little more room in the 100)

Before cleave

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-018.jpeg)

After cleave

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-019.jpeg)

In the past, I was able to etch through 2.3 um of Oxide in 16.5 mins

![Image.png](../../assets/fab/2023-11-1-etching-oxide-020.png)

While the etch rate of SRN is a bit nonconstant as I got deeper, this implies an average etch rate of 140nm/min as I went down. Oxide is characterized at 150 nm, while SRN at 170, so oxide will etch at 88% of the rate.  That means it will etch at 123 nm/min, so 16.5 mins will give me about 2 um.  I will etch for a little longer (17 mins) just in case (and because going a bit deeper does not hurt anyway).  I am going to etch two chips.  One will be used to characterize the etch in the SEM, and the other will be used to sputter some electrode on.



I ran a 10 minute oxygen clean and a 2 minute season of the CH2F2/high He Oxide etch

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-021.jpeg)

Took from top left of box

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-022.jpeg)



Zygo failed

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-023.jpeg)

After SEM, we saw almost perfect duty cycle and depth very close to what we wanted:



![Image.png](../../assets/fab/2023-11-1-etching-oxide-024.png)

![Image.png](../../assets/fab/2023-11-1-etching-oxide-025.png)

![Image.png](../../assets/fab/2023-11-1-etching-oxide-026.png)

![Image.png](../../assets/fab/2023-11-1-etching-oxide-027.png)

These images seem to infer the average etch rate for this run was 130, which is almost spot on to what we predicted.  This shows that the conversion I used for etch rates is usable. 



I am now going to etch ~1um deep into two other chips.  Below is an image from a previous SRN run that lasted for 8.5 mins.  This would claim an etch rate of 188.  Lets assume etch rate of 170, as that is what the book quotes and I have found to be true on other occasions.  Basically, the etch rate is what the book tells us.  That means, to go 1um down, we etch for 6.5 mins (assuming oxide etch rate is right).  I will try Zygo on this and see what I get.    I am going to clean for 10 mins and season for 2 before hand.  Hopefully all the resist comes off.  If not, it will need to be etched away.

![Image.png](../../assets/fab/2023-11-1-etching-oxide-028.png)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-029.jpeg)

After etching, the chips don’t quite look at shiny as I expect, probably meaning there is a small bit of resist left. I am going to descum for 45 seconds just to make sure

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-030.jpeg)

Descuming these for flat capacitor (5 mins)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-031.jpeg)

Otherwise, all the chips are now nice and shiny. 



To get even electrode sputtering, I am going to wet etch away my remaining Cr mask. After 5-10 mins in Cr etch and a quick acetone rinse, here is what I saw

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-032.jpeg)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-033.jpeg)

Almost same for both, which means I most likely got rid of Cr

Profile of 2um (2.5 um)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-034.jpeg)

Profile of 1um (950 nm)

![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-035.jpeg)

2 um on top left and 1 um on top right



![Photo from Library.jpeg](../../assets/fab/2023-11-1-etching-oxide-036.jpeg)

Usually there is a gap between large and small regions, so 2.5 um for 2um depth is not odd.  I probably underetched the first one.  it is more like 700 nm most likely.  Still fine for characterization.  