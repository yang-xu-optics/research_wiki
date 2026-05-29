---
type: craft-export
title: "2024-3-10 cladding conductivity scan"
craft_document_id: 94264F85-F48F-4359-ACAF-D77A7F11A9FC
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-3-10 cladding conductivity scan
The purpose of this document is to examine if there are any cladding conductivities for which we see the field contrast in the core have lower contrast.  Given our earlier results from our simulations for Ryo, I am going to do these simulations with an unetched device with a period of 6um.  I am going to use the following constant values for everything:

Core: cond = 1e-10, eps = 27

SRN_Dark: cond = 1e-11, eps = 8

SRN_Bright: cond = 1e-8, eps = 8

For cladding, we are going to use eps = 4.  I am going to use cond = 1e-11, 1e-10, 1e-9, 1e-8, 1e-7, 1e-6, 1e-5.  This should be a representitive sample.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/0763E4FF-BA50-4E5F-8390-EFF024D090D6_2/JycMe5EAIxXRygxOWYMmudwGFjkLawcesla2zYaD86Iz/Image.png)

For reference above is the device (bright in the middle)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/C7442C7B-CCB5-47F4-8448-B54A1356228D_2/oVO0XZFsTitxw6xrxYJQrxaxcuEbHu7MS4oHRhR5vbsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/CED79A46-9955-4C28-8040-3011AB394570_2/3iZ7YGftSg7s8we2uZA1QMq6yQyGWTPtNmhjJiLMLywz/Image.png)

I am getting some weird asymettry and discretization.  I maybe could refine my sovler a bit.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/9C2A45B9-8F2C-4E66-BF84-A0306F0B1978_2/zfelxwQBgSLWQDIFta9NwhFiOgBcEVXZC2QDBg7yIxAz/Image.png)

Above is what happens after I refine the pass structure a bit, and it looks pretty nice.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/F6E7CCDB-EA44-46D5-9AF4-C607760C616C_2/WC05VLmfQTQwLYwJZnxoduFMfifGyTxzI2VQIxHX1hEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/9739B2D4-937C-4ECB-B54D-760B9627DF75_2/V6Qd28xVLcYBWRAYs6DQRRyOulKxWQ5y0y35mRpnRiMz/Image.png)

It is still annoying that there are some weird effects in the bottom, but there is also just a lot less contrast there for the simulation to work with.  The top looks nice, and we can analyze that.  I say this is good for 1e-11 and we will keep moving along.  The way we did this is increasing the number of convergence passes.

After going into the lab in-person after resetting the computer, I ran the simulations.  Below is what I see.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/CEB932B5-6059-4933-BF28-FAB7B8E7BE1D_2/yEF8Dxzr9TzybRYyRNACh8kUPw1quyCElcPLOFrp3Vkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/A1917C99-3234-4636-893A-23B955ECC47D_2/ek6yN3sfltut9tL1yACwydXgCClndEMbtIkf9VPcZqQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/57F8A024-17AD-4788-9BFC-69E32AC20A90_2/BbVNa1XZMcVczgFfssQaq7BqCxxg55fOIl6OcYa3wQoz/Image.png)

The basic take away is, indeed, we really do want the conductivity of the claddings to nearly match that of the core.  So this makes knowing the core’s conductivity a bit of an imperative.  For chi3 (so E**2) materials there is a bit more flexibility, but not a ton more.  We may also have some increased flexibility with the bottom cladding (as the fields are already flat there) but that does not fundamentally alter the picture of the top cladding.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/94264F85-F48F-4359-ACAF-D77A7F11A9FC/520553CE-08A7-44BF-9E7D-29C230C44CEB_2/1xeAr5lx5AwFm9adcLxlyWn0cTe3caySeWNwooheSg8z/Image.png)

When I plot in log scale, I see that I have a buit more flexibility (with 1e-11 and 1e-8 being possible).  We just don’t want too far away.