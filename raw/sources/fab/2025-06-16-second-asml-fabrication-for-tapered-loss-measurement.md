---
type: craft-export
title: "2025-06-16 second asml fabrication for tapered loss measurement"
craft_document_id: 28A12122-DB8C-4E6F-9774-C520338398A5
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-16 second asml fabrication for tapered loss measurement
We previously tried to fabricate tapered waveguides using the MLA.  In addition to the mistake of not removing the edge bead, we seem to see very high loss.  We know the staright sections have the same transmission as the ASML (they should be almost uneffected by roughness because of the way that the MLA writes).  So the high level of increased loss is really only an issue because of the taper.  We roughly suspect that the sidewall roguhness is very high (or there are stitching errors).  Because the tapered region is very small, the waveguide mode can really feel these effects.  So we are going to make a new ASML mask for tapered spirals (attached GDS below), and fabricate new waveguides using oxide hard mask to test loss.  I am using oxide hard mask primarily because the recipe is not perfected yet in terms of final oxide thickness, but we know it shold give very good loss (from measurement on previous ASML devices using the older mask).  

[ASML2_Pass1_Negative_Final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/AD55F93C-1A5F-44DF-BAC6-8F75D5B527CB_2/N9Lt3ooYVxW7QAEOzCAIMkYYCAXK141lNlJOb8mgqoMz/ASML2_Pass1_Negative_Final.gds)

On the mask, we designed a couple of features.  Firstly, we have a default bottom alignment region which we will stitch to other top regions.  The dies are roughly the same size, but we should make sure to extend the bottom one a bit to make it line up as I want (as I want plenty of cleaving distance).  My main worry is about stress explosions as this point, so I really want to expose most of the wafer if possible.

We expect the 3um tapered region to work best (refer to simulat overlap integral results below).

![Image.png](https://lh7-rt.googleusercontent.com/slidesz/AGV_vUcAt286TzurdGBoFz_PASBOTqZNlCqCURknhjxRYaWS7f7_UAamdpS8V-d1gbjwP0KrIoehStGePWPE3gypec3wWv1eg_Ylz_6mX3T8WE1wOvIkh_BkGMKNgAqlcucrb9lg8dPy=s2048?key=__A0WojhaDz9ffNJM0-D0g)

![Image.png](https://lh7-rt.googleusercontent.com/slidesz/AGV_vUduLhnepHG4rFpKwG-mRntbEhiZK1V6n6PfL14FV1yBhMOcccn_SGcX4zq9bopdE1n5uzU7FV9dRV9AgwWvkJ6fb7EbFw9uqXS3CxSHZ0ahRvHvb9-vn2xoBeDBAAn7VgYUQ15k=s2048?key=__A0WojhaDz9ffNJM0-D0g)

We also have some longer waveguides at 2um in case they work, but these are a bit optional by comparison.  We have everywhere roughly 3 mm of taper region on the spirals.  We have some adiabatic waveguides at the bottom that very from the widths we use, so hopefully these will reveal if there are any issues with taper loss.  We also have a non-tapered euler spiral at the bottom for alignment.  

### DWL 2000

Before exposure

![Photo from Library.jpeg](../../assets/fab/2025-06-16-second-asml-fabrication-for-tapered-loss-measurement-003.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-06-16-second-asml-fabrication-for-tapered-loss-measurement-004.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-06-16-second-asml-fabrication-for-tapered-loss-measurement-005.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-06-16-second-asml-fabrication-for-tapered-loss-measurement-006.jpg)

During exposure 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/11D84FDD-92B7-4B91-A75D-A4A8D970ED85_2/gElD6oKQL4GEI1e8yx5CPmd2JhMkWiiMHKYoLMONR4oz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/8D792F9D-21F4-4AC7-884C-CF6A3AA12B9C_2/LuAi9ijHmcHgYWxoMp7PjzEd22iX6yfZ6G2CMhl1Oqkz/Photo%20from%20Library.jpeg)

Before developing the resist 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/EC04066C-08AE-4038-A349-56CABD6872F5_2/KZ5S0HMtoAAG1udyIE4S2giVbpXqXRKnCet7OKuIlcUz/Photo%20from%20Library.jpeg)

Before etching Cr

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/E7F52D88-242B-41AA-91C6-DC5436208052_2/2aQsulxh46BfMkU4gIsEmHXYQQAl7Lqq1qowvkq3Yt4z/Photo%20from%20Library.jpeg)

Run dry rinse and mask is ready

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/0B4F0E9B-F352-4F2D-ADAC-F60182DF4C5D_2/yaSX4SxyxyWXAa4MSfZHqnpzO8f9Mxy9ylsUaZgqnSMz/Photo%20from%20Library.jpeg)

### ASML job

Die distribution

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/F788D61E-C3B4-4B8C-BD3D-0B5D86EE632E_2/itTDdO108cjxAR4yPCW9Lojt03YRrxKx2iw0RTgPhjAz/Photo%20from%20Library.jpeg)

Image definitions (I made the bottom a bit big, which is fine, as there will still be Cr to cover up)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/1FF98A9B-1B1F-4E34-A640-8D9D42E23C87_2/TKTo5EBUPD4CClPcHCf5SN27N3yhyjO3xGNbbKmG1AQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/8A9AD0DF-0EE1-449E-99EA-A8655C7C48D2_2/OIbtbmGR8AImtcwYwF1eocqSpo1F3be1Z9MAX6wLN5cz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/0F87149C-5249-48F4-B540-3A89F9329FC2_2/2w5yIRKrEsBgd2bbFLEZcdTURDytMCkR62hwP76SUIwz/Photo%20from%20Library.jpeg)

Layout

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/B988935E-D645-44EE-A2C6-3F89C932A4CC_2/vzJ9EIlyD8rfM9ky7Gk1cP2Z4p9G7oxGldx2vYisMNgz/Photo%20from%20Library.jpeg)

### Photolithography

We are going to use the hard mask recipe.  We found last time that there was a lot of resist left over.  So we are going to use the 600 nm resist recipe instead of the 800 nm resist recipe

Before arc on hard mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/FA4C1F86-0280-40FA-B973-FFE33381B50C_2/yK2CrvPBf4XoxG9Kyoe1AVJWRZqLBbk8ZvCyWzyUUacz/Photo%20from%20Library.jpeg)

Before photoresist

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/A5DBB12C-5B19-4F12-B046-4110507DC848_2/BpAxQfBGUkbBJWjXomPF8LVmqXNpkskz5mh05XjlatEz/Photo%20from%20Library.jpeg)

We read the mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/00402F22-29DD-4AEB-A234-BED5D49F0B58_2/KUjkKVNSX2Avq0vcBEiYW6K4u1WTdxBeJTyXSY30FOAz/Photo%20from%20Library.jpeg)

New edge clear recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/A6678232-AF11-40AB-AB46-8C0EE356619C_2/8BdyiPQZ8FRxIJNqrMzfX1WqtHCdm6qZFDexYRiVjSgz/Photo%20from%20Library.jpeg)

During edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/5E1D38B7-DC81-42B9-B3B0-47AFD2E3338C_2/kOOVqCK447dGvHP9D0E5zol1XSyXF6ySFQhAwE5N2D8z/Photo%20from%20Library.jpeg)

Before main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/28658E43-62F9-4F82-9E24-DB894E5E6537_2/ZDM21tWSrvC4qB49McB8hyNgq1DXB6ZOru4xsNGLGOEz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/50A5F913-B075-453A-828F-2A3CAC5D57F9_2/rD1Tz3ABTagwyrR73HPV6psoisJxT4VrTdDcbyq2NDwz/Photo%20from%20Library.jpeg)

Before developing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/058D8A92-16AB-4677-B835-77F17D58BB05_2/XEI4MYxUO6CymtIlsjECgxLcjy56wA2LO9HfSuqU4bEz/Photo%20from%20Library.jpeg)

### Etching

We run 5 min pre clean on 82 and 10 min pre clean on 100￼

We run 1:20 descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/6DCC35AD-B342-4E1B-943E-6A96265E2034_2/M6hE4KBYuSPkW4aGymJM8nAqCdta5KPBybokYoXoxcEz/Photo%20from%20Library.jpeg)

1 min season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/1A5C7DCD-3ABE-4FA0-BCB0-DDE2C6FABCB3_2/9LPabTUC2h54bkVHIy7JppGDs6bHlJBXaYsTLwyw4Ssz/Photo%20from%20Library.jpeg)

We will still do 9:30 min etch so none of the polymer hits the oxide. I still see a small amount of arc left, so I am going to do 25 more seconds descum

We also setup the job slightly wrong, as there is no continuity between straight regions

the extra 25 seconds did not get rid of the faint streaks of arc.  I think we had a bad coating or something.  We can insepct more after the etch and see how bad it is.  My worry is this will add a scattering site.

During oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/EA7118CA-D97A-4EB4-9972-72F6C3104F91_2/2nk2M1ED6lOUBu2H1vqo6zGpJnec8njlE593sWyOxckz/Photo%20from%20Library.jpeg)

We still have stability issues during etch. Should do closer inspection. Our He flow is also very high.

￼We run a 12 min post clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/3296D6E7-9B03-409B-9F8C-98DC3EFF71DB_2/sYz07BPv7CioQXPm1pPmrs9QgPYFu4DzlPFbq5WvJqcz/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/BCB9014A-835A-44F2-9B47-A9EF89ACBDD5_2/LoBaqgh4XiqevxPWwKDQK0xL2xqjKkIDggiw6jFZcvIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/C40F43DB-1E64-4793-A182-437A4010D613_2/lSek0cyA5MmH32CX3beWfCkHF4Y1UrelQ4GVe2763dkz/Photo%20from%20Library.jpeg)

Microscope 

Effect of remaining arc

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/3673218B-DD81-40C7-B927-49B6536604C9_2/Nb8RNoPsz6WUx5tExJMxPIL4invCgg7ajW9h1GbWWKoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/AE8D9615-2391-4092-9D86-85F9AD071F51_2/U2EZk9mx2jxEL7nyOeIGMhEv3cXnM7sxKeEfbJpLwg4z/Photo%20from%20Library.jpeg)

2um

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/0678C14E-A611-404A-8A1D-BB239243CDA5_2/wUOyHVOyhkzsV9yOFOMolHV42r7N3pcWcDUYdQxV5Acz/Photo%20from%20Library.jpeg)

3um

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/CEB1B176-705F-4E2C-8479-B7ED8B11ED5D_2/27BFunCGeaCEWwoI9ukfqbCy6Lyss4p1MyjO8Ty7Qx4z/Photo%20from%20Library.jpeg)

we run 3 min SiNx etch season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/3A4E1A52-DE78-4574-97A3-F32017A48970_2/l5d4ysPDWovGdKyw303DGQDETFytfg9NAKOMd6TFzPwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/2AECF027-3766-4479-B630-CAF876F14C4E_2/4rrjLyFnNhkcaN37xuPzxMjxtx7QN6N20nEl7PWIsyMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/376E094E-D25D-4223-A637-34CA4B916B79_2/6xh5mKMqx1947w3kFYaizFB07JVmhxoyYHYbH18yqHwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/521CDC77-997D-43C2-8812-AE258EDD7F64_2/MtLtayEzYMpRGCcfDPibZWXyzJCNFGbo1kW0oxxrJPYz/Photo%20from%20Library.jpeg)

we now do 6 min SiNx clean

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/F3325809-5C2B-45DD-950A-D63D52354622_2/Id1xlgZplyP9JM09BDltfGOmRP9l8fw6GDBnFTIF4ZEz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/C17B6EBC-031B-42B7-B0C5-522952F1ABAE_2/myg3sYMChwzWSxIruHVGy0xHDOlmFrsx64kEx2bMSrsz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/305E0B87-7479-45E6-8A7C-099CBB95F972_2/Q4U1q31lMTWfcaQWGSqGTl5duoQ1JI9MGMtVCRPm9yIz/Photo%20from%20Library.jpeg)

### RTA

Calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/97140FE0-913D-4B6C-9301-50832FE2DDF6_2/HYFSpdF31aKi2Yhh4M6M9fuTOUMC13kiEWgRVvR3Ixkz/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/759864A0-EE88-4FF7-8C22-6F1397B4BF1B_2/KIxPDRfeFVxt2ZX2IXOszKjxMba5i568ixOUeJvDgfgz/Photo%20from%20Library.jpeg)

While we normally put oxide cap on first before annealing, we have annealed shortly after etching in the past with no loss issues.  The PECVD is down right now, so that is why I am skipping that step.  I worry if I let things sit for too long, dust might collect.  When it comes to arc issues, lots of dies in the middle are ok.  We probably have issues with 20-30%

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/4270A9DF-A4C3-4567-9F5F-5D090946CC7B_2/idK10FkGGTMlxlxs0dZuRaFk9EpC9JVPcD6zH7ecyhoz/Photo%20from%20Library.jpeg)

The bottom ones are a bit annoyed by the arc issue, but there are definitely enough for a loss measurement.

### Loss test

Edfa 10x 1570

Straight 1

3.5 mW

Straight 2

3 mW 

Straight 3

3.3 mW



Slow wide adiabatic 

1.2 mw

fast wide adiabatic

very small

slow narrow adiabtic

0.2 mW

fast narrow adiabatic

3 uW

Keep in mind the above numbers could be due to unfortunate cleaving positions



Small Circle

0.3 mW

Large Circle and Euler Spiral could not be found



Die 2 (3um)

Euler Spiral

360 uw



Straight 1

3.2 mW

Straight 2
3 mw

Straight 3

2.8 mW



Wide Slow Adiabatic

0.8 mW

Wide Fast Adiabatic

0.85 mW

Narrow Slow Adiabatic

150 uW

Narrow Fast Adiabtic

110 uW



Short Circle

200 uW

Long Circle

44 uW



This is indicative of some higher propagation loss in the 6um wide region



2um (completed with 4X objective, so powers should be ~4x larger)

Straight 1

1 mW

Straight 2

1.2 mW

Straight 3

0.9 mW



Wide slow adiabatic

0.6 mW

Wide fast adiabatic

0.3 mW

Narrow slow adiabtic

160 uw

Narrow fast adbiabtic

80 uW (328 with 10X)



We are now using 10X

Euler

750 uW



Short Circle





# SEM

![Image01.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/7B7F3F6B-E38A-46A0-865D-193C26200EA1_2/c8pa2B9G4vgbUYHhc0xIFdbJXpgW0IueZiqNyZHFY0Qz/Image01.tiff)

![Image02.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/3EC7A62D-397A-45A0-8AF2-AC5397C7BE5E_2/2y7qG8m4x61XTyfyfyOupoKK9W7ba355MuMtw8eZ2REz/Image02.tiff)

![Image03.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/0720D74D-BCF9-4DEB-89E4-B2EC36C9B9A3_2/7iiDfDKh8YYuCTSl41uWuEZbGILKFtU3cLbyvaoHdw4z/Image03.tiff)

![Image04.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/C0E75918-06BB-46DD-A674-9D03D00094FC_2/dfdHYPJizU9OLPiBLxV0LKSSoV890l1jeE2BD4Yy0eAz/Image04.tiff)

![Image05.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/4BB8B5EE-B664-41FB-911F-E7104516A22E_2/jJylXyF3TCQGoPEc7iIEygn4EhJPjwOu5i2UMtyapAsz/Image05.tiff)

![Image06.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/43ADAFAF-F937-4411-9863-7C82A98F6713_2/bHjXJCRu4My2fmgqHjVfufeH7xep1lyThvEvE1Q8abEz/Image06.tiff)

![Image07.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/9C535B1C-4388-48D7-8291-9855491D0045_2/DFuYdvIDlkV4ZPBcwJj9ywwZuNVL0g1lWwSeWyhOid0z/Image07.tiff)

![Image08.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/0752FED8-3C3C-4F43-9969-DB1924FCDCC0_2/7wkcJT9pJDdCil4Jbd3gdc2MNVlMyayU9xXxJozVJPgz/Image08.tiff)

![Image09.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/28A12122-DB8C-4E6F-9774-C520338398A5/E8ACC77A-0308-426D-A0B6-C7F795B73338_2/KlcDHLV8iZavCbgJ8PpfzTFknBfjY0lQlvvO8dux4LYz/Image09.tiff)