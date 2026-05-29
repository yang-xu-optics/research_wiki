---
type: craft-export
title: "2025-04-25 spdc attempt on low-loss sin waveguides"
craft_document_id: 5D1104D8-6C8C-451E-B605-71D4687AE89A
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-25 spdc attempt on low-loss sin waveguides
[`Fri, Apr 25`](day://2025.04.25) note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/CCF6ED9B-9AB0-4B2B-B3F4-65486F91D1FC_2/vG1qxzcn0fJiO3CyDuuhjBaCyXrLaku34vEliQPyYLwz/Photo%20from%20Library.jpeg)

We test the waveguides fabricated in [2025-04-18 Etching Full Spiral Device with CHF3/O2/N2 recipe](craftdocs://open?blockId=57996FC7-96C4-412F-9D45-00B42342483C&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8).

# E-FISH measurement

## Elmo

We first couple ELMO in

We see 1.85 mW / 8.3 mW = 1.85/8.3=0.223 transmission. Not a bad number for ELMO.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/66C0C0F6-FDB4-4628-B1C1-5626DFF4763A_2/LHYKwVAwvuOCejIBenygvQvKlxd89iyu2ITbP01h3gwz/Photo%20from%20Library.jpeg)

Electric contact established.

We move to SHG characterizations.

Note that we have both ND filter and the dichroic on the way. We apply 3 Vpp,

![2025-04-25-ELMO-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/ABA4BBEF-2E55-4BE0-813E-3DED05D82DDB_2/8ClqAxDx0wllNWkH0tRwtgl8bvAAes7N1CxMn7XljxYz/2025-04-25-ELMO-baseline-peak-normalized.png)

![2025-04-25-ELMO-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/9370A4E1-5D6A-4218-A9D4-86994FF868C6_2/Ayv5UoIXxie2Iw2TzL9DeUpiLrvt7wCQ9gllbDLgALsz/2025-04-25-ELMO-baseline-peak.png)

14.1 um

Realigning the setup. We found the horizontal alignment and focus of the imaging was off. Setting the bias to 0.7 and taking data again.

![2025-04-25-ELMO-baseline-aligned-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/77679252-D1DD-489F-AC18-9719D266C141_2/92CT0nfzUMX3zZ62QaE4QUMqeL0u4NMCQohDbqp23Doz/2025-04-25-ELMO-baseline-aligned-peak.png)

![2025-04-25-ELMO-baseline-aligned-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E9F9BF2F-DF53-4670-9410-4AD7FD04DBCD_2/qCr4PNiRfQkpDaCkbbGEbxE97kv1ZDBpxkERunRiy6oz/2025-04-25-ELMO-baseline-aligned-peak-normalized.png)

Higher order peaks are suppressed

## Santec

### 1570 nm

We have 15 mW coming in

![2025-04-25-santec-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E1518E65-6D79-4F88-BA56-56B8F4DF5439_2/sDF8yRXbWefcJaqAQKxIg54dTAxR4pngXgxWVihNVSUz/2025-04-25-santec-baseline-peak.png)

![2025-04-25-santec-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/0AA024CB-2A63-4A5B-B309-7441AEA15D93_2/ybeqVwIYXvHkVVnaqdlNNlySCPxksZg1isQGXHkX4MEz/2025-04-25-santec-baseline-peak-normalized.png)

Optimizing the signal

![2025-04-25-santec-baseline-realigned-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B2D39328-0090-4D0E-90B6-1B64729C895C_2/fMnGJsXBgWD7AEPgKnmEcginMvWbh9xAx5yKTAOuD1Ez/2025-04-25-santec-baseline-realigned-peak.png)

![2025-04-25-santec-baseline-realigned-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/6EBA652A-5E00-4719-A01B-09CCAF662D2C_2/FHcFwA1ePfrJ6V1uwyyQsYxa67r4ZDP5s677fECgNXEz/2025-04-25-santec-baseline-realigned-peak-normalized.png)

Signal level is much higher. 

#### The side peak indicates that there is an issue with the imaging. We want to fix that in the future!

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/DCF23810-55C1-4F52-98EE-2D3EEF39DBFF_2/JgrbiTqQmPNYsLP84GulY3m0vxNnoYy4LhxGWoGeUd0z/Photo%20from%20Library.jpeg)

### 1616 nm

Changing the wavelength now.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E1C3D15D-DCCF-400C-AC3C-D44BE1522C20_2/hq0zqgK6Q00RyItHQu7FRpxXkFMpi1tqpvxrETgb9K8z/Photo%20from%20Library.jpeg)

![2025-04-25-santec-baseline-realigned-1616-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/EEFA042A-7380-4616-83D8-743B155355AF_2/DCiWng86YojnCRT0dMbSqspss43oz9zm1hvaJexcgUgz/2025-04-25-santec-baseline-realigned-1616-peak.png)

![2025-04-25-santec-baseline-realigned-1616-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/DC72036E-A9DB-4E03-BDF5-3281073F997F_2/noy4tiHIlwLBu34i0KDxKOpgC2jSZ7ewPCGHbJyRPWwz/2025-04-25-santec-baseline-realigned-1616-peak-normalized.png)

Optimizing the signal

![2025-04-25-santec-baseline-realigned-1616-fine-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/66B34369-9039-4413-8B4B-09CCD41B9E19_2/dvf7rK8WtJTJzuvP7lKJB6VcLivaEKXbLvaxsonsLvEz/2025-04-25-santec-baseline-realigned-1616-fine-peak.png)

![2025-04-25-santec-baseline-realigned-1616-fine-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/4FC6A89F-B073-453F-81BC-1DE0735268D7_2/d7jA10t4qZsNODmGjrA70deQNLcOFcxVyC90wTKt7dMz/2025-04-25-santec-baseline-realigned-1616-fine-peak-normalized.png)

Power: 3.7 mW / 14.4 mW = 3.7/14.4=0.257 

Now, with santec installed, I will try to couple the maximum amount of light into the fiber at 1616.  Once this is done, I will optimize coupling for 808.  At that point, we already know the back side is aligned to capture 1616 well.



---

### [`Mon, Apr 28`](day://2025.04.28) note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

# SHG

## ELMO

We couple 2.2 mW / 9.5 mW = 2.2/9.5=0.232 

Bias voltage 0.7

![2025-04-28-elmo-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/3FD9F6A7-B9F8-493B-B654-9F8A84217C02_2/P04Fpep2V2hDG0hmAVYqQyzQfb8e4KxgtV7S1FTngq8z/2025-04-28-elmo-baseline-peak.png)

![2025-04-28-elmo-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2ACFA02A-AC71-4374-A1C9-883C121F74EE_2/ixvwuPptCixHSyy8DWTqgD6TGfEcYTWrwxY6dc6kcuoz/2025-04-28-elmo-baseline-peak-normalized.png)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/DBBA92E0-622A-401E-9065-3AA233AE2A78_2/PASVoIfxoWL1DyIloPNAbYqXnxFLMTGySSRcvcxWBSEz/Photo%20from%20Library.jpeg)

## Santec

We now combine the EDFA to amplify the signal

![2025-04-28-cw-baseline-1570-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/5BFAECAD-11B0-49DB-B370-96F0C536AF6D_2/s09A3hJk4AaFaza6YmgH6MbsBC4GTUNe7c5eMKaB72Uz/2025-04-28-cw-baseline-1570-peak.png)

![2025-04-28-cw-baseline-1570-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/127FE62A-D7AC-4323-B61B-BDFAEB3FACC0_2/NtsLxV84WyQYmqAp9o7IfajnUXo0PxcWd6QEi4aO5Esz/2025-04-28-cw-baseline-1570-peak-normalized.png)

Optimizing the coupling

---

Somehow, things got misaligned. Need to realign the coupling.

## ELMO

We see SHG. 0.7 Vpp bias.

![2025-04-28-elmo-baseline-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/894A23D6-88E2-49EE-9C23-0DF33FB64260_2/NAtqFDPAruZM6jLg15KDbNErb7gcafBRFCQaqH3sVvMz/2025-04-28-elmo-baseline-2-peak.png)

![2025-04-28-elmo-baseline-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/3F28AFD7-7FF0-4D80-94DF-BFBB8D43D6B6_2/Wqz2a4x5yFGDfG8dDWPhk9z15pN58REiu5rIWbndIaAz/2025-04-28-elmo-baseline-2-peak-normalized.png)

We see more power but this is without the asphere.

## Santec

![2025-04-28-edfa-baseline-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2B282F8F-FBB4-4934-B56E-970C36CB85BC_2/FkgdkRofEyCM6rTsnvbSghcesFoX2nyoELJTDB4AWWQz/2025-04-28-edfa-baseline-2-peak.png)

![2025-04-28-edfa-baseline-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/79105524-4B94-43F7-86A5-FC19E28A9F0D_2/rSpcxmiEUEmuaUVtxUTFI5DJyIw7B90y3OpAKY8H7x8z/2025-04-28-edfa-baseline-2-peak-normalized.png)

Using EDFA

We align the imaging setup. It seems quite sensitive, which is a good news. Got some nontrivial improvements.

![2025-04-28-edfa-baseline-3-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/0B2C202D-7B3C-4AEE-8309-8595B8F9E5C6_2/QFSyyW6Pban1FC5MOnp8WbZDxxA1YyDcZVAC1uRxZnsz/2025-04-28-edfa-baseline-3-peak.png)

![2025-04-28-edfa-baseline-3-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/A906A327-6BC2-4463-948C-1E8CD7C64F98_2/VKnPqxHILpH6pK12HybTTJ4svpV6rRxXfVpO9MMx6ywz/2025-04-28-edfa-baseline-3-peak-normalized.png)

It helps to first set the poling period to a longer side and optimize the SHG

![2025-04-28-edfa-baseline-4-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/885BA1FE-5C49-4770-A783-AF836FBC374A_2/ZKy1FxJmyd3w8QEVdb9Z4WVZEm2VdIAVByOvJ2YAWTgz/2025-04-28-edfa-baseline-4-peak.png)

![2025-04-28-edfa-baseline-4-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E45A792F-B9C1-40CE-8BAF-8FB675967740_2/7ox3Wade2RFeEnErL53BrDtXvwaT4PFMOlkMooHxoDkz/2025-04-28-edfa-baseline-4-peak-normalized.png)

Further optimizing.

![2025-04-28-edfa-baseline-5-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/4AF91F20-83AE-4FFD-ABE0-A688F8DC423A_2/Bp91YQ6Xa0Kyz5aTUOL5lz8lvixvLBlGQ0f4yPsGcV4z/2025-04-28-edfa-baseline-5-peak-normalized.png)

![2025-04-28-edfa-baseline-5-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2A8596F5-3871-477B-A8E2-F5C9AA1A2626_2/RAJDVkB7H0xJGCRqxms2t021pWBafKGsf90tPo2q0iwz/2025-04-28-edfa-baseline-5-peak.png)

A very beautiful sinc! Extending the scan window.

![2025-04-28-edfa-baseline-5-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/BFB46FFE-3B6E-40E5-96A0-67C037C3486F_2/4UReayPYogtxv7xFLrKq5Jx2gWiEESt9qWr3Yxc7HcAz/2025-04-28-edfa-baseline-5-peak.png)

![2025-04-28-edfa-baseline-5-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/96653C4A-4EC8-44E6-A5C7-E4D0ADAA7D68_2/By8nbpmUUTUK68h1nq73nyRooQlyx0sxDclrxGK6xxAz/2025-04-28-edfa-baseline-5-peak-normalized.png)

### Vanilla Santec　

We now remove the EDFA. 

![2025-04-28-santec-baseline-1570-1-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/1BC06A62-253F-4EF4-B892-71AE1306C2A5_2/axESNNozafqV78q1WxgTGfq0e3ymyKKHmDrHTxBuWhYz/2025-04-28-santec-baseline-1570-1-peak.png)

![2025-04-28-santec-baseline-1570-1-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/6C8CCC69-5A63-4279-AC52-A0A458547075_2/9zQ97yuUogM8PY0VUeYQoYj5tB6yuWlXpEEF0pyUk68z/2025-04-28-santec-baseline-1570-1-peak-normalized.png)

### 1616 nm

![2025-04-28-santec-baseline-1616-1-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/906CB793-F17A-4F53-9DA3-DA61517DB975_2/c3vTLvBtybDra4HF8e0IdamyKSYpQr0X1FYteVfL1T8z/2025-04-28-santec-baseline-1616-1-peak.png)

![2025-04-28-santec-baseline-1616-1-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/37F01DD0-D842-439F-B0A3-8B0C94F80554_2/0yVaHXLyrc28WZk7s8jLfkntJcOKR4C2FZOksLR98osz/2025-04-28-santec-baseline-1616-1-peak-normalized.png)

Good curve.

Optimizing the coupling.

![2025-04-28-santec-baseline-1616-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/966C49FB-C805-4B8A-98CD-4572EEEED50D_2/UMlLUShiDwJM2B1bM0vt4Xcu2bwVPg49sMxCaU4s7CYz/2025-04-28-santec-baseline-1616-2-peak.png)

![2025-04-28-santec-baseline-1616-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/C1000A46-82BF-4F46-BA77-14551477271F_2/mVTeo4rXIaR1S7sngML7I9ioGjM8w22RpMem7wFlqcQz/2025-04-28-santec-baseline-1616-2-peak-normalized.png)

The power is good. Even better than 1570 nm.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2421F112-A86E-43B8-8BE6-EF5E030B4DD2_2/3MwIVIQtDycZ2A3xbuqFWOPQXCtjzm1ehi4NUWDmUtYz/Photo%20from%20Library.jpeg)

12.3 mW / 2.2 mW = 2.2/12.3=0.179 but the power was measured with the 780 nm gauge 

For fiber coupling, we get 250 uW with single mode (with 800 filter 177 uW). The multi mode has almost no loss (so 2.1 mW). The method we used we collimating each lens to infinity, doing two beam overlap on mirror close to fiber objective and output waveguide objective, coupling into the multi mode fiber, and then slightly perturbing to get into the single mode fiber 

We now couple 800 in, being very very careful not to mess with fiber alignment. We can break 1616 input alignment, as we no longer need it 

Below is power with red light

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/CE3E96B3-415D-4ED1-A3E2-E91601FCAC29_2/PhlsNUlyMSeuh9ZGyzr2KWoP3bXLmkTkJmuBH2sxTEwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/482990EE-811D-4C32-86DD-76AF82545556_2/sM448nmyfdrvHbCVyWNYHUpHxiTJkMwINAtVobFAmmkz/Photo%20from%20Library.jpeg)

We see 19 mW input power from laser

With 450 mA on laser, we get 166 mW 

20 mW after the waveguide with red light on. So no burning, as this is consistent with 10% transmission 

# SPDC attempt

We plug directly into SPAD

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/13CDF4C5-43CF-4628-8CA7-592EC88A14B1_2/2LYy6AALpDyWfPQ9tbgmkwcqIbeKxhgrkx8nkjnI7B4z/Photo%20from%20Library.jpeg)

Use ID Qube as software. Box behind is how you turn SPAD on. We set voltage to 7. SPAD takes a while to turn. 



---

[`Tue, Apr 29`](day://2025.04.29) we will start from recovering the baseline. We first couple the ELMO laser into the chip.

# SHG

## ELMO

Used for alignment. We took away the dichroic, so the signal is brighter.

![2025-04-29-elmo-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/98AE7C7C-CE9D-444F-9496-5744020037B5_2/0hCqyCXGFUup3X3s9UmCx4bohZKOgJPTH6yKrjBcQsQz/2025-04-29-elmo-baseline-peak-normalized.png)

![2025-04-29-elmo-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/65C6182E-1793-4A50-A04C-0556A96C27A6_2/W6TDkvxtNc9mX78DLBJSDBOKOLLbXEJIkmyoJjjcvK8z/2025-04-29-elmo-baseline-peak.png)

0.4 Vpp

## Santec

Moving to Santec with 1616 nm pump. No filter on the way. Previously, we saw 0.017.

![2025-04-29-cw-baseline-1616-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/19063EE3-6FD3-4DFD-97D6-C440BE5CD60F_2/YgqBmrsLsSe1pxxoTyyC8EA0ljDFhRiKLQO6X90rXBgz/2025-04-29-cw-baseline-1616-peak-normalized.png)

![2025-04-29-cw-baseline-1616-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/F88C3E7E-3062-464F-B771-E2637CDA1D8B_2/bC5LyXx9jM3iAYcAvSYh1avNWPFsP0zuyLyi09pWJDMz/2025-04-29-cw-baseline-1616-peak.png)

Signal is a bit lower,

Optimizing the imaging setup a bit. Not a significant improvement, though.

![2025-04-29-cw-baseline-1616-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/AD101729-A3D1-47AE-929A-EED79C4A2999_2/Y7WypziHc9nrMyu2PXNQolYs9D9kaGyWrh4xsLRxL6wz/2025-04-29-cw-baseline-1616-2-peak-normalized.png)

![2025-04-29-cw-baseline-1616-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/D94AE881-B509-44FF-B537-A50C5A89781A_2/AOcNk7KL5BQRyPrw0eWQWQ4LmF9ZsmHZcO3iDNGwJuYz/2025-04-29-cw-baseline-1616-2-peak.png)

Turns out that the vertical alignment is also important.

![2025-04-29-cw-baseline-1616-3-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/9FBEB5E7-C8AB-4ADE-8D9B-2E67D1A015F2_2/Wdu0ZMLydEO07z8EVOXsbVSuP4hDjdpaE1onydDGgFUz/2025-04-29-cw-baseline-1616-3-peak.png)

![2025-04-29-cw-baseline-1616-3-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/578B7216-E707-47D2-A60B-E600D0B43A88_2/XfYS8ld7Mf7ME2NryqgtRbHRI9mNNMoLIEV0W2wE3Hgz/2025-04-29-cw-baseline-1616-3-peak-normalized.png)

Signal level increases. We move on then.

14.4 mW in, 4.3 mW out.

4.3/14.4=0.299 transmission. Pretty good value!

# Spectrometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/502ADE6F-917E-41B9-9266-B5CE368E9F48_2/tS8X54X96P1tBVlNlhw83euvHnciXVTVTIz7Q2sblYgz/Photo%20from%20Library.jpeg)

Aligning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/113030FC-C589-4E48-8988-87EB7F7558EB_2/ZFaU6XHd3SARxssoRII1UU5XxxLj9SxZJ8ituDLpL9Uz/Photo%20from%20Library.jpeg)

We measure the spectrometer output

![2025-04-29-calibration-multimode.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/5D2E59C4-9960-4CB0-B8FC-DBB59754B537_2/xud8lnPRNcTx2Joys9x17AvNdziNBvtG9r0g2oV1Dhwz/2025-04-29-calibration-multimode.png)

Single mode fiber

![2025-04-29-calibration-singlemode.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2C459985-EB46-4DC0-9A33-7A8FDABF0634_2/4yDIFr2F6jd69TpEoW7jRKB6xLirbnIQR5XWFO7bdMoz/2025-04-29-calibration-singlemode.png)

Wide range calibration

![2025-04-29-broader_scan_1550nm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/0F2AC509-488C-41F4-B407-51DA51CA8B1C_2/CCNb4ekNaqyXzRXX9y1Gu93AvOLia2x4OWtBOgR17doz/2025-04-29-broader_scan_1550nm.png)

![2025-04-29-fit.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B2CE8E31-C3F6-46CC-8296-5A15636AFAB9_2/YYEx5QpXoz2fxa9SoGdGcTd0ebabkKCpwRN71vHR0T0z/2025-04-29-fit.png)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/4055F3C7-A7C1-43D9-B42C-4B1C236AABDA_2/31oOKpM0sMZo5SvXD2M7KjlyOIt1Rt9iRzM91etUXkUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E445E17D-6230-4B12-9285-A25D901FE836_2/DgDX2lJ9WTFr8x1S7OV5qYqpgpdUsECExd9DONBfV9Mz/Photo%20from%20Library.jpeg)

After coupling Santec through waveguide, fiber and spectrometer, we get

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B1C278BF-8B00-446B-915A-FF6CD3D36795_2/GvZnoXPyvDDuH4OczFtROQq0yn1mHx5f77rWeteOhBUz/Photo%20from%20Library.jpeg)

We have 4.5 mW out of waveguide and 1.5 mW on spectrometer.

# SPDC

We couple 808 nm light in.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/6B3DF911-1F43-448A-A49C-D241628930DB_2/BkmNP6rY781HCxzxHt2BhB9DchoxxDeTxlURDhkyi9Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/70F4B517-7B91-449E-8CE2-C73E8A813613_2/CI1xu4u0iJQx7G1wWBv3TFcyvWy5LvQmeAWRyPamxg4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/305764E4-3659-46D5-B705-D82BC97EE626_2/HONmCq3bXdWZgAFFFbdcmzksos7Cio19MK4zvJ45K4kz/Photo%20from%20Library.jpeg)

450 mA pump current.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/EF4AEBDC-B85A-4B16-873B-09F9801BA721_2/w5X48nbyXHumZG2H61mGVf4r9RpPmuDbLpOqEtg41Z4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B94889D0-D7E9-4007-AD47-E596BF6DE89A_2/8OVPs0Tx55Amw7KPKD3Zh1DzdzGSNYzUvwYHrLi9luAz/Photo%20from%20Library.jpeg)

Make sure that the Santec is off!

Connecting SPAD to the spectrometer.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B63252DE-8AA0-4F5D-9CB1-FAD1BAB5D203_2/iz5vyYZP9ucv3Y2dWb9xEfoVeNbbsXVRr15rXZa8WJ8z/Photo%20from%20Library.jpeg)

7 Vpp bias.

![2025-04-29-SiN-fluorescence-no-poling.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/D701B479-A482-4273-B3C8-F02F7C916F61_2/q9aswPRg5xIQLci59T77fBv7lnx4Vjz3xcUcvy1FGEcz/2025-04-29-SiN-fluorescence-no-poling.png)

![2025-04-29-SiN-fluorescence-poling.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/001827EE-54F8-452D-9A83-54758A48E42E_2/IlxjLSriBoBiGiJXVCF7QeHDUCxFG9l5wJCcrcyKhEUz/2025-04-29-SiN-fluorescence-poling.png)

We see fluorescence..

## Scan

![2025-04-29-SiN-SPDC-base-period.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2B58A910-005E-4739-A9A9-EDC86F2C16FA_2/h8goWKAxWaQslDFLX2x1cTe8RccvFyFN1E9GyQqCAqoz/2025-04-29-SiN-SPDC-base-period.png)

Switching between two poling periods. We then reduce the pump power a bit.

![2025-04-29-SiN-SPDC-base-period-3.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/6267C3F1-DA71-4FFA-A0ED-CAC10E9993D0_2/33OHAZt5nHxb4adp2ZhkM5UYau4IjrRoGyCxmbsPH9Ez/2025-04-29-SiN-SPDC-base-period-3.png)

![2025-04-29-SiN-SPDC-base-period-down1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B7AFD317-2677-4A64-8AFA-0D478065519C_2/x3AdZMeiNxZnXjgxkukQB6zZ1B2dyAegOwPipzDnUCoz/2025-04-29-SiN-SPDC-base-period-down1.png)

![2025-04-29-SiN-SPDC-base-period-right1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/F67620C9-4358-437E-A3D4-1BBB44D9A890_2/maduJsCoI8xxgJ3MLcfydg9wOSF4amgG2f5xf5xOw3oz/2025-04-29-SiN-SPDC-base-period-right1.png)

---

# [`Wed, Apr 30`](day://2025.04.30) Stimulated emission tomography 

# SHG 

## ELMO

![2025-04-30-elmo-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/F736F0A9-AF0E-4DF1-8915-CC83D33CD17C_2/7xMz3mAYKMMgcQxnfXEEkXN1PYuaNxdlBq6pT0EYbxUz/2025-04-30-elmo-baseline-peak.png)

![2025-04-30-elmo-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/DDCFF34E-028A-4C80-B37A-97927C80E54A_2/W79jZwfCrryT9AMbTQo1Bgkq5vizucN9xNYUfyySjpQz/2025-04-30-elmo-baseline-peak-normalized.png)

We optimized the alignment of PMT

## Santec 1616

![2025-04-30-cw-baseline-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/C3AFBDF5-E4AD-4A40-925E-B70CB256BCB9_2/3dMtNchK3jfZNHmU7JbFpbzpi1clugWSbiKplFoynRUz/2025-04-30-cw-baseline-peak.png)

![2025-04-30-cw-baseline-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/BF6D4D48-2DBF-4CE0-93CA-C4B261877232_2/GanGTMxu5DgnNCEtvi1II4JsN35KiOcq2acx09nItykz/2025-04-30-cw-baseline-peak-normalized.png)

Optimizing the imaging 

![2025-04-30-cw-baseline-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2BA0D5E9-1D4A-40FB-B521-ED4BCBE122D1_2/IczNorqweGMlUboJh391fh4O0bh25ifu8kxedxxKGjIz/2025-04-30-cw-baseline-2-peak.png)

![2025-04-30-cw-baseline-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/C1142C36-3551-49E9-B2D0-F1A9B1D70027_2/gOubJAySlj7nhSqv4x23RFlSngQSTsMsaiy7hfawNtYz/2025-04-30-cw-baseline-2-peak-normalized.png)

12 mW in, 3.3 mW out. Coupling the light to the fiber. 1 mW fiber coupling seen.

![2025-04-30-broader_scan.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/FA2B60D0-C747-47DE-AC9A-13F3BE08DA6F_2/8M7e4sAJ3w9xHCySjxzDk9YayxaPjxp1uo4QS4jWna0z/2025-04-30-broader_scan.png)

![2025-04-30-fit.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/70CA9D5B-8AD6-4CC7-8975-B3E00E178D0F_2/vwNXQabb0u7mE4tgDbzo6zJvAApKSM6mOUBvVoOa0IAz/2025-04-30-fit.png)

Calibrating the spectrometer

Pump light wavelength: 804 nm

1/(1/804-1/1630)=1,586.586 

---

# Continuing on [`Thu, May 1`](day://2025.05.01)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/4EFB778C-D1BF-4960-A3AF-82D0B0A470B8_2/fkyBA2yyAwTwc3v3FDxHedQonqZ65NkktkeMBsmrkjQz/Photo%20from%20Library.jpeg)

1586 nm we see 1.1 mW after the spectrometer 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/B1F85AF0-FE38-4850-8C3F-68478D683C01_2/fqUfaxEhqeeprKqnOr24OyiC6b5blOSRfCpGtTR6EZ0z/Photo%20from%20Library.jpeg)

k= 0.0216

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/AB44C168-0C16-48E2-91B6-644E87142687_2/LNkn6w0yydxsKD5QYxH4D5OE7X6cNTfpGorNzBplIGEz/Photo%20from%20Library.jpeg)

![Drawing](https://resv2.craft.do/user/preview/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/7122B404-89AB-4418-998E-8A7CABDD5676_1/CVcEytZ8KwDhUUHyqpoIRYVpgsyqCxwxrlszM0vYIpAz/Drawing.jpg)

We use A220TM-B for the 804 nm

![2025-05-01-calibration-singlemode.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/5616D12D-26BF-4E39-899B-F87F4435B0DB_2/rgYOxA6niycIy9dWbbX0UI9gtLFUh812XbNhy39sqTgz/2025-05-01-calibration-singlemode.png)

![2025-05-01-fit.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/61DD0E4A-05D9-434A-BA4F-84F34FB0287C_2/fyQofVu5uLKz6ErBejxPr02mUouu2n6N97wQXzAbSTMz/2025-05-01-fit.png)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/277E7FF0-86B4-47D1-BF91-FA50676A89C2_2/IIjKIyl6P7IofH6ODAblNZayIFDYaDxJMvBtEU7uvuQz/Photo%20from%20Library.jpeg)

We have 6.3 mW coupling through the waveguide.

## Fluorescence characterizations

SPAD connected.

![2025-05-30-SiN-fluorescence-283mA.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/87B2560D-1D43-4D24-A08D-423EB40E37B5_2/CsHqgsgTvwqODcN2ZKGxnLJcHThIMYxkdqPx8od9QUIz/2025-05-30-SiN-fluorescence-283mA.png)

Fluorescence level 

Reducing the pump current to 200 mA

![2025-05-30-SiN-fluorescence-198mA.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/266D232C-72F3-470E-82BA-459DC9702D2F_2/8ZwBlCsu3Q4oMVzujHARUzhtVxd65oooPRoXaJCCmn4z/2025-05-30-SiN-fluorescence-198mA.png)

Less photon counts now. We keep the pump power here.



Baseline: We send in -10 dBm Santec power at 1630 nm. Pump power is about 200 mW. Poling period 14.18n um. We don't see difference in the signal level.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/811B1865-AAF7-43A2-B4BC-4027B4C3B4A4_2/A3uJCCZwfgS11TtMjs1kyffQ5Z0cyRIwe2f1GhhRzIgz/Image.png)



Taking SET data

![2025-05-30-SiN-SET-Pseed=-10dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/EE71DB97-83DD-4648-82CC-8CC4BD330832_2/4A9dUX4wwvJ9WlvnOZOdGcw6xO2CwnvUQY71zTJyLk8z/2025-05-30-SiN-SET-Pseed-10dBm.png)

With -10 dBm, we don’t see anything. The average photon count is around 8 k/s.

![2025-05-30-SiN-SET-Pseed=0dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/79517C24-4FC7-481D-9677-78CEA219293F_2/hOURLIOpvRS6q0FdnXGjoLMaR2QaYMRinGA0EIz5i6Uz/2025-05-30-SiN-SET-Pseed0dBm.png)

We don’t see it at 0 dBm.

![2025-05-30-SiN-SET-Pseed=10dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/552EBA7A-B6B4-4C4D-9013-66BF0FBCA948_2/JyxTnl3Qdj8y6eMZ5SM0NqG0Wyw7CsEQnMVjSjEL8M8z/2025-05-30-SiN-SET-Pseed10dBm.png)

We realize that the alignment was off between the waveguide to the fiber. Realigning.

![2025-05-30-SiN-fluorescence-198mA-after-alignment.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/6CB28FB9-0941-417A-B095-A01A1CED7BEC_2/vR4EbfpZUxcnLT5kIIEbIzy73vXm7xLFkYGiiYmHjWgz/2025-05-30-SiN-fluorescence-198mA-after-alignment.png)

The fluorescence level decreased. We optimize the coupling at 1586 nm.

![2025-05-30-SiN-SET-3-Pseed=0dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/05E05FAE-3B07-4F08-AA22-AB72EC9A1204_2/qvbvArTiTJzdgoZbniYYXevsocgQeD2fwEM7CyMa9bgz/2025-05-30-SiN-SET-3-Pseed0dBm.png)

![2025-05-30-SiN-SET-3-Pseed=10dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/ED20444F-2AEB-41BE-BC6D-576B08DCBC84_2/hEVLImiwiFn9crfgHxKWZV9ebhoMFd6488HGiJsqe1kz/2025-05-30-SiN-SET-3-Pseed10dBm.png)

Repeating to see if the features are real.

## Realigning

![2025-05-01-cw-baseline-1586-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/2F3B536C-327F-4020-A1E9-ADFD75531361_2/3cTzevBDKlvfbzwyQxciri866vTSMblKLabGWTygdmEz/2025-05-01-cw-baseline-1586-peak.png)

![2025-05-01-cw-baseline-1586-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/077B8E5E-58A0-4E24-9109-692FF1BD760F_2/2xbKszYOAAY9CseqC45QFEqrRFI51O8q0Iao3JIyzZ0z/2025-05-01-cw-baseline-1586-peak-normalized.png)

1586 nm SHG. It felt like we were coupling into the photo conductor mode. Now it is well aligned.

![2025-05-01-cw-baseline-2-1586-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/111E0F96-B8D6-4979-9763-FB3ED88E6554_2/xutX5eMjn5iaBULoQWKzbZKND4UsyTBVdyVYlUeqh5Qz/2025-05-01-cw-baseline-2-1586-peak-normalized.png)

![2025-05-01-cw-baseline-2-1586-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E3EBC11A-7F9F-4BC5-A07F-B85C64280E58_2/ZFdOS1wf6P1lvXIiHLGNuwUJoBdbVdf2RzcTMyOu8iMz/2025-05-01-cw-baseline-2-1586-peak.png)

More signal now.

We have 1.4 mW after the waveguide.

We make sure that the coupling is into the right mode. Using SHG. The SHG power is good.

![2025-05-01-cw-baseline-3-1586-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/8B654E95-13C8-4C6E-B630-C58D7F3BBFAE_2/goITM4He1gpx9OXtCTfTgrbmHRXnktPzg2ECUQiJVVAz/2025-05-01-cw-baseline-3-1586-peak.png)

![2025-05-01-cw-baseline-3-1586-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/69A5A6D0-B9DD-4A24-B235-1FC41791F88B_2/zlqyhkbkTGVhCjfvVaEeaj6nLR7rd88BbYHDTYqfjYwz/2025-05-01-cw-baseline-3-1586-peak-normalized.png)

We see 1.85 MW after the fiber. 4 mW after the waveguide. 13.5 mW before the chip.

Coupling 804 nm now.

2.7 mW / 40 mW coupling to the waveguide. 

We now move to fluorescence characterization.

![2025-05-03-SiN-fluorescence-206mA.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/7444EA60-34D9-466F-A509-7B20877AAA0F_2/GN4YRrpyhmUECTdTNUJIYZksNDy3pMTxwmvBmcIsnicz/2025-05-03-SiN-fluorescence-206mA.png)

Poling period has to be somewhere between 14.095 and 14.18. We should scan 0.15 around 14.18 um.

We find that Santec causes scattering and saturates the detector. Instead, we increase the pump power.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/24BD2929-E412-451E-A8DB-4CC6D147B463_2/uxxyvCPlYFbuyEmFInQXVF4ytWh5vsyxRH0J60WM2hoz/Photo%20from%20Library.jpeg)

Attenuator.

![2025-05-03-SiN-fluorescence-450m-Aattenuated.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/BDD3CB58-D4A9-439B-AEE8-3CE82B895106_2/p9XiSKBxNLqkZUeUkxydWk1PlLKJREA8nQQyNyUSMxMz/2025-05-03-SiN-fluorescence-450m-Aattenuated.png)

We reduce the fluorescence counts.

![2025-05-03-SiN-SET-Pseed=-10dBm-0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/04041D9B-392F-447B-9AB1-4DE1D1924AC9_2/U0UsmfgVIOgr5jGaFqcXd6nyMx0GVxyWY1DzofMKdlsz/2025-05-03-SiN-SET-Pseed-10dBm-0.png)

SET attempt. The signal level is not high enough. Moving to -5 dBm.



---

# SPDC attempt with 785 nm light

[`Fri, May 2`](day://2025.05.02) we installed the 785 nm light source. We would like to get the signal at 1540.

## Baseline

We use 1540 nm for the SHG. 

![2025-05-02-cw-baseline-1-1540-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/20F5C379-7D18-4499-80D9-3EFA182202A5_2/9DGxkIwf8z0YKzDixI22bnpcgFQHudDTSSOGK6sGjTkz/2025-05-02-cw-baseline-1-1540-peak.png)

![2025-05-02-cw-baseline-1-1540-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/3480839E-BF3F-4B9D-8598-A6448333BA47_2/EeuOLzhf58QVOTet9ETHGz4as5ypVyV6jAWTWeJZY8Ez/2025-05-02-cw-baseline-1-1540-peak-normalized.png)

Optimizing the signal.

![2025-05-02-cw-baseline-2-1540-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E56B3527-3BDB-4C48-86C0-12BB45DE18A9_2/jdxmbqyrZZXdzpgUxKkZQscFPxQDeja25y56HGexWHQz/2025-05-02-cw-baseline-2-1540-peak-normalized.png)

![2025-05-02-cw-baseline-2-1540-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/A31E0D72-E385-45FF-B4C1-44034B3DBCF6_2/pq4JsCmiXNV3HcBGoA9DtE4oSuC2Bi0MSPNH0MMOD5Uz/2025-05-02-cw-baseline-2-1540-peak.png)

1/(1/788-1/1540)=1,613.723 

1.1 mW coupling to the fiber. 2.3 mW after the waveguide. 1.1/2.3=0.478 coupling!



Wavelength of the pump is 788.

## Seed

Seed wavelength is 1613.7. 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/7BFAE0FF-4450-4349-A2E8-64A7B99C202A_2/GDBxHUuIEC0tA6rZ5kWF8cPTKMAUtS9YGuV9w37m7bQz/Photo%20from%20Library.jpeg)

![2025-05-02-cw-baseline-1-1614-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/F035C1A9-C3F2-4F4B-B3DF-6E1D8E532927_2/4n1fx2Kdnr6GGQe4K7LExYAEVPSUHa4u4TyOpdGceHkz/2025-05-02-cw-baseline-1-1614-peak.png)

![2025-05-02-cw-baseline-1-1614-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/38CEF4E8-D808-47D8-8EC8-D9ABB48A1F42_2/Xjm2uqvP4YGgrSUleD6Fq5zlxrqRPvyoKRTPUeqqn14z/2025-05-02-cw-baseline-1-1614-peak-normalized.png)

Aligned

![2025-05-02-cw-baseline-2-1614-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/657CE261-5A93-4091-93C2-9DC5E46BF3FE_2/xh1gh0r0xPEmdeIBNTclI6XmECSutvbg34sFdv0OEicz/2025-05-02-cw-baseline-2-1614-peak.png)

![2025-05-02-cw-baseline-2-1614-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/1959ED91-DEE5-4C0B-9594-807E43EE1F11_2/iLgICi8SEqyNM17gcmLeknNOzyF70fP2M3BeOyahFpgz/2025-05-02-cw-baseline-2-1614-peak-normalized.png)

## Alignment of the band pass filter

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/EF3C70CC-DAC4-43B2-B3E4-739CC3465A7C_2/ny3LCefLkCPwmuGiXDV8pUh5LNqYq6TF59oM459gjc4z/Photo%20from%20Library.jpeg)

We maximize the transmission at 1540 nm. Maximizing the coupling to the fiber.

## Pump coupling

We see 4 mW out for 55 mW in.

# SET

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/1C55F99E-956A-490F-A6FA-D4E20EB07682_2/DadWAilu38VIRxqWwkXwJCaTBf0WBHsIFIJyaqsisR4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/F989C52A-5DE9-4870-8135-B5BBC0F04953_2/tl0rx29P14zzwqqyhNT6UZI95x01Vhz99RnlbZUANB0z/Photo%20from%20Library.jpeg)

![2025-05-02-SiN-SET-Pseed=-10dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/4D21BFE4-766E-4FDC-BA87-5414D53FF447_2/FLgAyHUxORrCIUZyAxa6AMeAo7pKtQaE1ZxtIXCRrBMz/2025-05-02-SiN-SET-Pseed-10dBm.png)

![2025-05-02-SiN-SET-Pseed=-5dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/57FE7BF5-4E63-4BA9-BA28-23705FAEC67D_2/vZWSIvE72XsMpcfNs52ZQITLoKlXHweuTFUPGgOaFIEz/2025-05-02-SiN-SET-Pseed-5dBm.png)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/83D7B99F-21DF-42B2-BFE2-8C11B13CC3E7_2/ZoEVzVHfWevbVZywaqSMLleRUBoOyd92KhMxyd026nYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/C4E13D7F-E913-49FE-8CAA-657DBAADF0BE_2/LS0CjC9veiiCmlsgIfkmXzhboz8CWBBrrN6l3j2usacz/Photo%20from%20Library.jpeg)

![2025-05-02-SiN-SET-Pseed=0dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/7A194701-7C2F-4B5B-8741-FF4E2A0DA3AA_2/RSXmOzOXpdcWiWx1pg1HOTmhZpBvkzNS4VRixaXlHwMz/2025-05-02-SiN-SET-Pseed0dBm.png)

![2025-05-02-SiN-SET-Pseed=5dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/0B6AA20A-ECA7-4F2D-AA40-3B7DA0DF6CC7_2/WnXxcTh5LEqWa9Q08I6itHTs6YoJxucXfj4xTzQ2geMz/2025-05-02-SiN-SET-Pseed5dBm.png)

![2025-05-02-SiN-SET-Pseed=5dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/93CB53BD-D3C3-4DA2-8865-EB90FE528709_2/Q5CeV3ucy6RlqAvKxVLqTgpzpBbeRrz33mgUeoEJ7yIz/2025-05-02-SiN-SET-Pseed5dBm.png)

We see the signal!

![2025-05-02-SiN-SET-Pseed=5dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/0CC94E04-327D-4938-95A2-A50EDE66AD47_2/xzyEAv49Q9YDhz5CHrPB6xK2xGoEDDFyzUL9olu23S0z/2025-05-02-SiN-SET-Pseed5dBm.png)

Peak seen

![2025-05-02-SiN-SET-Pseed=8dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/E984D579-2FEE-44B0-B729-2DD9350F088E_2/Fmz31sgXXyF1Erhe4KfvW27yqxocoxxwGx85Sh5C9uoz/2025-05-02-SiN-SET-Pseed8dBm.png)

To reduce the saturation, we add a 10x filters.

![2025-05-02-SiN-SET-Pseed=8dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/CE50BB67-1D6F-42F3-AF6E-3502CAA8E880_2/xI2gRnX0ecW013QShji5I0e7qAmfTXIxNhYa4FNxxe4z/2025-05-02-SiN-SET-Pseed8dBm.png)

We see better SNR.

![2025-05-02-SiN-SET-Pseed=10dBm.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5D1104D8-6C8C-451E-B605-71D4687AE89A/D62CAC6B-6AAF-42AE-97FC-A18D2B7EF426_2/mMxNCZsjr2Wglt9mEeaXxWndK6WLyyvJgWVOflKLDIUz/2025-05-02-SiN-SET-Pseed10dBm.png)