---
type: craft-export
title: "2025-7-1 srn3 cap and stress test"
craft_document_id: 7B7302E1-0CFF-47AC-B3D0-41B40CE2732B
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-7-1 srn3 cap and stress test
We sem to have converged onto the optimial device fabrication scheme for our final 1D nonlinear waveguide devices.  We have confirmed that the tapers do not cause much extra loss and that BOE dips to remove the oxide hard mask also do not increase loss.  We know the final oxide hard mask recipe we should use as well. We already have SRN3 wafers in waiting, which have ~2100 um of SRN3.  This is almost exactly what we had from SVM.  Below is the procedure I say we follow:


1. RCA clean and cap oxide deposition.  We deposit cap oxide for 6:35 to get ~1100 nm using the smooth recipe on PECVD
2. Spin coat ARC and 800 nm of DUV resist.  We found that a dose of 20 is a bit of an over exposire, so lets use a dose of 18. Develop after with Gamma
3. Descum for 1:20 using 81/82. 
4. Clean 100 for 5-10 mins, run a 1 minute season, and etch the oxide for 6:40 mins.  Do Ecoclean for 5 minutes and piranha.  Check depth after in profilometer and ellipsometer.
5. Clean 100 for 8 minutes, season for 2 minutes, and do a 5:25 etch to clear nitride. After etch, BOE dip for 45 seconds. Run ecoclean + piranha as well if you want
6. Deposit capping oxide with 9 minute smooth deposition.
7. RCA clean and do 1100 C anneal.  Ramp anneal for 2 hours and run main anneal for 5 hours.



We will be making two wafers.  One will be used for 1100 C anneal today, and the other for 1200 C anneal in the future.  While there is some legitimate debate as to whether it is best to put an oxide cap ontop, I am going to do that for now.  For one, this will help get rid of any hydrogen in my PECVD oxide.  More importantly, it will proect the waveguides from contamination.  In theory, no cap might be better because it would not create surface trap sites for defects and might allow the material surfaces to smoothen more.  But for now, we play it conservative.  We are making two wafers because we are paranoid about the etching process not working again in the future for no reason at all.  

### RCA and hard mask deposition

![Photo from Library.jpeg](../../assets/fab/2025-7-1-srn3-cap-and-stress-test-001.jpg)

I was following JVD as he moved my stuff around for me.

I am running 10 minute clean on PECVD.  Will do 1 minute season next

Before seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/44F24ABB-621D-4B81-94D1-9B20BDC9BFD8_2/CC4HwOIToudZxRCJ4S8kNiI1y9f6QF4kI0JOmqi7Msgz/Photo%20from%20Library.jpeg)

Before first deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/C6B9D320-B320-4B4C-A0F7-1C422C608021_2/QtXFF3bYh1eJxgSqQe6KQ4bUUV4uOQseFrenn3qJ8K0z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/9C2B1CC6-96E4-4C2A-8C1B-C90F365837DE_2/KQR5qV4VRmaOIggpL5jHyaQbpzHtGauMaCz0XaHg0x4z/Photo%20from%20Library.jpeg)

We now do an 8 minutes clean

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/3A6A92A8-6965-454B-A845-561B74548D75_2/Mt1KerQBtxA0xrtdXtry0Sg1zENjawbPYyNgZo9A4g8z/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/35CB1407-1247-4E5E-8597-4DBA5453B554_2/NXNYMbGA0T5yqMLfIdbApBXrdZy1YaIE3N9C9TU64noz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/95A59F57-FCE7-4FAB-81B8-F77772955F37_2/QvLxpVdN7jeqxD8MMNUvJgQUX6TFuNOnPgd9GA77iGoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/6F24AF2F-3DA3-4212-A47C-7C656D2F1A16_2/6wc1dje0pnweysbcga9FtFarToeVBtaTGydzu4d32r0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/B3EA118D-6BA9-4D14-8660-E86739682C18_2/j0gfADgPTAgXtQBWqmX3DhFFNL1mXqELxDAovvMRAxkz/Photo%20from%20Library.jpeg)

### Photolithography 

Before ARC

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/2BE2C180-1DCE-41ED-986C-B9DC21E01877_2/9Sm3KeVh4MpXmWk5Wlz1wWKrDvQmcosQIQenaqminJMz/Photo%20from%20Library.jpeg)

We are going to process both wafers together during this run

Run failed, and it won’t take my wafers. I am going to strip the arc from the one wafer that was coated 

Below is the bow

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/2A7B36F4-4EE4-4A73-B6DD-C753B4C6F374_2/MyRfSSFM3ycfyfLK9hgZmzEyjGR7ns8HybmtIuBLiIwz/Photo%20from%20Library.jpeg)

Color changed as I stripped arc

Other wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/705991E5-B17D-44BD-8D83-1E0F70C3DB48_2/1Gr6ZmvXj6Tx2UkXNFkJe1O9Beem59SSljUPhtOysK0z/Photo%20from%20Library.jpeg)

So there are fairly compressive wafers

Below is the thinner 800 nm wafer (which worked in the past)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/A00301CF-B5E0-4C6D-85CD-51450C69B526_2/IiYZKscjMjuiRXaKuyUXgMMIpDqLuFkKZTkn3iECfd0z/Photo%20from%20Library.jpeg)

The end point, as sad as it is to say, is that SRN3 at 2um is simply too stressy.  I don’t think this can be fully blamed on the oxide, as the SRN3 is quite compressive.  The solution instead seems to be to make the SRN more tensile.  This should be possible with some short anneals.  We are going to take some of the SRN3 wafers and do some RTA.  We can start at 400 C and work up in steps of 100 C.  We will dwell at max temp for 5 mins.  The hope is this can help correct the wafer bow.  Elsewise, we do SVM and make a waveguide that can test the taper.

### RTA

400

Calibrating

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/FA17DD50-6265-40DD-8212-A81EE9B60CF3_2/Uu9X4LtdStS1xQcZO9YjPiiieaZN4kZ5umzGgPDM3pcz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/5D6EE50A-C880-44C3-AAF5-50DF826FB395_2/yytIFppKzy5AJiOaejOEZ6EE0U4yKnfxOZjDdVS2GGsz/Photo%20from%20Library.jpeg)

After

No signs of cracking

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/DE9324D7-8005-484B-8F99-694DB9AFB0A6_2/VlJWyVaqo6tntLpH0dM7lK0NnHRvKawniidRVLtK1Yoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/522D7A61-023F-4235-AF03-1A25D74B56E6_2/GnOf3rTgSnlnnAYr4MUyxhxTOmqNd59HNfPBi3AgC1cz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/8666AC4E-5703-4B83-B8E4-781B80FBD30A_2/YWpOxyA3HxTxaZRLOVe345iys7OWywidCRDkPWyt3cwz/Photo%20from%20Library.jpeg)

If you noticed, stress already cahnged sign.  Lets do another at 400 just to see what happens

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/FE1D68E1-CE5F-464C-A113-5F4CF465352A_2/yXBGWwJhYkcHHZA1zGJUsr9Hjf69MqGzOx6xtnreLz0z/Photo%20from%20Library.jpeg)

After 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/A5E3F337-DD35-4A30-82D2-128CF7A6D186_2/4nJlR39jlqg9gJxLpFTGv3FFDcRAayUNQk5fKaXUwgQz/Photo%20from%20Library.jpeg)

Other orientation

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/70763364-D150-40BA-AFCE-94B577298706_2/AMvvJEtp1esj40akMTOSTtL6yOOlWUqAg35U2kZAl0Iz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/F22FB2CB-39C9-4654-AEFD-DEC8F4C618A2_2/6GPsFEpHfBryRk6RWQFSrSgCilFSgLYlr7353q86vlkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/42300F54-3AA1-4DC1-8E35-34B655396E79_2/t4DBHxsaf5sMwpVjsYTCSQPeuIvaWVxsQV1Ud8WHyC4z/Photo%20from%20Library.jpeg)

I am going to plot the bow below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/A4B3C8A2-AB1E-4271-9B5B-C400508A52D4_2/TBUvTWmQ7lqMgUmVCW2EA4DlMdOH3uHnLyJdt08RFOgz/Image.png)

Below are the things we learned:

1. The gamma needs wafers with minimal wafer bow to operate correctly. Garry claims we want low bow compressive ideally
2. The SRN3 (with oxide cap) start with very huigh compressive bow at 90 um.  This makes me suspect that the SRN3 (after deposition) is somewhat compressive
3. RTA seems to change the material stack (most likely the SRN3 layer), such that it is more tensile.  
4. The index of refraction does not change much as we increase the RTA time, but the bow does.  So they are somewhat decoupled
5. It seems the bow changes with RTA time.  We get the most change at the beginning.

It seems we should use the other SRN3 wafer and anneal for 200 seconds at 400 C.  This should give us something functional.  

Baseline measurement of the SVM bow with oxide cap (as a target)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/5E604C4E-866A-4F95-ABB9-062C9FDFB729_2/0Xnm6qpH5Rxb95iPGTyc4LBUeKUB2REVmcpPzVyNEb4z/Photo%20from%20Library.jpeg)

We are have a baseline now

Front wafer in box is the one that we did RTA to.

We want to make the back wafer work as a final device right now.  Based on our above characterization, lets try 180 seconds in RTA on that wafer to see if we get the right stress.  Below is the baseline bow measurement

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/291BFD06-95D0-4E2B-A91D-BFED168ADE75_2/hCyaF58ddRloxRjyJkU9gTUxCoAFgcexWx2MYAtkn5Mz/Photo%20from%20Library.jpeg)

Calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/12CCDA72-4637-455A-A06F-DD9168219733_2/yZgo8pAqAFxfesIhU6VCXxvGEMxfg9Xp1hp3iZzfK24z/Photo%20from%20Library.jpeg)

During main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/8A65878A-8D19-401F-BA3F-250A65A6C2F1_2/gLb8dbZvIOkmkuA99S4V1pS2vlYaDlBxDmbYAA6gygkz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7B7302E1-0CFF-47AC-B3D0-41B40CE2732B/B1CDFB4C-A5F7-4F85-AA63-9C34F5A45F9C_2/5Azu4A7zyZsu33b6qHeLj40ujmPsZ08tlUyRWd3aT00z/Photo%20from%20Library.jpeg)

Re clean in piranha, starting with back