---
type: craft-export
title: "2024-5-25 ln linear device design specs"
craft_document_id: 8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-5-25 ln linear device design specs
The purpose of this document is to lay out the optimal design parameters for a LN linear DC device.  A lot of these principals can be transferred to the SRN nonlinear device as well.  I want to figure out what thickness for the middle would be best, along with what thicknesses for the claddings would work to keep the mode confined.  At some level, the thicker the core, the better, so long as we are NOT multimode.  We would ideally like the device to also work at multiple frequencies, so we probably want to design the device to work well at our desired telecome wavelenghts, namely 1064, 1300, and 1550.  Below are the relevant LN indexes of refraction

1550: 2.1376

1300: 2.1455

1064: 2.1555

[Refractive index of LiNbO3 (Lithium niobate) - Zelmon-e](https://refractiveindex.info/?shelf=main&book=LiNbO3&page=Zelmon-e)

For our bottom oxide, lets use B12 data, as that is most likely going to be what I use

1550: 1.8886

1300: 1.8926

1064: 1.9019

These films are about equally dispersive, each showing an additional 0.01 for each wavelength jump here.  This means dispersion should not be too pronounced here.

Ryo seems to show good results with SiH4 = 6 sccms, from the following measurement

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/8fe5e6b7-20d2-55aa-9cb1-d281340a3277/hfHWz1fMKcM6p9qTRKNFSmdE2D3LzbBqVmxsGepWti8z/Image.png)

I am going to use my ellipsometry for this film.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/b8a15d79-1f77-887d-0da5-e69643d18b49/uqzfCZ03UramJ6y3wo3rC6FrFgWby1dY7C0wyTdDS0cz/Photo%20from%20Library.jpeg)

1550: 2.1732

1300: 2.1818

1064: 2.1952

Welp, we can’t use that film, the index is just a bit too high.  Tbh, this is a huge pain, as that film really did have ideal operating conditions.  But we are using the extraordinary index of refraction, so we must trudge on like this.

Lets instead do SiH4 = 5 sccms.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/f9ea09d3-9aeb-3cd1-4156-de9ed5a500bd/0GtbdNXjKOe94G3ZVlZ2R4NgJHybodZDDq0YhpZ8hN4z/Photo%20from%20Library.jpeg)

1550: 2.0963

1300: 2.1035

1064: 2.1143

These are lower than LN.  Hopefully, with a bit of silane decimal scanning, we can slip the recipe like SiH4=6 just below the index of LN.  We are now going to plug into our model solver

For d_LN = 0.67, d_DON = 2um, and d_SRN, we get the plot below.  At the begining, we definitely know we will need a thick core.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/8A8886D0-8F0F-4484-B53B-5E3BEB3351EE_2/srqAhjtbiQl6kk7vqkrQCC0DX4bNJ1p6Wj6GDrUlCwEz/Image.png)

I am going to do a parameter sweep and see what I get.  This is for 1064 nm by the way and using a delta_n of 1e-2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/3D39CF84-89C4-4FD9-9A48-2EA56B8FABDC_2/2GK204KZ7fRjA91rSoqxTV7qaOLNmJsowiucqlzGMogz/Image.png)

As we kinda expected, the thicker the core, the better.  We would prefer not to loose 20% of our programmable delta_n, so 3um seems like the play.  We will have to tell nanoLN this information.  At the very least a micron is needed.  One obvious way to reduce this issue is to use an SRN with a lower index.  This might eventually be the play, but let me simulate through and see what I get.

Below is the plot for 2um of LN as the core

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/893A16F6-A507-4E42-B8FE-1A801625C120_2/2qCnOEnvoXZIC4PykvpBeASIcvhkVjpgo6YQiEWppYgz/Image.png)

Below is 1um of LN as the core

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/2A5C6746-9AE9-4A8B-B05A-4667E5C2DEB9_2/STM90DXEgmDKhXy8uBpDUReByVLRpkwUuiooApzP4Tgz/Image.png)

Below is 1.5um of LN as the core

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/69C4C340-B663-4E0A-A09F-7FF8DF7A0CAB_2/AeHcQJSCUxscfRUE9Lws5eYcQ28femFkTuMHztYTyfsz/Image.png)

1.5 might do, but it is annoying that I take this hit. The only reason why a thicker core will be annoying is circular loops of current might kill us with a non-photoconductive bottom cladding.

From here, it seems fairly obvious that this device will confine our mode and not lead to loss of the mode.  We could probably even use a thinner bottom oxide, though based on previous ansys simulations, that is not nessesary.  Some questions that follow now:

1. What are the design advantages of using a thicker or thinner core.  
2. Should we try to insert a doped oxynitride “seed” layer, above the waveguide.  While could cause frindging issues, but if a thicker core is really anissue, this would help shift the mode up a bit.
3. What happens if we use an SRN with a slightly lower index

In theory, if we can easily get a thicker core and it shows no issues, we have a possible device.  The continual issue with a device like this will be multimode behavior, which I imagine will be quite pronounced.  We will also need to simulate how the other wavelengths are efffected.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/23C4292B-8048-4E5D-B74B-1C599F93181D_2/tvWmWMog1ovxxxEblXCpg3XHUIUxZ2L9Nz6Kta3FCBIz/Image.png)

I was actually quite wrong.  We don’t have a multimode problem, as we can see that the first order mode is quite leaky.  This is probably because our index contrast with the SRN is sooooo low.

Lets do Ansys simulation then

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/551DDF2C-258B-46A5-A26A-304C97FF6CFA_2/jEbdVoFTPwyrwyvemjYN7yGwyStCbzk5bbkpAtM74Hkz/Image.png)

Above is the device we are going to simulate in Ansys, and we are going to vary the thickness of the middle layer. I am also going to simulate with the following parameters

I am also going to set the following stack layer constants as:

SRN: cond_bright = 1e-8, cond_dark = 1e-10, eps = 8, d = 2um.

DON: cond = 1e-8, eps = 5, d = 2um

LN: cond = 1e-9, eps = 27

I am going to scan d_LN as follows:

3um, 2.5um, 2um, 1.5um, 1um, 0.5um.

I am using a period of 6um and a duty ratio of 2um of bright SRN.  In reality, this might be stupid, as I likely won’t be writing features this small anytime soon.  That being said, if we ever have the ambition of etching these devices, that is not a crazy period anymore.  I am also setting applied voltage to 1.

After 2um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/B9F3EF8F-8C2B-4F6F-A1DD-1EA80130FB13_2/DyBZ3dPKvzKMxorRErgUyX7xlPeeYZBOxSKiyHxfuxAz/Image.png)

After 2.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/695C816E-2222-4B6C-876E-35B93132C1F5_2/oJalkqeAosW18tvjSOReDaVFJgfJrKxi3IY7VhwVlV0z/Image.png)

3um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/60693946-2BD8-4477-851A-F281A36352E7_2/yJLSYYgXF8eHJG90GVPoxDDDL777iNdgIxz2p0JiwlMz/Image.png)

1.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/87E8EE38-B40B-43AC-992C-A5855244F678_2/r5231pbTbzGpmAyKwNsVFr0mBcu0C2zkQOnpWkClvbYz/Image.png)

1um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/5EDAE669-49CF-4030-8974-1A3B1BA47D54_2/gFz8EO28wDs78d7E2zbCD3v2sejNI029ygynnk0ULaEz/Image.png)

0.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/D89B50F2-F33A-46FF-A6A6-44E0EC80CED3_2/y9ijRLy5OaC9RE5P9zYVQ9hEk1sPg98hGK8KW4Cmn7Mz/Image.png)

By pure observation, we can see that the contrast is greater when the core is thinner.  This might have something to do with the fact that the thickness of our capacitors is on the order of the width of the capacitors.  I think it would be better to simulate these devices for a period of 20 um with a duuty (bright state width) of 10um.  I will simulate 3um → 1.5um for that (not as many points are needed).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/8794F5B3-A4D5-4CBE-BB88-C3B5BB89F45B_2/Qb40cmnhX8FppWP4LQlBFzKJT48serJHggFluR9NMyMz/Image.png)

3.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/EFB2B616-9F52-4E47-B4AB-30DE12C4BDE9_2/6J6UvyN24imxk0w2kknL9w8Cs3Q4AeMIfTug2Pw3ye0z/Image.png)

3um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/77E199ED-90DC-4134-99B6-29158645FB46_2/yMf6S10iGksBBalRfdiyeZJVTNZYUIwxOiP1szKMqBAz/Image.png)

2.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/6CE74D31-30C2-4A0A-BDA3-31314DD4A10A_2/qH7HVFy18F2PLLQKVhx1u4CCFbVuCz3F2opbGKVN04kz/Image.png)

2um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/366CDF0C-ABDD-4D9C-854B-54B200A39DF6_2/OZdTTqVqFCesDxxRivN3sNqQndKTRVnx8XYAQxlo3Xkz/Image.png)

1.5um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/59EE1AA5-6044-402C-8B2C-7B144837B467_2/4YbSWVAdymirDGFIPxI42KjRdsKKRMxtG0kb5qebMHQz/Image.png)

It seems, in the approximation where the width >> thickness, then all my previous simulations work.  The issue here is resolution, and a thicker core will limit the resolution we can achieve because of frindging.

Below are the results for a period of 6um

Bottom

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/AE14A622-4D8E-48C2-81E2-0B01C8B3D1B4_2/khUjjDdo5SJFxiHvhyxulEV2ps8NSkgxveHSQDiRsR8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/140F1796-18E1-4195-9C71-ECB6214193A5_2/yJpY0QAlSAxa5DnqEYLhaFqPMy8ojLEFICanF58rG1Mz/Image.png)

Middle

![Screenshot 2024-05-24 at 6.45.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/328BE5C2-38CB-4ABE-A927-1E419DC09EBA_2/NNFBCdaBEGbBM3QFlO5aUEbEHgPyOnOdwsE31tuCPFYz/Screenshot%202024-05-24%20at%206.45.05PM.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/6F27EB4F-3B0C-4E85-88AA-47A083136F10_2/rK0Qyi5rUSW7TAQXbQGz1FXDfarCGNwnMv5yUZ6ASz4z/Image.png)

Top

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/9F00C286-105C-4621-8969-1FBAFF0937B7_2/8tCMXFWGhoUFtcoegcXh9MxzyeOMbWrXl5eD9TLbuygz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/0797C963-38A8-45DE-9894-D5BF8F217041_2/hrJObdRn9vpvwyz3gVUrWxy9UmvjOSimWFXBJa4dgZQz/Image.png)

Now for a period of 20um with a duty cycle of 10um

Middle

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/7C5BDE69-9127-489B-82D8-8AFA7AC6D9A6_2/3ZnTdEBFKNKJ1pQmLGhgeuHWnvzK2xPcrzlhlPGyTecz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/700EED65-DE24-4BC9-9A13-A96D5488D40F_2/ET0f3gl2s2EutAxV4h7szYrPtR5ykpTE2iNna1mwv2kz/Image.png)

Top

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/B9562811-7134-49C8-8A3B-5CC3F64CE57D_2/TJE6jTyRIGy9j9OZ0OFTOt76h4mQ1cEP2fV6UQt0MnMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/3F193F6C-3868-46C7-AD6D-667C439236B0_2/Clgr5k7HGZWRO4N2OjtxcN6h0bvcBQJxbvUvBkGxICsz/Image.png)

Bottom

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/81FFC4BD-980D-4526-A14B-E7821E761877_2/alJzywzDZHMC9Lo1PusvZcWEdYciF1Umnqx3c9KOxYEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/2831AA02-99C9-412B-9AC6-E9E3BF8BD6BF_2/yKDRurouBN3JvWxKc8vOkTO167STwjCGRyy5nzUtIVIz/Image.png)

Something to note.  While it looks like the thickness is bad, this is highly deceptive, 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/88F26195-2819-422B-8828-2F45F2206401_2/XVHDIOSedAsMyBLvHuwrIhl2AR3wCAx6ddaOQ92lWi8z/Image.png)

As this plot shows (which is not in log-log scale), I decrease with 1/thickness.  So a key draw back is that as the film gets thicker, we just don’t need to put as much field in.  It still looks like some smearing effect is happening, but it is hard to tell.  I don’t think this is the most important parameter, and even if it were, it would be hard to make this thinner.  We will just have to apply more voltage to make this work.  Lets quickly cross check with what our step derivative code has to say.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/E46FA2BC-03FC-45D0-8499-2E35621D0061_2/aMY4XaTxFaRnkzL5ZoVO8X5vzJ5UTIRKQXFdqUNZ5rgz/Image.png)

Quantitative agreement for bright state for bottom and middle of the 20um period, 10um duty cycle simulations.  Top for 20-10 seems to actually be a bit higher interestingly.

For a 6um device, the middle graph agrees with this, top is a bit higher, and bottom is a bit lower.  I think the bottom being lower if the fringing effect.  So it seems that fringing matters at the bottom of thicker devices.  It is intersting though that the top effect to hav extra contrast.  This might be due to some weird horizontal effects?

For Dark state:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/3602F357-73A3-456F-B242-2FE94D434682_2/RgzXlqtrelhNfcAzS8lvyR63yxPiCwgn6vL2RIjyMWUz/Image.png)

So things should go down to 0.45 v/um.  All of the 20-10 agree with this, but none of the 6um period agree with this.  Looking at it, what is kinda crazy is that the shorter periods get better contrast.  Interesting effect.  For 20-10, the contrast is basically constant.  For 6um, while the contrast does vary (this is fringing effect), it is still impressively big. It does seem to prefer thinner films, but I also did not simulate that thin for 20-10.  My take I think it that we have no huge reason to worry here.

Actually, taking a look, it seems that the shorter periods are just inflated on the left side because they are thinner.  There is NO actual difference.  Overall, the difference in contrast is not super bad, meaning that the only fringing effect is from the field spreading at the bottom of a thick core.

We still prefer the effects of a thinner core.  Lets see the simulations we get for adding a seed layer.

Below is the simulation with a seed layer that is 500 nm thick

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/C822733D-6CF8-4B30-B78D-7E890EA54DFA_2/uXlQ48vvFjas9VieV235IUDE47jFBp3t4bIrTJzsXdUz/Image.png)

Ignore the weird peak, we verified that this was somehow simulating a leaky mode.  I am going to do a sweep for LN_thickness = 1um

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/8308F304-9AD5-4B9B-AC72-281564D8E2D0_2/UbClImZyLCs83mcPh85uutoXl6ijzNJEhAytcNn9Hmcz/Image.png)

Anything above 1 is likely some weird numerical issue.  Basically, a small seed layer will do

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/D9CAFE34-5AC0-4EF2-8E36-F64F88953E65_2/BlwAPTyRzwqXvqkRPMU3fsAT2QmyT9ZmHsxtQcysLdYz/Image.png)

This is an example of this weird leaky mode shit

Lets do a quick round of ansys simulations for different seed layer thicknesses in what technically is a DC device

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/00CDFAC3-2B91-4992-99A7-7DB3B33DD1BE_2/GfSHGXtG3dXNagA7d54RugD3BlzgLRHVYeQacu9TXjAz/Image.png)

Here are the constants I am going to put into the simulation

Bottom oxide: Conductivity = 1e-8, eps = 5, L = 2um

Core: Conductivity = 1e-9, eps = 27, L = 1um

Seed: Conductivty = 1e-8, eps = 5

SRN: Cond_bright = 1e-8, Cond_dark = 1e-10, eps = 8, L = 2um

I am using 20 um wide and a period of 10 um

We want to do a scan of the seed layer thickness.  I am going to do the following thicknesses:

0.1, 0.3, 0.5, 0.7, 0.9

0.1

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/83F05169-B7F0-41A5-BC21-92E2AB153562_2/SMXbryqOxj5k14EbuGfQfZHU4GbTsD5elFkzvUuk2Uwz/Image.png)

0.3

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/3CC6F763-7B3F-46B7-ACBA-63EEB4BC7E69_2/6flsZjf5OCAfECQ44m8yfL6q1ujt3jXzUmCzcSGGIhoz/Image.png)

0.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/21AAE612-5B68-4052-B518-FE8FB51979EC_2/xtW2fU5QfbA9TXxr0188qWTAHzv4cHouZEvr22y1dTAz/Image.png)

0.7

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/BF494402-2D90-4EAB-A8AD-E1352367E7C9_2/1Lzyt6SVIoGuDtKzjA2xMGDtKvqadbm240jTmjlNxAIz/Image.png)

0.9

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/FF298E83-3826-4F29-9037-5382B2D80F7D_2/6FhNaPydMcvUdZsmRSFTOObx4EQTwIXkuQsIFSpPD5Qz/Image.png)

Below are the results:

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/4C1E1033-03BE-43D6-B6B5-B7FB02E28D2C_2/t2t5wIr40QDgtG9IHd3J1y5iYgIuwqDLNfwHtwQp0yQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/D1DA33B2-5BC6-4B07-8810-E5D3A95A29C9_2/bQcSDXPXC6so2ZF0xX9lLWmNsBmukYjlUOheBHu4YTAz/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/98522BB4-3FB3-447C-95F9-6DDFFFD7A9BF_2/1d8l5lShjWfnRCf4Y1Qm8KZjYr4LueEJLIlto7y2fx4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/5E53A848-3A5F-4D9A-84F9-BD9DBA50F4F1_2/ImPrQSF8X6HzDCHgxKTsIT2j2wAUjffTaZGt3F77xpwz/Image.png)

Top:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/2114DC23-8DFF-4842-A113-2E78C4430073_2/VdFh2GJLJc19Mu8GBBxV9v9FbvetnIAvVBjJQcTyQ6Ez/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/5A1A4C1A-2BDA-4A3B-9825-993871E16A32_2/xduG7BD4Z8yzlyTqLywec6bX0omERCF4phUoq4Shu1Yz/Image.png)

FWIW, I wish I had used this ratio and linear plot in the past.  It is far more helpful to visualize.  The most obvious result is that there does seem to be reall fringing concerns.  Of course, we should use the transient solutions as our best measure, as they account for non-constant conductivtivty and we can tune voltage to the best possible value.  This simulation is obviously going to suffer from the fact that a thicker top oxide is going to absorb more field.  Still, given that it is 10X more conductive and usually 10X → 2X thinner, I can’t imagine that is the dominating effect.  But, at baseline, this fringing should be concerning, as we definatley want to keep the DON seed layer around 200 nm if possible.

Something that is a bit tough for me to see looking at these simulations is what our expected value should be with a thicker or thinner core.  I think it would be best to overplot on the core and seed layer thickness simulations a quick plot of what ideal resistors in series would do.  This would allow us to see how big of an effect fringing is having.  Below is for seed layer

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/0C85F428-9A93-4013-A4DF-DFBE695F6988_2/d5Hjccb6KO8zyAOj2cqZor5FYX2WbDuCEziy1PjqjUIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/FD2E5927-0D1E-47A9-ADCC-641411B39263_2/8Rwg2RbTOYczhzxUACKlkhsyMqtPyto0xVigxF9qIBAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/46207DB4-184F-4512-838D-26B8DFD79C0C_2/e5SuUxaOM7ChJfVG8yogfs5Fp7bxk28js7HL5Z2xYS8z/Image.png)

So, we basically see that we are exceeding the theoretrical maximum.  The reason for this is likely quite simple.  Near the top of the waveguide we are getting a small horizontal component.  The field becomes totally vertical near the bottom.  Basically, I am not concerned about fringing that much from the seed layer here as long as we are only a few hundred thick.  

Now for no seed layer, period of 6 with pertubration of 2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/1CCDF1B4-0FA5-4863-AFA4-9619F384F379_2/nomrkET2hSZRdqrnW4PV9k5c555zc8i0JGDuUbQRWxAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/9E918E98-FC57-44FB-892D-B213BB6F2B96_2/I5lAv9CIOyaq3f2mrYCdkGriV5fGH78Z2IuoidpF5eUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/064CC847-B495-4FE5-8268-485745F13168_2/Eq6XWi9vQIZlA3CeNxHSLlrkKuMKMNMkTCbFQUe1PZwz/Image.png)

Now for a period of 20 and perturbation of 10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/FC21E87C-0C7B-43C2-9A26-C805615CCF81_2/Jfoxt7hxzxDi6Jv4xxPulMUcAnUKfsb97g2wUCMxDiwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/6118BCB1-B84F-4047-990E-D3A4EAD97B4C_2/jqQN0yTDDGiL7Fpzxo9SGumlbJZwr4xLFzjkDs6C4Zgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/136280EB-9724-4585-9126-FFC94ABD6107_2/Qq6bIWRgcVQApYH4dKrPzcT6MoPX7XnQ7bbgeuurPWkz/Image.png)

These plots are actually super helpful.  Here is what we learn:

1. There is definatley a notable difference between our results for a smaller or larger period.  This confirms our intuition that the smaller periods will have less contrast (this still assumes block like conductivity profiles)
2. For thicker cores, we do get more fringing.  This is most notable in seeing how the bottom contrast diverges more from the ideal solutionas it gets thicker compared to the top cross section.
3. The effect of the seed layer is a bit harder to understand.  We do have some substantial horizontal fields from that film.  I think that is inflating the values we see.  Nonetheless, it is pretty clear that making the seed layer thicker definately causes field to flatten. I think the bottom case is most compelling, and it seems to indicate that thinner is better.  I would go for 200-300 nm, as that seems to give us a factor of 10X contrast at the bottom, which means higher everywhere else

I would like to improve our ansys simulations such that we only report the verticle field.  This will give me a lot more confidence in my results.  It seems achievable for us to get a factor of 10X index contrast, but I just want to confirm it.  At this point, I think it is better to prioritze delta_n over applied voltage.  We will probably still be around European wall plug anyway when it comes time for us to find the ideal operating voltage.

Below is Ansys result when I pick just the Z-axis (ignore the negative sign, it is just a scale factor for direction)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/B36D4EF8-B4D4-4DAA-9512-403C48D5F69C_2/5ivGTyYxKwym3x8rBGJ3vyU82IFPWrH2YD4AY1ywaI0z/Image.png)

Below is Ansys result when I JUST plot magnitude

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/BE2D4B76-8F21-41A4-868F-F29EA7B3CE8A_2/RzCKznMbmuDgyiVSxzt8i6T59bNDVvsAxDehqTzcEzkz/Image.png)

It does not seem like there is a huge differnce between the bottom and the edges.  It truly might just be the case that a thin seed layer beats ideal case?  This is weird though.  Lets check our previous calculations for top.  FWIW, running the numbers, it seems that we were not wrong.  This is very weird.  Maybe lets look at field overlay?

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/152A96E6-120F-4F03-903F-656E94C5549D_2/pm69gjKpSkgvZsWooQTdBsxSttrJAXklJLdpSLUYgVMz/Image.png)

This is indeed quite interesting.  The seed layer helps throw field horizontally quite fast.

When we print out the field strength in the bright and dark parts of the device for different seed thicknesses, we get:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/BBEB8595-739F-4E21-9ABC-E6BE12E61BE4_2/iMo3nkJCqf1Q3JQy190GhB0mJLcIqrQbxnz28a4BK4Yz/Image.png)

What is most interesting is the bright state is really not effected, but the dark one is.  Back of the envelope calculations don’t reveal much, so there must be some type of interseting divergence from nice behaviour here.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/34C76C78-8E3C-43C3-9334-46AB8B91544C_2/qPStxRRlAgRW9n3zcD678v5L5d1xpJasEuY0eT7FXR4z/Image.png)

These are not quite the same, as the seed_layer film is 1um core and the other is 1.5um.  It is really quite interesting for the Top.  Lets do the middle and bottom

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/9A3BA7E4-AD8D-4218-826B-68B199654A0D_2/xUfcxDqyHk10tNZvudcXgNWcxg6LRzHhVvb8yM22nBsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/6578E45B-C9B7-46B0-901F-C28156E0F1D8_2/DC24Dv8ni9Mm6QU1nh4LR0k0ODzH9gjWsyQ9cNssmIwz/Image.png)

This effect generalizes, showing it is not limited to the top.  This really is quite strange.  Lets see what the ratios are

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/B5858409-36EA-4631-8D56-5C9723765263_2/VZ9rhGJ7piCCyf3gFiUrxorvx1xrXyGbj2UneBjWPCkz/Image.png)

For reference, 1 in the above plot is with seed layer.  2 has no seed layer.  I really can’t understany this to be honest.  I am going to do a quick additional simulation of a 1um thick core and 0 seed layer to see what I get, as I just can’t pick out a trend.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/52293BB5-B063-46A6-B4D2-73A756FE1DC1_2/84kgdLTs2NX0SeakC2n5AWoov6OJ4MAFrqttviqaVFkz/Image.png)

I found the issue.  The middle conductivity is 1e-8 by accident

BELOW ARE REAL RESULTS FOR SEED LAYERS

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/4E78BA50-2D90-4BE3-BEAE-742F7F774560_2/lz8CMNwPCyH5yxeFjpcE2C2v5N5wYzqiG9XzyNA7Aegz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/1C2E79E6-6505-484D-820B-B8AA40511FC4_2/LcFXGXNflmTcO5VsqZNY7JRmQET1syqMaq4pxGzUwgIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/F28B63CE-234D-4C0D-ADFD-E30449BFEB13_2/XeoFFgZ7icxqx67SJGgH80ZPVOlkvJ4s1JWi9KDM5xMz/Image.png)

A few interesting take aways.  Firstly, it seems that we get better contrast when the core is more conductive.  Or at least, when the photoconductor is skewed to more insulating compared to the core.  I kinda wonder why.  Lastly is that seed layers do dramatically.  It is suprising that there is still such a huge gap between the ideal and real case.  We can at least see the effects of frindging clearly.  It is just very strange that this more conductive core is better.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/300FF5AC-FB8C-4694-8ED9-14240E8EEAC9_2/MTLBy3JwPL7qSJ4nHGAJXKXUpwq3NjMKCkY5wlo9gc0z/Image.png)

Above is a quick back of the envelope calculation.  Roughly, it seems like a more conductive core (or at least a more insulating SRN) gets better switching ratio.  This does make a lot of sense, as the SRN will totally dominate the resistiance, so the total resistance swing will be entirely dominated by SRN impedance swing.  Still, the issue with this setup is that we also need to use a LOT more voltage to get voltage swing in LN.  And again, a factor of 10 is really all we need.  We should think more in terms of percentages here, and realize that we are trying to go grom 90→95% with a bigger swing.  Kinda not nessesary.

Including with zero thickness

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/E0F71E92-36B5-42F8-BA7F-C858ED247468_2/gztyg4v2RJkjyjSjzeiSb1qynDYZ0Bl8La4HWdj5dHsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/014BFC67-6843-4173-A2A6-17DEC8117C6D_2/D6OcSupwoqnFi0WlHvDaXMLW07AwVtdlEtogq5Wc2wcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8ED763CA-04C8-4EBD-A38C-541A4DAE5EF1/EF8C90AF-954B-4473-BC65-92E129022335_2/gvyCnPUwY6cMQetQ9dTtEohtK3hd1rpAuncTWIhruH0z/Image.png)

Zero (besides for potentially Top) does not substantially increase contrast.  Really not important.  100-200 nm is fine.