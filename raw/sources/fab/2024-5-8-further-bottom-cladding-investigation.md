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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/7851f068-b334-98cf-446a-ab83c08590b2/lrstnYZbyCGVs5txyYzlvK1YEnhcEgt9ytjDreiCDwkz/Image.png)

The above data shows conductivity inconsistency, which worries me for the future

After Metricon training, I had a productive chat with Jeremy.  He mentioned that there should be a way to add a light step (right click, add).  Just make sure to fill in all the values for these new steps).  Additionally, we will need to link the step to the follwoing step.  This means we don’t want the power to turn off, as this defeats the purpose of a light step.  There is a purple button we need to press to link steps to one another.  Giving our history with lighting, I say we light with 6W.

Jeremy seems concerned that we are not actually being given the read power.  I am not sure I agree, as the light has been pretty sensistive to the power we applied

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/2A97B3EB-C5F3-474B-8450-0BD09CAAF9AB_2/CEXZ28mqEaagYkxX2pTNW0PgoiW1RrV3psp1LAryxsQz/Photo%20from%20Library.jpeg)

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

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/1DB69A8D-A1DE-4FF8-8865-A01049F2B602_2/RU4GiixZq5Zkk3t2yPwXCTNb42107ahGTZAeKJdvMosz/Photo%20from%20Library.jpeg)

Checking that we are indeed using silicon.

Here is generally what our recipe looks like before season B12

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/1F91770D-BB11-4136-B03F-CC2093AF461D_2/2JzZKddRybph3FIJvehB6HxGC9WaPIXG9tsEVxN3bncz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/5444C5F5-BFBD-48D9-97B3-ECC2FF93A885_2/Scg9PiCpGXVvc6gSU0btfigZWgEzmTda9LTW4BDtOsAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/6219819E-1549-4D0B-85DB-AC9621780F91_2/Wvew2lmPGSvFLQc4glCPuY0bwayYu0DhAYTdbN91gfwz/Photo%20from%20Library.jpeg)

During run

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/7DFE8DFF-6AC9-422A-BFDF-5271DEFBCCC5_2/Pfymda9BadNf2J6ZEONzy2lLrogOykhiMyp0PlkoKMgz/Video%20from%20Library.mov)

Gas stays on!!

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/B6A7F281-E810-47DA-95E2-7B338C4F5A64_2/c9RtcKIjzxonlpSqCbfi0feAq1DaK818GFPKsGcbXnEz/Photo%20from%20Library.jpeg)

I checked as well that it was still on at the end. 

After season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/A320B9F3-8C77-4C1B-825A-3FBCAEF86A59_2/b68vArg40Qrrex4C1U82YMsQC1dgmyJkUMDbBHr52f8z/Photo%20from%20Library.jpeg)

Nice and blue. Let’s proceed. I will deposit everything for 5 mins. It could be possible that the slightly elevated temp during season might matter, but I doubt it. 

During beginning of deposition:

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/1A27BD21-C73B-4664-ABC4-ACB68FF55598_2/BXhVS65rKPle4j44TY2JDKtyxiZnlx8IVVEtyd6guP4z/Video%20from%20Library.mov)

It stays on

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/AC658588-EAA1-41D8-A906-A770DB72A4EE_2/z6IxHbc7vVokVCD5iyxhoDs0CzJzXgUqudUEhH55nq0z/Photo%20from%20Library.jpeg)

At the end, 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/AA0AB9C6-5B05-4C6C-8EEB-9E8E3719F8AC_2/LrlOnu6yHmi5jUnXqtLhjgperVRZ0f6eyEAc7G4Ty1cz/Photo%20from%20Library.jpeg)

Still lit. I think we might have a path forward here. 

After deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/41258896-F31D-4403-B0D0-032F3C6DC436_2/d43lLhJiiCE0BacMylTtsSgfK0cFwFTHScZw51uVwC0z/Photo%20from%20Library.jpeg)

B14 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/FF841687-232C-471D-A248-9EEED5F8E120_2/RtkByFRD8eNsyx5eO5uf0yCVNr2xenj2y3w1Iz6CGGwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/C01CFA1F-B72B-42ED-9053-4EACB4633774_2/jMQF1TDG9QIm52wtmsrYQodtCh7O6us6paiIcDAJCZMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/0AAFA4C9-B605-48A8-96CF-8EBABABB3EB4_2/NeyQ6JaQV4ZgOeOfWL3NclyImvMySp4djUp0p9DfcV0z/Photo%20from%20Library.jpeg)

During season

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/AEC0E8F9-0E6A-421E-8D7B-957DB91F3F37_2/xyigJVB0uvXojNDqQaqvuOICmUvTFTi7S1FXUcxoFoUz/Video%20from%20Library.mov)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/48A52A3C-9D09-4B4D-AB5A-EF62C51E90BC_2/n2d3HMjFs74jNwtdo91xSKqtz37dhV5tECxaBsApuiYz/Photo%20from%20Library.jpeg)

Lit as expected (as we are using lower N2O flow)

After season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/C3C58318-9170-4540-B65B-3AC26D119DC9_2/MpbMxdIEBtB0xt5OcycmBqIpkpwRRtHL3oO1u60elacz/Photo%20from%20Library.jpeg)

Nice and blue, let’s proceed

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/04B47203-E9EC-4F14-B1D2-C956433C6399_2/9J0MDfGGdI9x0FVPaZqZQm8xyLruye1qcLsDLgehWQMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/802DDFB5-8C22-4CC8-B3AC-48FD697617F8_2/BUaH9bFycJyI7zLbn07xugByIikyxxSMu24AA85sbcsz/Photo%20from%20Library.jpeg)

At end of deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/00A1E924-D690-45FF-8825-9F859201296C_2/PLvQD0fic7ulfkhx5iOfApH8u6sC9K87Ui4AttNfrSAz/Photo%20from%20Library.jpeg)

It stays lit. After deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/9D623459-62AA-4C07-BBAF-980EAF7B2261_2/WmS08BD2x24aGymOvqG2m1v4vZyGsWUoXljeAg8HbF4z/Photo%20from%20Library.jpeg)

Now B13 (highest among of N2O)

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/1FE7CAAC-B410-4EC8-A99F-1BEEF86B7932_2/8bfYwB9XgEruhYX7WP4ONqqHn7SgQx3zvQoPZLFDRnEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/688453A4-2749-4E2B-8157-118DDA6293CF_2/dx2DvtzzGCQgV00XAM80sqnlrQ73Sy9QgrNq6jt2uJUz/Photo%20from%20Library.jpeg)

During season

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/0C21C7B7-116D-4B5F-8F0F-73145800084B_2/YiMwoziynhVD2UAjO2JbR1LFq8B1PX26KaZMV9sEvtEz/Video%20from%20Library.mov)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/4ED28C58-B928-4F12-BF30-62D8F62CBB70_2/DcYtS65V9nn5NZmDMv4Po6j7GJ6pip9ODAqGxIIBKswz/Photo%20from%20Library.jpeg)

Lit again. We had nice blue water after season

During deposition 

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/F7B062CA-536E-49B7-9BA1-DF37D4C4852D_2/E4uF7kN3MPpTLnvv9s8HjAUYyiPah6nCUS3yIHgsNcoz/Video%20from%20Library.mov)

You can also see it get dimmer, which is cool

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/A3949FE8-7FB9-4227-85F3-4C813A4DCF80_2/exyqnXu6HF25uxDpJUAYr2dDmbuG3Nf4Fy6i1WabVakz/Photo%20from%20Library.jpeg)

At end of deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/DD9C33BB-51BD-4DD5-9C5C-5D847B63DDB1_2/99RBW6i5UxppCE7wy7WbUpcfWEswsG9y48DqMIoWwIQz/Photo%20from%20Library.jpeg)

It stays lit

After deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/96F6265B-5A03-4F53-AB5B-3F80D436FA4E_2/ya7vCSXglc8mEyBtz8A4WvOVMB4DShGMyzRyyDOoiUoz/Photo%20from%20Library.jpeg)

Now onto ellipsometer

B12

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/E0538719-93F8-4464-909B-3150B04A9776_2/tHauCKBk5CwLqQ1vZCwsyy2yOQHh1uWYEeuuWXWyvhoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/E1D645C5-FF43-42D5-8517-BB5AF0EA50BF_2/NrEyFtdypPS5qBRbNAlSz2TjW51MAzryU7m4IZ7TClEz/Photo%20from%20Library.jpeg)

B13

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/01361001-26AB-4DCD-A73F-38312D00F0B4_2/681SnUp29d0sX2KUPWKts86roxf4lj4xSuP6MpN7kSYz/Photo%20from%20Library.jpeg)

For B14 too.  Just emailed Alan to see if there is a solution, as this is very annoying.

 Let’s evaporate 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/6303EBEC-F013-42B3-AB23-1B7A31F57E8C_2/ejitFBOqtAylgHUQixgpydHiH8dh11bya2LkqonXsAkz/Photo%20from%20Library.jpeg)

Life is good. 

For Ti (nice and low power too)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/4B04FD55-F092-46D8-86A6-622F97A8395A_2/sav2g4j1Qw5vnYaGyecKem2BHKP5QYPIqVhmBvTphX0z/Photo%20from%20Library.jpeg)

Onto Au (adjusting prog parameters)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/CF542299-B5C9-426C-8061-9606DE77797D_2/p1eYzvAXwlSz4xaBYPr5bl5FdLIOxVXXT4ImiGhMp2Iz/Photo%20from%20Library.jpeg)

After evaporating 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/7F080353-8A67-4DA2-B145-1437170A7774_2/CPe3d1hakW2Cx3WkYd68ocWcVlqL8gLeUYq9sDAmJ5kz/Photo%20from%20Library.jpeg)

Same geometry as the box implies 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/66C9FB52-3F36-4123-9DEB-552A2A9E7AFB_2/PLyKnwVmfMxevOJ3y21VP5sxUXD8gk04s2wEyPv1rgsz/Photo%20from%20Library.jpeg)

The chips are now back in the lab.  Lets do some conductivity measurments

Reference:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/4217119C-C325-4177-A9FE-2DEA0FAF5648_2/WdQUxAcIl4v4ndHSo1bYs6ckKNJ1bzqazgUXB1UNNjgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/FC86083A-4CCD-414E-BA0F-4D136F2B7C4D_2/Ie5aKjbgHFD3FsJdt87lHxn7zwo80MySvMORtZoWA2gz/Image.png)

B12 (I am saying all of our chips are 1.3 cm by 1.3 cm, and 224 nm thick)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/CE5B8A1B-0C65-4A8D-A2FB-05D0FE09CAE2_2/TQ3zbZUBqPmhuqxY5YMU2UIAXHMKmZcfEcOeZS2gbnkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/59124749-321D-4C45-AA48-45CB3D308268_2/9QDVOULUpQZKRqYy8SxmOMR6iw1XJQGalaaFlKXd4Xoz/Image.png)

B13 (1cm by 1cm):

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/ADFF6F9D-CEDD-4417-9692-C29FEEF1EE70_2/xnxmjvjPqyvynXWZ81KSniRqxTkaVAKJpIc9MKy0rqkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/2FE4067D-FC3E-486A-B15A-98AA9017792D_2/CyjyH6dSqKlgylpVEsQMBuRsTXKDtBKEz8CfFc81ufwz/Image.png)

B14 (1.3 by 1.3)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/A92D4FFC-9FB3-4A4D-8276-CEFA84CA3610_2/04pfWuaIPOfRgJyzdzOzv65qFYvRKnFPxY11FJOvdqQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/7092FDFD-4800-4560-9116-1AD07CBD6200_2/IKt8ptpzV18OWHS6FgEtutF9uuMqhnbhhAbeYyhnSo0z/Image.png)

Now lets check to see how consistent these results are by doing one of the larger pads.\

B12 2.0 (1.4 cm by 2.3 cm)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/9E763BCA-CF28-4F1C-86CE-E68566F5B0C9_2/7MOyqk4b9IFzXKwRnOs8BnbJbtXwmoUyCB9VHaP0awEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/48974BAB-5AD9-4766-8174-776FFFEBA4B1_2/AVwq2IxlmIID9RuBdxaSp4b82lZPlhrsfvYSsB8xPIMz/Image.png)

Those last points are real.  I suspect breakdown.  This is fairly consistent with before.

B13 2.0 (assuming same size as above)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/2627FE30-0B14-48CA-8FCB-A7EF9037B9D9_2/mFgWIkdO2QWhCZUoGlFcBJrzBzQMjXZRUvOLXD8Duogz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/309DA316-E376-47D1-B94B-015024B8F91E_2/cnwMxizOLaMxuI8x3JcfBy60tI07zIHWMd9GgL4Etigz/Image.png)

B14 2.0 (2cm by 1cm)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/9D778739-B025-4C22-A506-AF500A47AA5E_2/YTE3PWnjcg0MiZKF3pARKWwfLMh7ERI4AJxqyS6aWqQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/D8045D63-425B-44F1-B75B-70F0BE55CD6A_2/BvsywGeqOmpI8O9eLhbFurlR2IeqkxkYE12tU3MoZ0Yz/Image.png)

Below are the nice graphs:

The first take of data

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/50DB60C7-814C-45CD-B7E1-ABE8BF870C3A_2/0XyXk4pTxF4YtunboanU5iWhRiHNsE7r7FtjdVSPGScz/Image.png)

Second take of data

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/D2F00C8D-D763-4903-B92C-F0A06B0A007F_2/GRI8EgFbTJesHX6E7PjZcQemhDElrb57jVTGdIxxtC0z/Image.png)

Pretty much the same.  At least consistent on-chip results.  Lets compare some of our B10 recipe results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/C1C3D788-4F8E-4FFF-A5F8-14DCC0C215B0_2/qLsybiaRiacbQCQhz4hrQhnglNxqyxn5Wy0mwrG0nQAz/Image.png)

So it seems that we get a lot of variablity between depositions when we use N20 = 150 (though this week’s depositions to look good).

The graph below shows what we should expect for other 5W depositions

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/3ECE3046-962F-40C0-9BE5-B8A0FF66C61E_2/TYlzJlMO657vhYkgyqMIrnjyQEaKtf6Jl0Fvlh7xJXcz/Image.png)

FWIW, it looks like the conductivity does follow a trend at 5W when things work right.  The key question here is why is it that the 135 sccm and 160 sccm films not follow this trend.  I suspect the PECVD was not really applying 5W.  Maybe we should light at 6W, and deposit at 4W.  It is objective that these films were still much more conductive than their 6W counterparts.  Even the films that were exponential at low field were still much more conductive.  I am also happy that each pad gave roughly the same result, showing some consistency across the wafer.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3F4A3340-3A8D-425E-B673-EE0BEC97018D/9D1EAE4B-F7C1-4D02-AE25-562AF145CCEA_2/A4RCcuxAtmJzdoDclhj6LxLhoNnEI83L7e9VCxui0Mkz/Image.png)

Above is a direct comparison of 5W and 6W films.  What is intereting in this comparison is that the 6W films are all linear resistors.  More resistive than their 5W companions in the high field (mind you) but for some reason they are not linear.  I just don’t know why they are not linear.

Going forward, there are two possible paths for me to try:

1. Doing 5 second light at 6W, and then depositing at 4W.  Hopefully the improved conductivity will make up for nonlinear effects
2. Try messing around with doping.  It is possible that the dopants are not doing much to help us conductivity wise, and instead might be hurting our optical loss.  If we can get low loss for lower N2O flow, that would be a win.  In that case, I would try to make a film with no doping and 200 sccms of doping and see what the result is.

As a final, desperate, resort, we could try seeing what the results are for lots of trials.  This seems like a lot of time and effrot to learn minimal amounts, so I say we avoid it.