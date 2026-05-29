---
type: craft-export
title: "2025-03-20 rta and electrical capping of negative exposure 3 and 4 layer devices"
craft_document_id: 5C28966C-D039-42A7-9F0C-7C87037C0EC5
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-03-20 rta and electrical capping of negative exposure 3 and 4 layer devices
In a previous note, I fabricate three layer devices and four layer devies and used a negative exposure pattern when lithographyically defining my features (which is shown below)

![Image.png](../../assets/fab/2025-03-20-rta-and-electrical-capping-of-negative-exposure-3-and-4-layer-devices-001.jpg)

We also have some longer features than usual on this wafer (look in the middle rows).  First, we will want to Cr etch.  We have might smaller features, so it might make it hard to see when the Cr is gone.  For that reason, I say we Cr etch for ~20 mins and then do an HF dip.  I think the fact that we have much less Cr remaining means it will all etch away faster.  We will then do a 3 minute RTA at 650 C for 180 seconds with 20 C ramp on the 4 layer devices.  I say we conserve the chips that are three layer for now.  We still have a rather thick bottom oxide, so I don’t want to risk any cracking there.  I will handle this before any depositions.  We may also want to put the annealed quarter wafer into the Cr etch bath just to clean it off for later depositions (as it has not had protection for a bit and this will just get rid of BS).



For cleaving, I did make this wafer rather hard (and the dicing saw is down, so no dicing).  I would assume the easiest way to do this is cleave in the middle, try to then cleave the left quarter off.  If this does not look reasonable, then we can cleave in the middle and have a few 1/8 pieces.  Just make sure to cleave through the waveguides when doing this in the middle.  We can probably cleave the left side waveguides more easily once we have seperate pieces. There is a fair arguement that we want some of the middle pieces to get longer propagation distances.  I am against it mainly because I am assuming losses will be too high at the moment.  For first study, use the less valuable pieces.  So we should try to have the two pieces below for the 3 and 4 layer devices

![Image.png](../../assets/fab/2025-03-20-rta-and-electrical-capping-of-negative-exposure-3-and-4-layer-devices-002.jpg)

![Image.png](../../assets/fab/2025-03-20-rta-and-electrical-capping-of-negative-exposure-3-and-4-layer-devices-003.jpg)

I must say, I did not give myself a tonne of cleaving room on the bent waveguides here.  



After cleaving, Cr etch, and RTA, we will then need to deposit TEOS.  I would like 750 nm of TEOS.  Given the deposition rate we clocked a week or two ago, this means we deposit for **13.5 mins**.  We must use a 12 minute heating step as well.  This will be on the 1100 C annealed straight waveguides and our current RTA 4 layer negative devices.  We expect a bit over 700 nm of TEOS.

Next, we want 4.5-6 um of SRN8.  This means we deposit for **23.5 mins** 3-4 times.

For the three layer device, we want 1um of conductive oxide.  This means we want a **14 minute** deposition with the parameters below

For the films, below is the recipe for the cladding:

SiH4: 40 sccms

N2O: 500 sccms

Ar: 475 sccms

B2H6: 133 sccms

Temp: 375 C

Pressure: 1800 mTorr

Power: 10

I might do a few more simulations of three layer devices to quickly double check this is what I want, but it feels fine to me

I just cleaved. I am Cr etching for 20 mins and then doing an HF dip for 15 seconds. I am also warming up the RTA B

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/BA6A0C5A-2B8F-4A6A-90F6-7428A4C1B7A1_2/PMQWK67Zi72iR6KIv52iuVgAKlQizyrMzeurpfbvMdAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/174E9DF7-A34A-4284-BDE9-61ECA023554D_2/HvoGTyyYtmGi3Wo5LijMBdTP7aobz8E5CGdSQxBcdAcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/EC735FF6-597B-46A9-86C7-4FDFA96619A4_2/RWnZyljPO9BfBE8XE5koEmI0YvGDWzyvSdFVzJdHWHoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/9A15562F-DB5F-43DD-8AAF-7C6F3622C20D_2/IPNKXToYN01cjZuwmyh7HML0Qbs9v82JYmvXr2BAXWEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/7305AC0E-4740-4630-9675-12D4BDC20CB6_2/SHvCl4KrLnqBrBnPY9pip7XjjH5Zr8Kb3VB8Zl3ZEMsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/CAFA83AE-1F45-4302-85EF-718D5FD65752_2/zLAadh5v9xK0bWu81wkCUK3L0M6nVJSuZautFTocAAIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/BA5C1CC7-6662-4071-8ED8-A625DC408DDE_2/txxR7DSyG9EJFTZh8ooLXzVLVTHbdx0dMaDb9lOpRw0z/Photo%20from%20Library.jpeg)

During calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/0C556138-C83C-40C7-AFB6-3C97DE48F0EE_2/WdygcoaXhKpauyxe3aCg9xiYl5rnhN6IZdh65fq0Wncz/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/97B90281-A7F9-4201-943A-685C56535C99_2/mySfXmA1Kf0DjRq9FBV1HE91DOu816fDW7y7NCu6QMgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/421DD5D4-92E5-4B00-B781-08B0B378AF40_2/BcmUH7CTwpqON0FkZAyiw6FX6Sbjf7SL7brC2bKKFBgz/Photo%20from%20Library.jpeg)

After spin clean and RTA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/1856F31E-5879-46E8-A068-3C2B74FF0F4F_2/vetM2afqcnJdwQFjEoCgroArXQBhRjsZoV5S2XUbOwcz/Photo%20from%20Library.jpeg)

And the annealed one before deposition )I did a subsequent spin clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/7565390E-499C-4E26-8D11-72BE95D4CABA_2/xxdAfaEaNSyghc1UJQZGUFpXThbSabX34bspMRyOikEz/Photo%20from%20Library.jpeg)

Box

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/7BDED98D-40B2-4FDC-BDF5-9BC989243B32_2/uJ3yNG0xocOTzdlN8ubxKlfBWfhYJDvo2IVpZMainZMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/B340F3A1-EDEE-4FF7-B71B-586668FB19AE_2/z66LJRxcRBphLQCGchV3hS3kayUZeyq58d2AVy2tBsoz/Photo%20from%20Library.jpeg)

Even after hot HCl, nothing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/4A542587-B23A-435C-BD64-6D4BB608B367_2/g81X08p3yfu46GFpHJRy7N7jK0XLjgoSyjvu3yqULfYz/Photo%20from%20Library.jpeg)

# [`Thu, Mar 20`](day://2025.03.20) note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

## PECVD

### Seasoning TEOS

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/22E80021-FCF4-498B-8DC1-879CF0E91DC6_2/BM5GKOX7AyuAolaaKZ1kv1ZIggAESu2PWvr9az0T2Qcz/Photo%20from%20Library.jpeg)

Samples

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/CFE6BC92-0F26-4ED0-BABE-1CC6EB105251_2/eW5gqeb9GBhgpfo8bSx5MVb1MaZS4iSOyqfYutjR8UUz/Photo%20from%20Library.jpeg)

There’s a red alart

Talked with Jeremy. It’s fine to accept and go ahead. This is caused by the leak of the bulb.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/5DE2DF31-58F8-44CD-90D1-6AA7AAC49D67_2/tGdSSiqAAaKjyvqrhpw9zwTbzfBTG7yK6YTiygsUEREz/Photo%20from%20Library.jpeg)

![IMG_0581.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/20DC6BE1-8458-437C-BE52-9411328E0C74_2/fOuxiZzj0TTFWSSSP0hGtIhkfSZGtWOS4ityjCKFb0Mz/IMG_0581.png)

1 min seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/66572A92-8703-483E-BA04-AD94D27F28F0_2/T3cwmKUGlxhPL9Ch7r4dTm12He8krxOQT0qoTIA3UkIz/Photo%20from%20Library.jpeg)

15:08 Venting the load lock to load the carrier

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/B6085109-D010-4371-A5E9-D003254BC0F4_2/ySdMBUDhV0z7G7ixWmaSSQKqsvNMzqsu9ahyeNgxEe8z/Photo%20from%20Library.jpeg)

15:11 TEOS seasoning 1 min started.

15:20 Seasoning finished.

### Main run

![IMG_0582.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/C55D01E1-5E56-4239-B807-0C3D78597F27_2/oIUdVKsF1zxer9elo6eNp30NGhyhyqLsiGZg0NNP69Uz/IMG_0582.png)

15:20 Venting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/9196FA57-CE4B-4048-A628-AB7ACE4687C0_2/I7Wiqsp4MOaGItAY7KBsZTFUTQ35UenbX7e05iMVZuUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/07853E6B-1AB3-4964-8E01-E43D4FE9EBB1_2/se3DAhxtkJovFmxQCqpM9cBwJhfyaZU3cPgpB14lejwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/E0B464C8-0839-4B8A-B2F1-F5C59200DAB5_2/ipsr5Lk2MiE34QAyQsSGu1GS4yLqnc24v2bfI2P9rPUz/Photo%20from%20Library.jpeg)

12 mins heat

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/78AE6B31-1AA5-4C79-AFC5-1CCD2D10AD5D_2/pxvulx2DivGP2bXtyoXuiUnVgDry9VEvpsaFSk9JDDYz/Photo%20from%20Library.jpeg)

13.5 min main dep

15:56 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/6A4F1956-1ECA-4495-BD12-DECD2DB03BF0_2/Ll5NUNBpo5H5Toa995OUV0qkHJgyKR531VkFudyAYBsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/4AEB9A2E-1427-49CB-9E55-7F0DF1369034_2/IwDvKllZWQ9wRdjLKNQcRdiyVsZxqxwy7yjLPRb9Rq4z/Photo%20from%20Library.jpeg)

### Cleaning TEOS

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/30915BD3-EA55-4237-98A9-4B09152F935E_2/2bnf1nq9opbZyGxFx26dywHtUp21yoFplpAScoiKPD8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/D8CAD025-7D01-48B4-A769-6A2E1CD46036_2/0jyYtyMFzXsIOXSEJIAgVkyUhvocAX2htKDHi4anZUAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/9439040E-3D18-4D3F-8EA1-B3433609A6A1_2/71xECtZg3weyrs6gQQatF8eS3PoSGav1HyZrfMaBtIMz/Photo%20from%20Library.jpeg)

16:36 Plasma flickered. We skip the process.

Venting

## SRN deposition

### Seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/4F83433B-4383-4F97-940E-1136012BDC02_2/jLDgaP4Q8FyciAixnSqPmgYAEpTBdCTomvU17Kyofckz/Photo%20from%20Library.jpeg)

16:41 Seasoning started. SRN8 recipe

16:49 Finished. The color looks good.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/DEFC205B-9C02-48E7-AD6F-621FD28F46AF_2/t5ETzu8V9qOGOtMRpNLK2ySJywxryWcoC7QOE15b7kwz/Photo%20from%20Library.jpeg)

### Main run 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/A87E001F-EE05-4EF0-84DF-3FFB916C66F1_2/e1f3PbIvKQyZXesqapqXIPhXoRxvJYJHhra4ZneVzYEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/7731847E-B5A2-4C0D-A8EA-61D5733FC023_2/5dXlTQZNMcoR0pvCHhyDzqLWv0nkIYTt4M4Wm1Pc6pQz/Photo%20from%20Library.jpeg)

16:55 23 mins SRN

After dep 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/5DB696B4-AEA2-4483-BB01-29C4ADA0BD47_2/eJsC2YfePd7x4gCrCkd32N9EKuG9aa90zK8UFbVfkSUz/Photo%20from%20Library.jpeg)

10 nm thinner than expected.  Lets just do 24 mins next time

Second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/FEE7C71B-7121-43DD-8CC9-C68EBD9ABBF9_2/j11csaIhqWVBhaxAyGPGyCqulvluyyIDzVR4sUfKEg4z/Photo%20from%20Library.jpeg)

I should also note that 18 mins was enough to clean 23.5 mins. So we can probably get away with even less cleaning

Before dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/5418D6DE-0A87-4FA3-8FC3-4E247E9039DD_2/vRxSsdZS8guQuQhq0niKsuvM7vh1wRmVMNvc8PnBxsUz/Photo%20from%20Library.jpeg)

During dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/A2CCCF57-E0ED-483E-A2F4-444A66DA64CA_2/iWAk9iZctdlcSPj5onNUyej1SQFxIGQTdaydkZDw5JIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/23AE9125-474F-47C3-B5D3-31252056DD1A_2/XLOvNJeMHsJiAo69BX3LcdAg7eFmmpV8v7deJK5R6Uwz/Photo%20from%20Library.jpeg)

Ellipsometery of 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/36CF99CF-F985-4671-A1F6-6E604968EA0A_2/YIzcK8bdxVz62tGSDX66w8yeYkw0OcsmxnmF0lMmLXIz/Photo%20from%20Library.jpeg)

17.5 clean worked for 24

Before season 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/F8819774-270D-41F2-A0CD-64F7F503C421_2/QN9uN94ZpmPPO64mh1XuBweNsVxgqhJxlHvjK2X04A4z/Photo%20from%20Library.jpeg)

Before dep 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/7C05CF66-779A-4447-BAF9-891653D3C171_2/OrCgPx8gBP69jSEauxRZHYPgrphBO1cv47NdRGUqnmQz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/AAA26004-8481-4D23-8E25-957435B02AC2_2/NT1kvKyTE2hAfIMH5aZY4noBLfDlnAuwmv7v0o42xesz/Photo%20from%20Library.jpeg)

16.5 worked as clean

Ellipsometery of witness sample

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/8742A844-C18A-4F1A-A39B-A33BC7C37C0E_2/E3qI4j7BRvUFYTALyXqMy1WyPo8kdEKNc6xW1Ay3GCQz/Photo%20from%20Library.jpeg)

Before season 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/F8F1C3D6-5176-4C77-8619-484BE0CF7CF2_2/5xiyy7AsjzvVyXiTz8l6B5cSblfJenR5fO1yosDDx0Mz/Photo%20from%20Library.jpeg)

Before dep 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/CDF190EE-CC64-4960-AEF0-7E746D7D87B0_2/gWXiWmxOxxyux2yViavM6w4mcInyqoG8FOkHYIkDj4Ez/Photo%20from%20Library.jpeg)

During dep 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/2DE8F51C-B91B-4170-A2C3-D5325F4CADE4_2/TeSqZODpkeZuEDewr10UJrNM2DmziXq71kWEtStyA2oz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/6C57964C-CFDF-43C6-B0CD-F36F44E146BC_2/3CH31fng4513douzx2bElW2EhkWxk5DhlMpoM2b9AFIz/Photo%20from%20Library.jpeg)

Next, we need to do the conductive oxide deposition.  In general, a thicker film is better because this gets more field contrast as you switch the photoconductor.  The idea is you really want the photoconductor to not dominate the bright state total impedance.  So we could do thicker.  I say we do another 1.75 um, which means depositing for 24 mins.  Below is the recipe

SiH4: 40 sccms

N2O: 500 sccms

Ar: 475 sccms

B2H6: 133 sccms

Temp: 375 C

Pressure: 1800 mTorr

Power: 10

Keep in mind, we will be depositing using the carrier wafer, so the results will differ a bit.  It will probably be more insulating, so I will cut the N2O flow to 475 or 450.  We can throw a witness sample in to compare the index and dep rate to before.  We then want to use the Lesker to sputter onto all the pieces.  Please avoid any blow-up sights on the straight waveguides.  Fewer waveguides is ok.

I am running 5 min preclean and will spin clean the chips  

Before witness sample season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/A2FDB627-ED79-4580-BFAF-728A5454B71F_2/xGOIpZq60ys9DzoyDscdwpOaKuzW0Gk08mklV8AKB1Ez/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/C1FF20E5-4BAB-4847-8C38-E4D4C06B1BCB_2/McFMNbsbiQiIUPdXtgn4iIpjxJaviQV1sUZnx8GQPWUz/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/F50C51D2-7629-47CD-BADE-D2A741E10703_2/zsXu0q3r5Rv83mIpU2O3BHZk4B08ZK5R8VynSCr4jWIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/2AE37EF2-570B-4BAE-B435-7563B3C3E8D6_2/MFWOXIt2xNRuBinFEPDpXlz2sJoIyBTByjxaJram8pMz/Photo%20from%20Library.jpeg)

Below is what we got before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/61fbc38d-a693-6106-bd64-6f02a0cb674c/gVAjY7RofOOfUQTm4fpVWDythCQniTHKowQ2Vsr5Gzwz/Photo%20from%20Library.jpeg)

Index is quite a bit lower.  Lets flow 425 for 25 mins

Before deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/5F8CEE97-A3B7-4ECA-9BE9-CF1158CACFEE_2/J6KmBzRxfxFEDJravSbFuvpuuLZqAwOYXjS8MAlPP3Uz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/E823573D-E9D6-42DB-A4AA-1F6EB585F3B0_2/BC0GGyxYfy3mYwx9wcrduTZHsEnbgKv0vysgIGXux98z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/C89DB4DD-631D-415C-AAAB-4A0471FAD6D1_2/8zWWV2erYLh0asEwLDNPAxrCEEpVRjUdnzHKAqQNxicz/Photo%20from%20Library.jpeg)

After mourning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/BA4EC010-C932-48C0-86A5-7A3D273EE5E3_2/1YA9yfQJoF5bbQjHdENdPKx6PDSv5lHNhWA5giLLdEIz/Photo%20from%20Library.jpeg)

Before starting sputter

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/CF123645-ADE9-4F84-9EA5-15CA11913B33_2/E26hIhdktKcdReb08TrISxLqKWFu4dLtCK4SmoGFyvQz/Photo%20from%20Library.jpeg)

Ellipsometery of the DON top cladding

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/33539265-CAF4-4527-BA2E-3D42E4455E93_2/YmWYcMwppe45CQmkANAys5xbHGdN0lahh1wKCVyyLgYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/AFFC4BD7-A30E-47E5-8218-153492CE7491_2/qYMS3h447W5jA1OXyHx0Olt7hLct2yk2sJmxJ7N7Mhsz/Photo%20from%20Library.jpeg)

Index is a touch low, but oh well.  So we expect the top layer to take most of the votlage contrast, which is a bit rough.  This probably means we have a lower operation frequency.  

At end of sputter

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/623586A3-4804-4149-AE30-62F1010088D9_2/xNTSkuVT0magznB5M4DP2mLoe70X501biy3CbSpP1Fwz/Photo%20from%20Library.jpeg)

After a little while longer (cool down)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5C28966C-D039-42A7-9F0C-7C87037C0EC5/54D98AF9-E3B9-406B-98DD-718066DD032B_2/m6aQOeJ6Ix5cQmxfSooVdJbUw8iywGST7aOUgv9Eyswz/Photo%20from%20Library.jpeg)

After polishing the four layer snake

