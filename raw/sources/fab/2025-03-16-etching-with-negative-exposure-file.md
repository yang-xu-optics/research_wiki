---
type: craft-export
title: "2025-03-16 etching with negative exposure file"
craft_document_id: 3246DCDE-1018-479C-9C4F-D0A892242D6C
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-03-16 etching with negative exposure file
This note documents the process by which we do the flood exposure of the wafer using the positive resist.  The reason we are doing it this way (instead of with hexing) is that we want to etch ALL the way through the SiNx layer.  This will allow us to get rid of any residual stress effects in the film that could lead to cracking (as I don’t expect oxides to be the issue).  The rough draft of the GDS file is below, though there are still a few touch-ups to do

[pad3 pass5.5.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/005467B9-A95A-48C2-AE3A-AB4F1A74FCB3_2/GZl1YV78tQxMxJhxERFCX21HAFZRZW9B65KPbcJ7xx4z/pad3%20pass5.5.gds)

![Image.png](../../assets/fab/2025-03-16-etching-with-negative-exposure-file-001.jpg)

It does look a bit objectively insane.  I may end up recompiling it with higher resolution on the spirals.  There are also a few features that are pointy on the spirals that I would like to get rid of.  Either way, this is not bad.  Giovanni said the exposure might take a while.  This is fine, so long as it happens.  He also said to underexposue (between 50 and 55 as the dose).

We have two wafers in storage at the moment: Three layer device and the four layer device.  Both have Cr hard masks sputtered already, so we should be good to go.  Keep in mind, we want these devices so we can test whether three layer devices are better and if annealed in the CCMR can help.  These devices are already contaminated with Cr hard masks, so we can’t use the CNF’s high tempurature tube.  There is no huge parallel benefit to doing multiple wafers at once (as the tools can only take one wafer at a time and this mostly saves time on seasoning).  That being said, I can’t think of a good reason not to do both wafers.  So lets expose both wafers, and we can figure out cleaving later.  We will also want to cleave off a small part of each wafer as a straight waveguide test in the CCMR.

Below is rotated and centered GDS file 

[pad3 pass6.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/FCE76732-79FE-4CFA-8E21-7C89D183E8B0_2/cuJQq6VKdxxhZZ8Dylwgf0HLt1oM9HxnPgMk0btRkCYz/pad3%20pass6.gds)

For resist, I will use 3000, 8000, 60.  I don’t feel a need to vapour prime.  I will just use normal primer.  I will also coat the wafer while it is centereing (so there is a bit of spin)

Before spin

![Photo from Library.jpeg](../../assets/fab/2025-03-16-etching-with-negative-exposure-file-002.jpg)

I will also bake at 90 C for 1 minute

Below is mla before write. We use de focus of 0 and dose of 56

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/DDFB57CA-1AFE-4595-9EAD-E3F2A7AB0BBE_2/kwSP4G7z6yG8yExrFKnv2aeoD7eQPZapi8oBlmNt1iAz/Photo%20from%20Library.jpeg)

During exposure of four layer device

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/B70609A9-9856-42A4-8CD2-129676C5511A_2/5Vo2FZs7V5atCj7UJlAmPrQv5xXjArNd4mGk33VJTzcz/Photo%20from%20Library.jpeg)

For development, we use program 4, which is 726 for 1 minute

Before second exposure

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/FEAF609D-898D-481C-B033-324B0A1DE418_2/Yyjayi1jU7vnrJew8yOBAxHByG5mNQfrNj5BzbG6BoYz/Photo%20from%20Library.jpeg)

During second exposure

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/22CFA4C1-8C4E-4177-9432-452CDE0349DD_2/mngAZLZGNLvta8pjjNf4SgOixxqniz1gf3F5NWmMrBcz/Photo%20from%20Library.jpeg)

Below is first development program

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/65DE2908-FBBD-414C-A75C-A06BEF9AC253_2/4PFp7PgqTsvhxWJoMVi3oGnxZzIHTIkhnXUAhpZCproz/Photo%20from%20Library.jpeg)

After first development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/71935DCA-E136-447B-A01D-87D0261D667D_2/T0dFRjHzBOhpxSJUE1DxHhTnoogEhGxy1bKPIZyn5VAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/0502E719-AED5-46E8-BF8F-43FC8D758521_2/HzeikGWVT0LNgs9AMYUxa30JXOyVQbRrgxCdjRpxad0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/DD4C3802-28C0-448B-9CE6-F638CA6C95DA_2/AikKZiXhuwyW3UGBLKXribPKiKBfXg8TojQHDlubl5Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/490A0BF3-FD12-4E90-9F40-6351B85B3DB7_2/DWqZRY9zJaO7vlWQz7pRWkuZv49DdwvJOwQzst81rzoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/27CB1673-9EB1-4797-BE66-C15FD18B3F43_2/vpA6iufIuKghEyF9TMOjflVMS8r6aBr3QymfNxxateMz/Photo%20from%20Library.jpeg)

Next, we want 50 second descum.  I am shortening this slightly.  We will also want to do a 5 minute season of the 81.  We will do a 10 minute season of the PT 770.  Then we will do 8:30 of Cr etching.  Sounds like a plan to me!

Before Cr season, it is the same as we left it

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/632A898E-4B11-41E6-A786-AAED7799680F_2/ffCRjQj129wLqNyCYExZUSJr81T03lfTj1v8tqg4BDcz/Photo%20from%20Library.jpeg)

Before second development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/614751D2-7E26-45E0-964D-05DC847F5A7D_2/Aq6mjcfeivhno6cMb5FaQNjd16xuxs0vmzVU3atqaVAz/Photo%20from%20Library.jpeg)

After second development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/0826E33C-193F-49B5-A682-FA9973B51574_2/hS2YuJfyBKxnj97Us3uG2VhZ0IaOhm9ws0B1soralj8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/7CB0552C-C7FA-48AB-AF6B-431296C6DCF1_2/jj6fBhXESABRr3v8xrzjQe7fL0MPZ2wPduikMESHVdsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/FCE50916-D093-4A4E-8A4C-2A8D6742A3A3_2/5JqyIYHJ9R3fO24zMLaUv4F2KRU4d1pzN98ExUyidd8z/Photo%20from%20Library.jpeg)

Three layer on right

Before descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/C21F4165-2A11-4C04-B846-8EF8E1A5809D_2/mRujQnVTTBpPZxp1xoNgWC2tyy4Ugwcxax1jlJRHRTcz/Photo%20from%20Library.jpeg)

During descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/38F4018D-4FB9-4505-A0FB-96F0A6ED3593_2/UayjUfImt8dNO1CzxpFxYSKqBhjF9RcVdLAOunEzqtAz/Photo%20from%20Library.jpeg)

During 3 layer Cr etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/248B134E-769F-4D65-AE54-E339195FB05A_2/EiD3dtZ0Y5VggMAsF4fvlnUFWLBCfrJntX4an2G8kzkz/Photo%20from%20Library.jpeg)

During 4 layer Cr etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/EB4053FE-1A08-4DA0-9634-AA566C9E28BB_2/TRBdfQSmLVX0baqoGfIqlsaHfwP7xOO6NeYxD7ZjWncz/Photo%20from%20Library.jpeg)

After Cr etch of 3 layer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/06A3254E-0EE8-4903-BF42-2540F23C5792_2/I7VxjgeSE8yQQODyiawHR3H3xDNMpAxUJFaX9PUBRxIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/A85E6CD6-AF5F-4970-A790-E85DD807A919_2/30W496cJ2qHK0Y7Sb8HypTqY1FknwWcJha8FEPJf8f0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/5CB50D0F-D3A3-4A94-B19E-ED8808A18E0A_2/xhrUYq0QpviDwmjVjJWoaXplODKUA8MPOKMIM9pxxU8z/Photo%20from%20Library.jpeg)

After Cr etch of 4 layer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/D78BA817-0114-4C20-8783-C72961768A8B_2/xby3w9x8F3kobDZTnqXZc6npCjCM9CFCLMCqSpVbtqUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/9EFF40F5-5476-4750-BC84-805F21C642E1_2/PAZbVOpmrEuzkb8LcLp4Biusnlh52Uphkqnbx5Sd8poz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/A1A17163-C124-4FAF-A5D3-A2102ABEB1D8_2/zaOBx4o7ix0JyfxhtT5sfMou2XYi3UNkqR7oYtLHC2gz/Photo%20from%20Library.jpeg)

Notice that the wafers have different colors.  This is a nice little confirmation that we did assign each wafer the right layer number (as the four layer device after oxide is purple).  We lost a bit of waveguide extension at the top because of the wafer clamp, so we will have to account for that in the future.  On the right side, this will make it very easy to see whether the Cr comes over during wet etch (as we now have a large and visable Cr region).

Next, lets think about the Oxford 100 dielectric etch.  On the four layer deivce, we have ~100 nm of Cr, 300 nm of oxide, and 2um of SiNx (the rest does not matter).  We want to etch all the way down.  This means we probably want to see at least 2.5 um on the profilometer.  We can also use the ellipsometer too, as we now have plenty of wide and exposed areas.  We etched 10 mins to get this depth before.  Lets do **10.5 mins** just to be safe.

For three layer device, we have 100 nm of Cr, 300 nm of DON, 1 um of core PECVD SiNx, and 1.8 um of DON.  We want to etch all the way down, so we went to see a depth of 3.2 um.  We previously found that our native oxford PECVD oxide etches at 150 nm per min and the SiNx etched at 170 nm per min (but this was over a year ago).  Our SVM nitride etches at 275 nm/min.  So pretty high.  Lets assume that rate.  This means we etch 11.6 mins, but lets make it 12.  We definately want to etch the four layer device first, as there is greater certainty there.

There is a bit of an arguement to be made that we should cleave off a piece of the 3 layer device and only etch through the 1 um thick core.  This would preserve a higher breakdown.  I think a large reason we are getting faster etch rates is because we are etching on full wafers.  At some level, I don’t expect us to need to etch all the way down yet, as I have no idea what kind of annealing proceedure I want to do.  So we really only want to etch 1.5 um down (to get through 300 nm top DON, 100 nm Cr mask, and 1 um SiNx layer).  So lets instead etch for **5.5 mins**.  

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/B7FFEB69-19C3-46FE-BBD7-EFAD2DEDD5CD_2/EyM9UkKe7CyNaMksEyP1Ze9iXyUnD36PuPrsCzfdwUsz/Photo%20from%20Library.jpeg)

Before 4 layer etch 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/3C45FA37-B76D-4C60-8887-90BD6900ED46_2/i0ruaN9NRfvye9nU3tRMq0mwbfjU7wbre9FXJO9WSO0z/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/1D0CA765-7D91-42B5-B8CB-9E2F1E832668_2/HyyEczRNiZqayD5rDYrahCkSXsylcrxVVfXAgO91Bqcz/Photo%20from%20Library.jpeg)

After etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/485D2B0D-AF15-48C8-981F-FE30EE22BFDF_2/1xnSeMQleOQYzzuWf9svj7KhBIBUGlVFqoyyMvATEuAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/3D0843D9-29A6-4B47-8774-97B401700402_2/iAeaZLFm6MNk77O9c4v3qxbbugQVE7cqXudVYMfPdXoz/Photo%20from%20Library.jpeg)

Spin cleaning helps a bit with dust

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/F619F1A0-2723-4E8F-8E5F-FA066561E972_2/3fvqWtymLnqazaN4v09E5LS7y3sDdkmsIC5Ayx9wThIz/Photo%20from%20Library.jpeg)

No dust on other wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/D47E0439-23D5-483D-8ED4-0ADDAC7CC7B5_2/cpWThbniXhREoFHuwxad3fWDBSFxK1y2uk3jwVhc3Zgz/Photo%20from%20Library.jpeg)

I am not sure what the dust is, but I want to finish etching.  It seems the oxford 100 just does this.  Based on that etch, we have a rate of 210 nm/min.  For the 3 layer device, where we want to etch 1.5 um down, this means **7:30 mins.**  We also need another 1 min 50 seconds for the 4 layer device.  

Before three layer etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/7596ABDC-CA8C-4C32-BD4A-329FF9565F36_2/KkCwUnDp2lMZAQHBtAyxjrk1uso0yIrtx6IESOgr9Ssz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/36EFDA73-5A70-4C3D-8FF0-611DD4F977FC_2/VWzpuucuUohOwFnN2SeziyWxEKoQfFGCH6HKpVtRWq0z/Photo%20from%20Library.jpeg)

After three layer etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/9109AE24-8BBA-4EA6-B88D-7022D48524AB_2/wtym9CFHHYGB97U13QR5gzvp4Ngbk3zhWU96RIxns0Iz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/51BB4FF0-79A6-4F22-84BF-35600F0599B6_2/dnuZx5pdTQirKRqS6JPxHbZNcnyGnpcLxNDijXRNFDcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/80AC1B62-DC7A-4080-9DBC-114299B7FAAA_2/actQD08tynNB2zrLFNgUW8b9B6H5fqhNvV2waRxhNQAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/95A11E79-5479-47E9-9D23-7C1486FB0620_2/87UPMR4zJzdUUQTU86uyDph0QCVNRssvi0Ug6BuI3E0z/Photo%20from%20Library.jpeg)

So this dust is a bit mystifying.  I think it would also be good to take an ellipsometry measurement or two just to confirm the depth intuition.  I guess because more material is exposed, the etch rate is slower, as the chemical part is used more frequently.  From beforehand, it seems that acid cleans and spin cleaning seemed to help.  It seems that this dust just comes from using the oxford 100.  I am not sure if I am allowed to RTA clean these wafers, but at the very minimum, I can put them in HCl or something.  I will just need to check that it does not etch Cr.  This is not super urgent though.

We could also try sonicating in IPA, though I am a bit worried about damagining my etched structures (in case adhesion is mid or something)

# Note by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) on [`Mon, Mar 17`](day://2025.03.17)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/CE5A0ADB-CD52-41F8-BA69-284AF458F523_2/d2RnrCDKXZLljLLGQ9kmXTt1xMV67LALwdYh8y5xT1cz/Photo%20from%20Library.jpeg)

This is the 4 layer device that could be washed. We will try acetone and IPA first.

14:43 Acetone bathing started

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/34C7F652-AB43-4F73-9286-51DC0A3454DE_2/fVtgTcnxTi8cyJ5PoV7xlauem8ZBsWyxIqYQtZDyP1sz/Photo%20from%20Library.jpeg)

14:47 Moved to IPA now after 5 mins. We will inspect the surface under the microscope after this.

14:52 Taking it out

14:58 This did not clean off the dirt. We’re moving to sonic bath

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3246DCDE-1018-479C-9C4F-D0A892242D6C/685D3286-681C-4CD4-AC4C-675C7E25CF9A_2/iXgDsCk1YXtIU44CJc8zdu7zrorUrdurEosjbRylI0sz/Photo%20from%20Library.jpeg)