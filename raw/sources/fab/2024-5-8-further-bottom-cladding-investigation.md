---
type: craft-export
title: "2024-5-8 further bottom cladding investigation"
craft_document_id: 3F4A3340-3A8D-425E-B673-EE0BEC97018D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-5-8 further bottom cladding investigation
The point of this document is to, at first, think through some possible long derm solutions for my bottom cladding.  We really want a film with a conductivity that is around (or above) 1e-8 for a large range of field (including in the lower field limit).  We also want an index below 2.2.  For loss, we really want around 1 dB/cm (as measured in the lab).  We have currently done a lot of testing on doped oxynitride recipes.  The issue right now is we seem to need around 160 sccms of N2O to get a useable optical loss.  150 sccms gives us a loss of 5 dB/cm, and is not consistent at lighting at 5W anyway.  The indexes are good though, so we can do some stuff that might raise the index if needed.

Here are some ideas on how we can make these films work:

1. A light step.  Light at 6W for 10 seconds, and then move to 5W.
2. Reduce (or increase) B2H6 flow.  It might be possible that increasing this flow could make our films more conductive, or reducing this flow might make it easier to light at 5W without sacrificing conductivity.  This gas also may be a prime source of loss.
3. Mess around a bit with tempurature.  We know tempurature does not make lighting the plasma easier, but it may help increase conductivity.  I am not super confident in this one.

Additionally, we want to ask Jeremy the following quesitons during training today:

1. Can we put LN into the oxford 100 or Oxford 81?  Would he know if we can put it into the PT 770? (for wavelength division multiplexing stuff)
2. How do I add a light step to my doped oxynitride process?
3. Should I get consistent conductivities for my doped oxynitrides.  I am worried about variablitiy across the wafer and whether each run will give the same thing.  Show him the data below if needed

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-001.png)

The above data shows conductivity inconsistency, which worries me for the future

After Metricon training, I had a productive chat with Jeremy.  He mentioned that there should be a way to add a light step (right click, add).  Just make sure to fill in all the values for these new steps).  Additionally, we will need to link the step to the follwoing step.  This means we don’t want the power to turn off, as this defeats the purpose of a light step.  There is a purple button we need to press to link steps to one another.  Giving our history with lighting, I say we light with 6W.

Jeremy seems concerned that we are not actually being given the read power.  I am not sure I agree, as the light has been pretty sensistive to the power we applied

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-002.jpeg)

Jeremy also mentioned another way to measure conductivity (pictured above).  Hit ohm 4. Then multiply by geometric factor to get resistivity.  This does not seem like a bad way to do things, but the issue is we can’t scale the amount of field we are applying.  There is a way to code this voltage source, which might be worth trying over the summer.  Jeremy seems to think that we are getting effects from the type of electrode we use.  That is possible, though I believe it is unlikely.  Those effects really should not dimensiont our resistance.  The only possible reason I might believe this is we haev bad adhesion, so those effects dominate at low field.

Lastly, Jeremy said LN (even buried) would NOT be allowed in the oxford 81 or 100.  Apparently LN is class 5.  There is only one etcher we can use for this.  We can use Cr etching for the Cr mask.

Anyway, I say our first priority is to try processes with light steps.  We will light with 7W and deposit with 5W.  I also want to try vanilla B7 with 5W, as that recipe is not totally useless and I want to know its conductivity.  That will probably be the last one we try.  Below are our recipes

B14:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 425 sccms (Notice the change down)

Power: 5W

N2O flow: 135 sccms

Light: 7W



B12:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 425 sccms (Notice the change down)

Power: 5W

N2O flow: 150 sccms

Light: 7W



B13:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 425 sccms (Notice the change down)

Power: 5W

N2O flow: 160 sccms

Light: 7W



If none of this works, I say we try to scan the B2H6 flow.  We should try with 170 sccms (to see if more B2H6 helps), 133 (baseline), and 100 (to see if it reduces conductivity).  I would run these off a B10 seed recipe.

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-003.jpeg)

Checking that we are indeed using silicon.

Here is generally what our recipe looks like before season B12

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-004.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-006.jpeg)

During run

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/7DFE8DFF-6AC9-422A-BFDF-5271DEFBCCC5_2/Pfymda9BadNf2J6ZEONzy2lLrogOykhiMyp0PlkoKMgz/Video%20from%20Library.mov)

Gas stays on!!

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-007.jpeg)

I checked as well that it was still on at the end. 

After season

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-008.jpeg)

Nice and blue. Let’s proceed. I will deposit everything for 5 mins. It could be possible that the slightly elevated temp during season might matter, but I doubt it. 

During beginning of deposition:

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/1A27BD21-C73B-4664-ABC4-ACB68FF55598_2/BXhVS65rKPle4j44TY2JDKtyxiZnlx8IVVEtyd6guP4z/Video%20from%20Library.mov)

It stays on

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-009.jpeg)

At the end, 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-010.jpeg)

Still lit. I think we might have a path forward here. 

After deposition

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-011.jpeg)

B14 season

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-014.jpeg)

During season

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/AEC0E8F9-0E6A-421E-8D7B-957DB91F3F37_2/xyigJVB0uvXojNDqQaqvuOICmUvTFTi7S1FXUcxoFoUz/Video%20from%20Library.mov)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-015.jpeg)

Lit as expected (as we are using lower N2O flow)

After season

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-016.jpeg)

Nice and blue, let’s proceed

During deposition 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-018.jpeg)

At end of deposition 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-019.jpeg)

It stays lit. After deposition

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-020.jpeg)

Now B13 (highest among of N2O)

Before season

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-022.jpeg)

During season

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/0C21C7B7-116D-4B5F-8F0F-73145800084B_2/YiMwoziynhVD2UAjO2JbR1LFq8B1PX26KaZMV9sEvtEz/Video%20from%20Library.mov)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-023.jpeg)

Lit again. We had nice blue water after season

During deposition 

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/F7B062CA-536E-49B7-9BA1-DF37D4C4852D_2/E4uF7kN3MPpTLnvv9s8HjAUYyiPah6nCUS3yIHgsNcoz/Video%20from%20Library.mov)

You can also see it get dimmer, which is cool

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-024.jpeg)

At end of deposition 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-025.jpeg)

It stays lit

After deposition

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-026.jpeg)

Now onto ellipsometer

B12

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-028.jpeg)

B13

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-029.jpeg)

For B14 too.  Just emailed Alan to see if there is a solution, as this is very annoying.

 Let’s evaporate 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-030.jpeg)

Life is good. 

For Ti (nice and low power too)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-031.jpeg)

Onto Au (adjusting prog parameters)

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-032.jpeg)

After evaporating 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-033.jpeg)

Same geometry as the box implies 

![Photo from Library.jpeg](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-034.jpeg)

The chips are now back in the lab.  Lets do some conductivity measurments

Reference:

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-035.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-036.png)

B12 (I am saying all of our chips are 1.3 cm by 1.3 cm, and 224 nm thick)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-037.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-038.png)

B13 (1cm by 1cm):

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-039.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-040.png)

B14 (1.3 by 1.3)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-041.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-042.png)

Now lets check to see how consistent these results are by doing one of the larger pads.\

B12 2.0 (1.4 cm by 2.3 cm)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-043.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-044.png)

Those last points are real.  I suspect breakdown.  This is fairly consistent with before.

B13 2.0 (assuming same size as above)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-045.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-046.png)

B14 2.0 (2cm by 1cm)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-047.png)

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-048.png)

Below are the nice graphs:

The first take of data

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-049.png)

Second take of data

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-050.png)

Pretty much the same.  At least consistent on-chip results.  Lets compare some of our B10 recipe results

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-051.png)

So it seems that we get a lot of variablity between depositions when we use N20 = 150 (though this week’s depositions to look good).

The graph below shows what we should expect for other 5W depositions

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-052.png)

FWIW, it looks like the conductivity does follow a trend at 5W when things work right.  The key question here is why is it that the 135 sccm and 160 sccm films not follow this trend.  I suspect the PECVD was not really applying 5W.  Maybe we should light at 6W, and deposit at 4W.  It is objective that these films were still much more conductive than their 6W counterparts.  Even the films that were exponential at low field were still much more conductive.  I am also happy that each pad gave roughly the same result, showing some consistency across the wafer.

![Image.png](../../assets/fab/2024-5-8-further-bottom-cladding-investigation-053.png)

Above is a direct comparison of 5W and 6W films.  What is intereting in this comparison is that the 6W films are all linear resistors.  More resistive than their 5W companions in the high field (mind you) but for some reason they are not linear.  I just don’t know why they are not linear.

Going forward, there are two possible paths for me to try:

1. Doing 5 second light at 6W, and then depositing at 4W.  Hopefully the improved conductivity will make up for nonlinear effects
2. Try messing around with doping.  It is possible that the dopants are not doing much to help us conductivity wise, and instead might be hurting our optical loss.  If we can get low loss for lower N2O flow, that would be a win.  In that case, I would try to make a film with no doping and 200 sccms of doping and see what the result is.

As a final, desperate, resort, we could try seeing what the results are for lots of trials.  This seems like a lot of time and effrot to learn minimal amounts, so I say we avoid it.