---
type: craft-export
title: "2024-9-24 ln dc device parameter sweep"
craft_document_id: 04D7E739-193F-44A0-B52A-337CD86B6117
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-9-24 ln dc device parameter sweep
We are almost ready to ship a wafer to nanoLN!!  This means we have to do a more detailed scan of the performance of my LN DC devices.  The hope is that we can figure out the following:

1. Optimal thickness of bottom cladding
2. Effects of changing cond0 of the bottom cladding
3. Optimal thickness of top cladding in three layer device

We would ideally create a prediction plot of delta_n in the process so we could report a FOM number to the group.  The plots I would like to create (in the following order) are

1. Modulation efficency for core thickness (just to get an idea of how suboptimal we are)
2. Loss via substrate loss (as sanity check)
3. Data sweep of bottom oxide thickness and cond0
4. Once we have something roughly optimal for 3, then sweep PC thickness

Optional:

1. Loss calcualtion (though these are very hairy)
2. Ansys maxwell electrostatic field calculator (for fringing)

Below are some preliminary results for modulation efficency (using SiH4 = 4 PC and B27 annealed bottom oxide)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/E56372B9-7729-4F54-98F1-8F56DDF91712_2/bbitqaNBhWUTDNq3o7jVqFE86gPyYraO5xhZ7o3olEwz/Image.png)

And below is substrate loss for the same configuration

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/B1C7E39F-0DF6-43DE-A99D-E925E94D36AC_2/NZnAGNqMCVLQA6S6cZPJ5fbr5AfzL4tVUBb0qmeQnV4z/Image.png)

I am pleasantly subrised that we get a modulation efficency of ~75%.  Substarte loss is a bit higher than I was expecting, but not unreasonable either.  We will just have to deposit longer is all.

The more suprising results are below.  It seems that the cladding thickness and conductivity does not matter a tonne (granted, I may have just picked an optimal SRN).  

For cladding thickness (cond0 is 1e-12)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/16E4736B-C36D-44A8-A293-F43EDC2AD844_2/5xasvJbTFjYJaRsxhnGPORsjwwq4W5DejrygngXj9BEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/C3C49D0E-7B72-4096-8145-7C03498AC55F_2/WXV2dB8CwF8WvmBam18Loyl7uLKU0Vy0j3pcTyXXCwYz/Image.png)

For cladding conductivity (cond0 specifically, as exponent is roughly the same in general) (thickness is 1um)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/2F3DA213-782F-42E7-9C56-7198D7D79A64_2/v8nmeUnHEp8mCYAnyoLtA1iUJX8DRNuMBqt1fyaCjKYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/9C0DB8B8-12F0-409F-A885-CFE1E9A8CF6A_2/TG0OyL0UUum8Dlr0c3IDWnN6SdeYMNPoFMCzkTJZKp8z/Image.png)

It seems that, if you optimize your voltage correctly, you can basically get roughly optimal delta_n performance.  There seems to be a small trend for cladding thickness, but not cladding cond0.  either way, their trend is fairly minimal.  For refernce, below are the “Constant” factors for the rest of the device that I chose.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/7BD68260-D968-4A86-8EE1-65B43497C895_2/B4DJ8dKhVRFYnlp7ydlyf76IwAOL4KWw1kSIE5ozO2Mz/Image.png)

Only issue is that RC time constant is a bit long (~0.5 seconds).  Again, I really think that hte most important variable here is the SRN, not the cladding.  I will now do a 2D plane sweep of both cladding thickness and conductivity.  I will continue to assume ideally photoconductor behavior.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/A3D91ABE-5B62-4094-A81A-18E52C913447_2/Cqj9xYSrxa8JttzYIQ0QBM6ajSkS7hFBUzXZhbrJjagz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/D69EC179-3CAE-48D3-B651-1B0264F3AED1_2/8RlUZu6BvwQ8l8Ol02xbKaJvrmvkZ0C7HUYdzeFNs2Mz/Image.png)

Below are constant parameters

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/0F2E3827-969E-40AF-8D25-6F38EA10C766_2/eWORe3ZsE7i5cSxjHnaeMxhcdqxHl5ud60hURcPG5S8z/Image.png)

While the effect is not dramatic, it seems that we get a ~20% reduction for thicker or more resistive claddings.  It seems we were not near the peak voltage either.  It is possible that the RC constant in those regions is simply very long.  

So, after doing a quick simulation, it does seem that the RC constant in those regions is fairly bad (~2 seconds).  I am going to increase the N resolution and run the simulation again.  This being said, we should acknowledge that this type of performance is fairly bad.

After a longer parameter sweep

![Screenshot 2024-09-26 at 10.09.55 AM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/406D41B8-0E2D-4513-B322-4D781139787C_2/zIw1Pu7v6gn5I1te1QVUEOcqgIeA5ZMFB3xwMYV1vQsz/Screenshot%202024-09-26%20at%2010.09.55AM.png)

![Screenshot 2024-09-26 at 10.10.08 AM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/E50EB13F-A50D-41C3-B4BB-5E3DE15BDB40_2/QHzxPoJtzTLSQSTh9xP0rgQz6eyQngyhhCqH3oWKC2Mz/Screenshot%202024-09-26%20at%2010.10.08AM.png)

So it really does seem that more insulating and thicker are bad.  That is somewhat expected tbh.  Anyway, we now have some ideal of the loss, modulation efficency, and cladding parameters we want to use. While we could do a scan of the photoconductor, I don’t know how helpful it would be, as that is something we kinda figure out experimentally.  Other things we could look at is RC constant, but I would want a more finalized idea of what index I have so I know what the losses and efficencies will be

For SRN sweep

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/22716854-3A0A-410D-B240-5E443488490E_2/JKUaL4wVcF86XBxAm2dydzqi1M7k4C2HsqCZNPahPsoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/3D684C2D-ED09-4BBC-A467-BA44B6B8CC4C_2/C6HJQ3njVww2x9oFUvZj1oGbVYc2bcq0duHsRPyo7M4z/Image.png)

So an interesting effect here is that, because the exponent of the SRN in bright state is less than the exponent of SRN dark state, it might be the case that this effect dominates.  It is a bit tough to tell though. 

Below is a simulation where both exponents are the same (top is bright, bottom is dark)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/D08CA8C1-A41D-4EAB-90B8-3AC30A377D4F_2/Ac0y581vIyP2T5of6dLsSSzvbDVRo7hpCdMcsMY34hkz/Image.png)

Below is simulation where the bright exponent is less (like I found in experiment)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/E1DD7016-2B5F-43EB-8AC7-CCBD184D2B74_2/75Ad8GTx0MmUSZ6q5voKsdQKifv1QRPZofHAa7hYrYQz/Image.png)

In this case, the dark state is better.  

If you recall from electrical measurements, when we had field predictions base on DON, we got 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/261f1375-21f8-fb27-8673-8c29a4018602/oIeB6UsvAOlofcohMLdUhT7eo7LQAISafDfHbuoUrRcz/Image.png)

When SRN was the layer we modelled after 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/da38c3f4-4bea-e793-4741-298900fff9e9/WjCmghwEtnkWRN6VsP8kKyi5DnFZsxcyxGBDiosnv2Mz/Image.png)

So it is not inconceivable that these might be accurate results, but is hard to tell.

The idea here is that this is very hard to simulate

Using a bad x-axis (which is linear instead of logrithmic

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/3CF649D1-EE04-4E0E-92C1-F1549F5DBE7F_2/yQ6L5jEyBYCCImbg6xWIDg3vpkDpFypxOWye393wrxoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/4921185D-2995-40D9-BC40-1FAE04F5B46B_2/racanFxi6x9CBt6cPop7IbQAOKid8y9FFVOUDhjiORAz/Image.png)

SRN thickness roughnly had the effect we thought.  Hard to tell for contrast though

Final plots:

cond0 dark = 2e-17

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/D02C928B-9093-48F5-9EE8-9DF81DF8A6E1_2/bHOLMHTSObH8OC3aVt8C2603HZaDLpnzTZimRrxynv8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/B700A178-8391-4BB2-B46A-31F14BBDFA70_2/H3RyouWbQn6LrJpwnwkaydxJzlNr5GyR3nOEeWdOaQEz/Image.png)

cond0 dark = 2.e-16

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/270193CB-791D-4CFF-9451-783474BC8979_2/CUAKX8zY3jkimAfkUN0nOZRzrTj27bZPP5DwWK2xGMUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/02DA49D8-4E56-4308-8F4B-85559FE20012_2/bSEfwoObdFZJoxGVY9lP1QBKqpz3MrvdcOZFhe8W1J8z/Image.png)

Cond0 dark = 2e-15

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/62AEDF90-B172-4900-A5B9-09B27D240E99_2/mzKXHF68qUpAKRjV6xpKvvqZ10AvJgj9boJv8NE6Hosz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/4062A032-A66F-4406-B5BD-CC586A492F7C_2/obyUXKIPxd9pJ3BfPkGMAKGjNkKcktxxpwrZnV2ShEAz/Image.png)

Cond0 dark = 2e-14

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/6E220A66-945B-425A-92B5-76D8A091418A_2/9cFJmgL3yJnERffbxtE6I5AawwuzFwHU9Ln6l73TvCEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/D40DB0AC-53FF-4187-B9CA-C96CCC099597_2/5oBdtJmEIVaHLmRL40LqzBB6viEBqMskEdxOULor3MYz/Image.png)

Cond0 dark = 2e-13

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/C63237E4-E825-4026-96CD-59E186488477_2/l4pEiykK3bO2yjGrBdF2gRs7An1xMyaOtw6FIBC55mUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/01898D75-447C-4884-99D0-8249E987095A_2/3gmhs5NjO4klOOVlss4j9yYOAvDAkLIzEg9enhynHRMz/Image.png)

Cond0 dark = 2e-12

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/CCD20F2A-9472-43C8-B00F-EB7352F8B6B5_2/50UxLzDuwziPXxf1qvnjFywjhP75WIsXJCxRDCDyoXkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/ED0B97F5-9FE3-430D-9B64-906C47D306B7_2/x6O6WTJBki3PMsHtm4Q9Vbxvsg6GeNvdQFT5vF7DEwkz/Image.png)

Cond0 dark = 2e-11

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/AEF1F734-AFE7-4C0E-A773-A21A69B351EA_2/fdu5OAuv2okznidoCvlkfxGX61im2X3W38DCR1xIt5Az/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/968EB0DD-C5BB-45F7-96BF-9D4BB51D83D6_2/c2xQNHO6BGhUlVuNNLmlvQlH63Ntxk3dEDwxqAtxLxcz/Image.png)

Cond0 dark 2e-10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/908AF1EF-05BC-4DFC-9988-A712D3AB06C0_2/C5UyesjkVoFga5z6SLq5obQ3zQ1QAfYwzQ3jKBYaZO8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/04D7E739-193F-44A0-B52A-337CD86B6117/5BD25F2A-AF6E-4150-B8B0-5D53B7F5D497_2/esFZcuH9WeyEBuNYzoxECs5GgHkCAIHe1kTA5Ie6uTMz/Image.png)

This was actually quite useful.  It basically seems that more conductive SRN does NOT help for delta_n.  In fact, it gets worse at a certain point, with the only consistently good thing being a lower voltage requirement.  Higher switching is better and thicker is better if you are ok using higher voltage

The general conclusion here is that more system is very lenient on its requirements for DON and SRN