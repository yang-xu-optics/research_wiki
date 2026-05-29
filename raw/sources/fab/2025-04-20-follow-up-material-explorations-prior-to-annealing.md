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

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/9F520E94-26BB-4279-87BC-183040E38B43_2/GfxEYB04pF2y9HMvfiLuysZtyoWUBxH4xpOPHnYTvTkz/Photo%20from%20Library.jpeg)

As I start the clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/1148D2EB-9F21-4EF9-AE72-BF3790BAE8CA_2/nieZInBlVCV5YO9GggDB2RsF9dyGtC5qCL1RCarmkFEz/Photo%20from%20Library.jpeg)

---

### [`Fri, Apr 18`](day://2025.04.18) Metricon measurement of the bare loss of the SVM wafer

### 637 nm

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/F1EC4726-B74A-4B46-A9EF-12615C7B3BC4_2/LVccrktcoLup0xJD0ysuwMI9SRFzUAyBE1PZvEo6BIIz/Photo%20from%20Library.jpeg)

![IMG_0612.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/4995BDF7-2631-4760-92B5-640F45E92525_2/1iPxK88Cg3TrBXQy8yhkJzi7OI6y8GNZymOQs7T9vc4z/IMG_0612.png)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/075939AE-480A-4DF0-A20E-96DFD41BC80D_2/1QvsylglXHEw9AokR6TFm5x9Tm25xsgamaj9SelW94Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/74EDF3F1-4CA8-47C3-B426-D3F98CEBFE05_2/mhq2UnPNJIsu4OiSEY7HxuBOHTCAIkmhFllPHEv3yxcz/Photo%20from%20Library.jpeg)

### 1546 nm

We use oxide index of 1.44

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/6D7ABB2B-BD8B-47F6-AEB1-1437948EE631_2/k0Fgl8nhyjBEn7M86gD5VTPBBmZ9BzECXxC0VwKOmIUz/Photo%20from%20Library.jpeg)

Fit is good. The fundamental mode is at 127.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/41D900A2-8D25-49B1-B2F5-C007A40A89C5_2/oOahGK1fb7TLEkXIm9SHVkgiq1hJs9SjUhjre0mOhhsz/Photo%20from%20Library.jpeg)

Ben got it, below is index for fund TE

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/26791BEC-2F67-44E7-9D99-B183409095AD_2/rX8nTDLqjQ2wNeVYZ3bOV8L8ickcHZ0Y1mJLJC5hp4Az/Photo%20from%20Library.jpeg)

Below are some loss fit

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/61BF5F46-4CF8-412F-968D-DEABA2B1D3DC_2/kfP1bobt4fSTF9oraHsmfPVgnZ6820Ix6cPuSf18ZyUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/2F1EAB49-D924-4AF0-8A10-FFC3B514A413_2/VfFaWP96SbCy0TVyUR7CXdXzBlU6pE5xneInfoRe0AEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/E3766E4C-6C7F-4B90-82A7-584A1A5B00BF_2/O3YRbqhX3dOaRLC12wIoOs9LA74ujg94U7orylasYNEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/258437DE-8E2F-42E8-B879-E704DE98FBF9_2/6vAsLLCCdM9yIJj9Xt6fF2dWD0QNwDaRkfMmgCNh0z0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/312C09B0-A907-4EF5-9E1D-BD6B7D89D674_2/upPPniRyyinOK2uHdDv2bRkbmSpaNopSCx7FoyKFKAcz/Photo%20from%20Library.jpeg)

Now back to some simulation, as we are trying to design the optimal film thickness to get loss.  Below is a plot of radiative mode mode for SiNx films with different core thickness and height

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/A891BC83-26CB-4069-A244-ACC1D7B743C4_2/o61Odpdlr8jftxiyvxlMOEccqgvxSBY4rLFCIcAelOIz/Image.png)

To put it mildly, this is not great.  This really shows we need films that are quite thick.  Below are some plots of the index at 1550 for different SiH4 flows, just to get a sense of the area we are working in

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/D9C9E2BC-68E2-4324-B2FA-645D33DF035B_2/oByg3rNMkTyzPiJ3xUbAepaq0tcWFLQ9RxIbe8H9iH8z/Image.png)

It is also interesting that our index are already quite a bit lower than the SVM.  Below are the poling periods for 6um wide recipes using our previous fits for these recipes

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/293BDFDF-84BD-4DA7-9EF4-4C1D5BEDFC2B_2/EFbex9Y2mqgkERSOlaRQaI8Rt62GpYoUCOEyuQXrQDIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/B7B05240-88FF-4E08-9DD8-2DA032198BEE_2/2TMwyaF8JIdbggKE8BY3rcxyadOI3Bce15jvxj9cjUMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/23C1EE33-2D45-4CB7-8D0A-73732C1220EF_2/szea06rtvCcXCadfyZK8qtX2xsFkM6vE7BPBOq9VXkgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/3E887E59-D2CD-4008-A415-5D3F14DC41BA_2/T0sXltRyjKegyTODNa8ArvwsdT9jkYWbUNlhAUarBzIz/Image.png)

It seems the recipe does not effect the poling period much.  An interesting point here is that even SRN3.5 is more silicon more than SVM.  I would really like to be below the 1 dB/cm loss value, as that would just make our life so much easier (in the sense that we can treat that loss value as negligable compared to material loss).  We are starting with two cleanish wafers (though they were cleaned 2 days ago, but still).  I am also going to do cut-back method with full wafer fabrication to characterie the loss of these films.  I feel like that is safer than metricon (and in some sense less destructive).

Looking above, it seems that depositing SRN 3.5 and SRN 2.8 would be the most time efficent path.  SRN 3.5 needs a core thickness of 1500 nm (at least) to have low substrate loss.  SRN 2.8 needs a core thickness of 1800 nm (at least) to have low substrate loss.  Long depositions ahead I guess.  From earlier depositions, we know SRN3.5 deposits at a rate of 38.2 nm/min.  SRN2.8 deposits at a rate of 32.2 nm/min.  So we must deposit **SRN 3.5 for 40 mins** and **SRN 2.8 for 56 mins**.  This is crazy.  

If we just want loss values, we can deposit thicker bottom oxides.  Below are plots of the radiative losses for thicker bottom oxides

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/29CDE2F1-464B-4EBD-B5D6-A50EBC43AEBF_2/Ll36ujZtyY7bkHtrNQM6ZhY7OVoGPP4zxzXv43kFJaEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/09581F16-81AD-4C03-A35F-7A1F9BB11F8B_2/MUpSQz5TKUOwypJXexzIx4Tpb7ZJrgJEN5RK1wGM4hkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/C3FA3341-497F-4EDF-B094-C4CAA7CBA26C_2/j74cjxyWKENLiDLwFWj0QC13bE9StqMrDAt3EalxfDkz/Image.png)

It seems that 1.75 is very safe.  We then only need 900 nm of the stuff to get working devices.  Lets do 775 nm as the base added oxide.  Given that smooth oxide deposits at 166.6 nm/min.  High rate is at 240 nm/min.  To avoid any type of loss, I feel like smooth will work better.  Lets deposit smooth oxide for 4 mins and 40 seconds per wafer.  Use 1 min season as well.  We will then do **23.5 mins of SRN3.5** and **28 mins of SRN2.8**.  This is mildly more reasonable.  I am going to leave depositions with no H2 to a later date.

Finally, we may want to attempt a hydex-type recipe.  I am still really of two minds about the best way to do this (the fast way, or the smooth way).  While I am not terribley confident of this, I feel like the smooth way is still best.  So we are in for another longish deposition.  We can also try the fast approuch if we have time and feel up to it as well.  I generally feel like the only arguement against this is that there is almost no parallelization to all of this.  Given that, I think to SiNx wafers are enough for now.  We can try hydex later.



### PECVD

I am running a 5 min pre clean of the chamber.  I will then season smooth oxide for 1 minute.  Something to keep in mind if the surface we are depositing on might not be perfectly smooth, and because our waveguides are not as tall, the mode will see the roughness a bit more.  So we will have slightly more scattering losses

Before smooth season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/284A02FE-94ED-43BE-A97D-89579113F602_2/Gxz14RlwFT43zrx3mZPfwDN9j0ZZFJxI82RUSPbm2eoz/Photo%20from%20Library.jpeg)

Before dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/59DD7771-622B-4444-A00E-04AEE045E03D_2/c8uHaqTYdRM7XuIDzEZAuoGcc0uawSD7aqREXvRBDi0z/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/A68AB737-0D82-45E1-8D85-D386109469A8_2/S2dXtg8oRehq9fNpRNRlOLI9N18o7PWKW2wYplLfqO8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/31315112-4E45-446C-BC3A-A1A9646DB331_2/hUDYQfGmryJT8RW59fknU7RtUY9xXdlcMfR1jpaubnYz/Photo%20from%20Library.jpeg)

It seems we got the right amount

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/818DDE79-D026-45B3-95C1-18ACF46B131E_2/0adhaU1uYF4W0vROKToRv8CSInDEzotiMrsUsebB0M4z/Photo%20from%20Library.jpeg)

During dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/34EEDE42-3CAF-4E46-ADB3-BE8F0370D57D_2/ara19nUrG3j3YEPWR2E2MpdANqHgAd73rzwu3qEZhioz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/24D85E75-B378-46E0-9016-B2894271AEF7_2/GI2hfF0yB12yFTqhhC8PI4yDx6K32MCEkQL7tQExGHoz/Photo%20from%20Library.jpeg)

Before SRN 3 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/E4268980-580E-4A4A-97E7-8065A4F893DA_2/omhIe9kB6XQViZ2yhxKnLHgaMnQWvbxt8BWn4wmxiDMz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/E3027387-77BB-4B25-AF4D-7B4D7F2637C4_2/o0OghN7OVFnN1fMmydiAXW827XRx2QBLybM794Mz8UYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/540C258E-0A24-4EAF-87D3-C6EE24C927DF_2/U5NOcAmxb7wr7DdDsPopWcuoC7SxSmrkD9bM5Na3GfUz/Photo%20from%20Library.jpeg)

Deposits at 34 nm per min

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/32C0B7B7-0418-4B7D-9C09-156EF6B00D6F_2/vIop707atCoMhFu9D29eveJsH5haOyWFbNtpom8hlA4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/FC5983B1-E590-4CE3-81D8-519AC7C132B1_2/K9KDPRXMjtGLxoQx6JJWnA7xr33O1NrlGTqlZyCHvuUz/Photo%20from%20Library.jpeg)

Will do an extra min accidently did 3. For 3.5, I will stick to my guns

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/308B278C-1FA5-4E53-8030-2D5513CE2CAA_2/kMiQ1lnumpBhEv6J2LgGIwZlInp74HmAHaOKe3Ksppkz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/9A359186-C2F9-42EB-85E7-F7F463F2241E_2/hEBFM67aB4mcIasHLzq7eTFHpehjgk0iwczgx3ZjKTUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/C9FC1331-E046-405D-A3BC-5873E9769CA5_2/JRANHmcG5tvfibyUDBrZOW1BYZrsyYazGZCWxY36tT0z/Photo%20from%20Library.jpeg)

Front wafer in box is 3.5. One behind it is 2.7 (I am changing it down). 

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/178CE265-840E-4578-8B06-3C5A2AD9F195_2/YBo1iOBn5Sl6SJ5J6sHb2rbQWnbxIpG4DcMyZsqhSoYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/DE1A9F7F-08D1-42D0-B69A-685AAC55FD85_2/3ODWfPSnRTkZKtLFjzyR91jT4OWjcL2t7p2lY4hamLMz/Photo%20from%20Library.jpeg)

Before 2.7 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/79B2E01E-0F0A-448D-9633-0E07FD53B120_2/ceLtITu3igdxxpU3PsBdJXxRBeAzGf4PlF97QliuFuEz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/C75EB6DD-E74C-479E-A44C-9947DF0E5FBE_2/KZtisHl1y1P8Epc72qJsEIHsTXJVvyr4N3CcfSeETdAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/32E62984-E58E-416F-8C86-39EB00066435_2/hxLRJMWZufD8LDxELf5ZdC5x3x08eDE4gvx1mAJWv9Uz/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/0F2B0487-A4ED-4BCA-B270-9B85DC75E0C5_2/fSEFPhknUZjIuvKjao1Jr7mpL9gkoO0RHiAFNkHvHMwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/9D4D6F0E-A8E1-4BB8-AACB-C7633C8BAD12_2/7TsX5T9wB4o1Yvb3QWq83VMM9PS34xjcUEDArtALn2Az/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/9B11E938-F240-4EC2-8990-F11967413BA8_2/ZV2R7wtpTLBkpuZb7yUrwsbSAeAsLV6sNxiBfawn2KEz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/9A54B70B-2E4F-4119-8469-5984F7204DB9_2/pxEXYZtCMltTOLpjZVwgryFd8QrLfiBOiEtEvdhwxVoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/B0D34CB8-DD56-4C34-BE07-BC1BE55BBB89_2/aAQvWVxOv1EOxtxyS7XX3xRo03Mkxw1mrveIFKa8fs4z/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/33C4404B-0807-419C-AA03-35108993E957_2/jvycLCAkMw31estEqelTU9Bnr5CEJiZxUPqfPCdkoSkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/E2D24EC7-30D1-4E38-A901-E554E369CE45_2/u7ANPcyjUGkvDY1IYoRaYGgABzHmsyc0iBikY8cTGMUz/Photo%20from%20Library.jpeg)

I am skipping clean and moving to oxide dep with high rate

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/93D38406-BEE9-428F-B539-457FACE9294A_2/nmCz3zIOUei1KITe9Iulp3A5YyJCq12Jkiczdzb5pRIz/Photo%20from%20Library.jpeg)

I will do a 2 min oxide deposition

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/F74E98DA-9588-4F5B-9931-8F640F186DE3_2/bT5awZAgF6J0stlRxUlIMY35JxKZsrx3KrGxpiPiFxIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/BF519A22-6CF1-48B8-8A5A-92231A41C448_2/pqe40u2OIQVNhz7ebntsgg8kCdQ2Up8dYdeYou1Vy8Mz/Photo%20from%20Library.jpeg)

Before oxide on the 2.7 wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/A6C2D66F-0011-4B47-9636-5431C6593447_2/T2rLxRQYpo5Dfjo4QMpjvPvq431FqBfFDH0q8TcWNYsz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/3326C58E-B5D2-4AF7-84D0-53136AFB48F8_2/jbpBk1v6NyjmKSaes2laq7pNYq8ocTVdbo3i8JMGx2Ez/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/83E54F52-83EF-4C22-A110-A8AE3D5A436E_2/Mdhmjyl2xBsTyWLlCaXyvWfyGYgZbjSYY6EON7x5i1Ez/Photo%20from%20Library.jpeg)

During deposition of 3.5 (same oxide wafer)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/270D5513-F04E-43DF-A605-0A78E3A094F6_2/Qizp7Ndt0wR2k7MvSzye2KZ1Rh16xAXM11R6b8vNbhcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/B8E1DA5A-730B-4C9F-9075-4993B5C99DD3_2/ZAkCuv7UpyedrPMqwwTGK3RVRP0CfWAopBBMZVeq0q8z/Photo%20from%20Library.jpeg)

Remember, 3.5 is in front of 2.7

### Takachi PECVD

In light of a few papers (specifically these [https://www.nature.com/articles/s41377-024-01503-4](https://www.nature.com/articles/s41377-024-01503-4), [https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.22.054027](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.22.054027)) it seems that ICP-RIE PECVD can give better results for waveguides.  So I will deposit a film with the takachi PECVD.  Below is the recipe Ryo used last (it is the nitride recipe)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/07ba4bbb-d6dd-fc6e-e479-eac82475e391/I5D3g7mMVOKKWoJTA1PkyP8CedIxszSwPyqhPlCiLMMz/Photo%20from%20Library.jpeg)

Here is the note from Ryo’s work: [https://tdwg.craft.me/SXRb1ydrxl1jwn](https://tdwg.craft.me/SXRb1ydrxl1jwn).  Based on his characterizations, I will run a 1 minute season and 9 minute deposition.  This should give me ~1um of film.

They do have other recipes

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/7D4768E1-6B69-4C3A-8509-DCFEEA558E9A_2/lAIMc5s1mkBt7S2Hf72UQ4OunywVVviETaKLN1GRwmsz/Photo%20from%20Library.jpeg)

We might want to try the nitrogen rich one instead. I will season with it for one minute with a witness sample

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/8D5B7DE1-EFC0-4029-A98E-52F88B5284CE_2/98NR8iuMbmjIa8nYNp7IgLir1ntvwHFMolix9RyxBKIz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/83EE1C97-D2CD-4562-BD22-EC2E9DB141C5_2/CsxOupEjcDnyhHejoPYcyBGxX0UXQEKLwKZGTkZ3ve8z/Photo%20from%20Library.jpeg)

The difference with the normal recipe is less silane flow

Ellipsometer of witness

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/CB6389A0-069A-417B-98BE-F1CA2F06AD98_2/pT2hWpFOT8eQQW8h7asTaFaF2x5YQPDxg04o5ZfpoG4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/62D47D42-E031-4D13-A3BC-BD21114D2224_2/PuxZG4EDCm8i0ZfZi4HyKNmx3i1Je9LkJyElSVm40zoz/Photo%20from%20Library.jpeg)

This is very low index. Maybe I will save this for another time 

I will go back to original plan for main wafer

Before depositing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/B6C1ADA7-ABFD-46D4-901A-6A7B99F0AB2F_2/6puxXSk7pOdl9s3imy1WH3RadjOAgrZjgf5ed93wRcoz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/CFF8DF23-29F6-4541-A317-E7EB9943813C_2/OVcOSk7UXw7F2fOV0DoPYLQlmdnZ13eD5g7ZLj0gEWYz/Photo%20from%20Library.jpeg)

Everything ended fine too

Ellipsometer 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/C76DC3EA-39C4-42C5-BD58-A7C3350A2B12_2/dDchy3Bpu9HFBrgjf1USJrrivvuYS4qTFzKtSRI3GPIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/E08DA8DB-50B3-4C00-8763-8AA77BDA7CF7_2/ltCWzqvFCxyZNDPulJ2LMmy9sUbhx4GMoMqGxWbuYvwz/Photo%20from%20Library.jpeg)

We probably want 4 more mins of dep

Before dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/79781052-B0F7-4B35-8FC1-4C110D5C4E0D_2/hxUMtPixhErPKNwDr1B7tscNqxpuX7jUoa3T6a7ev9gz/Photo%20from%20Library.jpeg)

This should still have high confirement and little leakage even over 1 um of oxide.  This will definately be the highest index film we test.  I still think testing the N2 rich one in the future owuld be good, but that index was insanely low.  After this dep, we will run the long clean.  I will also get the PECVD going for a top oxide cap

During 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/5A4AC420-EDA2-4377-B222-7EBE3480007A_2/ctWtTePje7ccThjmTXJFUxMyKTxNegRolM4MK9dUo64z/Photo%20from%20Library.jpeg)

5 min clean on Pecvd is going. 

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/DD44635D-E793-4A55-B1F3-5BF56F844778_2/xE7zTeMv4FeNrzHTrKZpLcbNhO6oUEbVoid8huI1m6sz/Photo%20from%20Library.jpeg)

Ellipsometery after

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/AFBB120D-47FF-41F5-A607-5F2311C6FF6A_2/5FuWo2xGKmk9kWMFEmHQ0Ujr77GwjxTnyGqTVggIbkAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/95726862-134B-4575-9F83-EFCB9FD4C089_2/HyEKgEcV47zAMsEspqMrRHb1bCrvOXmQsawI2yRljpoz/Photo%20from%20Library.jpeg)

Still more borderline on loss than I would love, but it’s ok

Before cap deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/CA816340-C651-4944-99FF-79F3FED1EC34_2/uthvQa9jOdlTqGEv2ICkQkZVyzt9fHH4hfHuuT8rvtoz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/379B5233-6097-42E6-B4D5-D63C992DE5E5_2/pkPo5HHo9xnuyRXHU8bzzOeXvzNUMH33Z6aVtT8bjhYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/0E55F910-1F04-4C0D-A7F4-E7E4433E2219_2/IywgWIa6pkQdvg1rsCHaQlQPK291Bp6RLuDkAVffyk4z/Photo%20from%20Library.jpeg)

Wafer is now third back in front of the box. Should be pretty easy to see



Below are some dispersion curves: 

![Screenshot 2025-04-28 at 2.29.41 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6C9D1C56-4458-47D8-BDEC-3B7D43265757/FA624243-91BB-4950-B009-22425CEB33D0_2/OwRyCC1nhPHKlMNvQcxieqXSvn9yDD0WPe4ryigtR2Qz/Screenshot%202025-04-28%20at%202.29.41PM.png)

This is all before annealing ofc.  The Lipson LPCVD data should be taken with a grain of salt, as their stuff is deposited at a higher tempurature (so it should start denser and get rid of any non-bonded hydrogen, both of which could supress index).  Below is the reference where I got that index data: [https://refractiveindex.info/?shelf=main&book=Si3N4&page=Luke](https://refractiveindex.info/?shelf=main&book=Si3N4&page=Luke).  

The takachi is not as high as I origonally thought it was