---
type: craft-export
title: "2024-4-8 ln dc device bottom oxide exploration"
craft_document_id: 1E788CFD-48E9-4B57-874F-1D2CBD3F7086
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-4-8 ln dc device bottom oxide exploration
Given my simulation results today, I am interested in developing as conductive of an oxide as possible.  This film must have an index at 1550 below 2.2 (to be a useful cladding for LN).  We also need low optical loss.  



As a summary of out previous results, we found that B6 (N2O = 110 and power = 5W) had a conductivity of around 1e-7 and index of ~2.05.  While my fabrication technique (3 intervals) was stupid for the optical loss measurement, my B7 results do make me susepct this really did have onerous loss.  B7 (N2O = 135 and power = 5W) had a loss of 5 dB/cm and an index of ~1.94.  No conductivity data.  This loss makes be suspect that having oxygen concentrations below this might be a problem.  Given the trend (minus the B4 outlier) I suspect this film have a conductivity of ~1e-8.  This is already fairly close to where we want to be.  This makes me a bit nervous.  B8 (N2O = 160 and power = 10), I saw really low loss of 1 dB/cm, but I was not able to take conductivity data.  Index data was also hard to get.  The higher power might have screwed up my conductivity, but we had great loss.  I think, given the lower loss that the high power film achieve, we should try B6 and B7 with power = 10.  I think B7 is the upper bound of 5W perfomance regardless because the gas becomes hard to light above that.  Maybe we can try small scans of power and N2O flow in the future, but I would prefer not to do that if possible.  We can also take smaller N2O jumps in the future as well.



Given the conclusion above to stay within the B6 → B8 N2O range (because of conductivity concerns), B9 is probably overkill.  I want to use 10W because of loss concerns.  I might also want to anneal at a low temp (800 already broke my films so below that) in case I want an extra degree of freedom in the future.  Below are the recipes:



Recipe B6*:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 110 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Recipe B7*:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 135 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Recipe B8:

Temp: 300 celcius

Pressure: 1800 mTorr

Power: 10W

Silane flow: 40 sccms

N2O flow: 160 sccms

B2H6 flow: 133 sccms

Ar flow: 475 sccms.



Ryo said he was able to see good signal with chips that were 1.5 um thick and 1e-9 and 1e-10 cond.  Because I want waveguides (these are also slightly higher index), I probably want to deposit B6* and B7* for 20 mins on thermal and vanilla.  B8, because I already have it on thermal and have characterized it (those wafers are also in short supply), I will just do 5 mins on vanilla to measure conductivity.  So 3 quarters vanilla and 2 quarters thermal are needed.  Check wafer boxes to see if there are any bare vanilla or thermal quarters floating around.

Below is characterization of vanilla silicon wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/F9ECAD77-6249-4BC4-9257-2060B0779F70_2/k9UBC0ymt3G5CpFO3wcqZzjOyGSbWg6I1xW1Nj4FBuEz/Photo%20from%20Library.jpeg)

And for oxide

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/165B991A-A2C5-4812-A75B-2C26EF16F367_2/qxsYEmNqoCu96emcsMNj1tKVZl6obYhWKvRNjo2oNZwz/Photo%20from%20Library.jpeg)

We spin cleaned the quarter wafers and are doing a 5 min preclean on the PECVD because the carrier wafer was left out.

Below are the boxes the samples are stored in

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/D737AC4F-B6C1-49E7-8529-59FDFCF0C2F8_2/vjS0z2DSGAQXELx3qs5FP7IvyaVRBnNe1dcjxOuvDA4z/Photo%20from%20Library.jpeg)

We are going to do B8 first, so we can do ellipsometry during the last longer clean.

Here is the recipe before we get started

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/B038FCA0-2659-45B2-814E-F66B75C63AD3_2/ZcTf0WUS2CzS8N9wCF7LuoLwZZcFb6IeZ0O6GyIXqa4z/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/882FC5C8-F574-4868-A10C-91766554F8C0_2/ZqmQQETQj0tVTsQTJDR5Y4fnuFrCz2AFTB5V6QjJiQ4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/2A729248-60D7-489E-9661-563669B4D9A9_2/vcxr4GN2Y9F5Xwe4scyx4BVL66rqpBsg7oVatKIy7HUz/Photo%20from%20Library.jpeg)

The gas is lit and everything is within parameters, so I say we should be good to do real deposition for 5 mins

Blue color we are used to

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/49316085-89DF-473D-AC4F-5CB509268AF9_2/P7g1UKE32xjx83fqDJCqE39JjgLTutrysGuCyD3lh4kz/Photo%20from%20Library.jpeg)

During the actual deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/90BAEEAA-336B-47BF-A1B1-162ACBC0B10A_2/vv116jUOE3Yw2ETbVahPtxwzZ8onfD3J841AlY7VJF4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/39C91D00-00E5-4E58-84B3-0D3C10F058A6_2/SJXoGpKsxix8nsJGTxyjaZOdx8wY6rou3GvT0Pw9ptUz/Photo%20from%20Library.jpeg)

After deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/751095B0-7963-4D39-A293-0164B6625FD5_2/PnSC0u4BK08SsEHB2MFyTujGdPRSm6UGC8iguZhmvU0z/Photo%20from%20Library.jpeg)

The orange color is a bit new. Before we had purple. Probably higher power causing this more than more oxygen

After  B6* seasoning (forgot to take picture during)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/656F4D6D-1D8B-4590-9D45-622CE124F910_2/xR3eZ7Q4vRWQ0xHzyeRa2sRSb5jeDoA4DZsGSckKHVcz/Photo%20from%20Library.jpeg)

Normal blue we are used to. I am going to put oxide wafer on left and vanilla wafer on right

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/1ED86A31-048B-4724-952A-A1CF3A2A248B_2/y8ScCbelGtGrIq20E4OvyuxWTBtlvzPCp0iWU4I0F2sz/Photo%20from%20Library.jpeg)

Screen before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/F7B1D119-17EB-4900-8E1C-796BBB85E649_2/u0y2CYI5a19GAsPuhL9iSf8S2O2tTxDEVSfkv7MJLgoz/Photo%20from%20Library.jpeg)

20 min dep starting. During dep:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/5369695E-3D71-45A4-BE78-C004CB23B0ED_2/HX589g72AGeR6ZQGP673h4Uy4EDid92dHt1llO9YZngz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/296BEF5F-A35B-4B55-A281-3BDD6B6F6311_2/aifbAUg3rjQpzSwvceTtC9PH8VnPMJ0iodbTPaSBnxQz/Photo%20from%20Library.jpeg)

After deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/6B4B996D-4732-4508-BA23-A24C2487FC7F_2/a2gAMasj7RW7ZTucbBMJGFE3ooxAVu2jR3PJdnlmdcMz/Photo%20from%20Library.jpeg)

Uniformity is really good. 25 min clean is now running

Before B7* season:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/A211DE02-2E0F-4D67-928D-A06E13A87C65_2/jsYlFii3IURWkxTTg4LPxjlWyfCWdyfy1aykbPj8kDwz/Photo%20from%20Library.jpeg)

During season:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/A662ADB7-D3B6-444C-8096-93A6EFFB4539_2/a8vnoyJyD7p0EafzyBbzeEawR1m3DQjDyY8mGCc0vsAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/13FF6F7D-C274-44C1-9471-AC1C25089328_2/oO48telhGNyMwGxcBvh7HC9JUE9N86MKnbqj9hilAYkz/Photo%20from%20Library.jpeg)

After season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/FDC5BBAD-E0CD-4900-8763-A1D88B979432_2/HWqQZl4Nh0WnP0vYyfX6QHAHvVnsMkolw6lYXlr9nTMz/Photo%20from%20Library.jpeg)

Nice and blue. Let’s do 20 min dep. once more vanilla on the right

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/4F34F2B0-7EAD-4DB5-AB5B-91DE28687EAA_2/7gqNbWQrYZzMiGBcQX2jyNRt3ZFUDBp6a46BJ4AiX5Iz/Photo%20from%20Library.jpeg)

During dep:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/759FE021-51F5-42C6-ABEF-B4348F2DAA45_2/YiJZe18gnghoQWfZWK8NycRX22IJS6ukSfuWMDnyXI0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/11711D97-BF5B-4589-AB11-22DFAA561EC8_2/GkJyOcmLai2CcOvI8wQZJPbKmNHwLkxgITpKy1VSev0z/Photo%20from%20Library.jpeg)

After dep:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/9E196963-6A79-457D-84D0-6E75CA6B727B_2/Lsj7uxIFimQfXET3ckdiBPbQlD4wFbT1lEu59P0L0tQz/Photo%20from%20Library.jpeg)

Now time for some ellipsometry:

B8

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/64F8E4CD-B162-4631-9DEA-C51D7678B3FB_2/vIbNA3eaUqdfeedccOcS0AtYIrssTDlviWkQgeiFvxgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/DD112625-3302-44F8-9EC5-3FBC570BB620_2/R043JI7WxTlUxC81JgywoeluT8w7z9OXPs2T8VFzTqoz/Photo%20from%20Library.jpeg)

B7*

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/3860F4DE-255A-4EE4-B53C-BFD94EFDF94A_2/vBQH2yQzI219TSWgYfxHy3sxUXygQbSHSehyfpc4VkMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/12A0A541-6F15-4981-A5E3-4E86F7425243_2/3onRpHktxnDlKVxDRVDvLeCsfSWS8CMed0Z3KOYZdEQz/Photo%20from%20Library.jpeg)

Only a small hiccup at 45

B6*

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/D115811E-CF7C-420A-B8F3-4016BCA069D2_2/x3t22cu8UUSgnV2Ytl2AVK0mrWbF9TAqL2TAxVNBWBgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/C719C6D1-BC15-4390-BE99-00BB77FF9EF0_2/M07EECoEWKxwRjqlCfmdK1vPDE0zKDEaK0SdYyXNvdkz/Photo%20from%20Library.jpeg)

Now onto the even-hour evaporator, where we will deposit 10 nm of ti and 5 nm of au.  The indexes above are about 0.05 less than their 5W equivalent, so power does not seem be have a huge effect on what compounds are in the film.  My worry is still might not be conductive.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/2B80A7AD-143F-491E-BEC7-DF7DC586BFD0_2/uM6BqhM9JMfPBBunNqF9ub7APQAaqDv3f9hnTjWOmI0z/Photo%20from%20Library.jpeg)

B6 is top left, B7 is top right, B8 is bottom middle 

After taping

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/5AD19F3E-09AD-41C7-B80D-4114E0DFA67E_2/mcgUyl4Dk4ZPY1wnenDRKwMDsfhQzZo5NwXlHPwamY0z/Photo%20from%20Library.jpeg)

They did not seem to have the small tapes available unfortunately 

Life is ok

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/F949BCB1-C561-4819-A24D-57E5039A5CA9_2/ZcvGdyQj0YDnbIu6IMx9tVkmpEvyjFyyAFa31KaWvoMz/Photo%20from%20Library.jpeg)

Samples are in

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/21710FD8-AF51-4D76-975A-D7A5C877608A_2/GDL7fBOnDnYxuLzzD6jTqrd4uOTR3HPrl5nphx1d58Iz/Photo%20from%20Library.jpeg)

Our pressure is low enough that we are good to go

The Ti seems to have a somewhat stocastic dep rate. But it is coming so I say we continue

Seems to be between 1 and 1.2 A/s. Power is also 10 for Ti, which is a bit high

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/53AEAC6F-4047-4BCA-9F38-411DE892125F_2/rRJywOahdKbgvARf71x0im7jrabrJfpwrSb7PSoj6u4z/Photo%20from%20Library.jpeg)

Now for au

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1E788CFD-48E9-4B57-874F-1D2CBD3F7086/B0D4A707-AC79-44AF-A292-4EC28B7C9233_2/ZT3koO1pyxhKA0aJMxEUuhpLLRQd1g1JwyyBqNBoRZkz/Photo%20from%20Library.jpeg)

Gold had a normal power and the electrodes look fine to me.  We will see sheet resistance when we get into the lab.   Everything is unpacked and ready to be tested!!

