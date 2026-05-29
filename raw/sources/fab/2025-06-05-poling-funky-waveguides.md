---
type: craft-export
title: "2025-06-05 poling funky waveguides"
craft_document_id: ECAB3CA7-2287-4192-8EFB-A10B8E774F44
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2025-06-05 poling funky waveguides
[`Thu, Jun 5`](day://2025.06.05)

# Background

We fabricated programmable waveguides with various sidewall structures. See [2025-05-23 ASML fabrication pass 2](craftdocs://open?blockId=EDF9A93B-EEAF-4542-9EB6-A51B5A4C40BB&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8). We have tested spiral geometries from the same run in [2025-05-15 Square spiral waveguide characterizations](craftdocs://open?blockId=EC932AAF-E076-4FCE-B026-A7604C272D83&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8) [2025-05-31 Testing long spiral waveguides](craftdocs://open?blockId=1B977761-6950-430A-AD3A-BC4428FDAEEF&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8). Now we test the funky waveguides.

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-001.jpg)

[ASML1 Pass 3 (positive).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/C8C8EB91-EA47-4A72-8A28-D077722A8321_2/5qBlAkFlmxv8VyE9DEJRmx4lrAboJFiYcm5L2ogsbU4z/ASML1%20Pass%203%20positive.gds)

First straight

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-002.jpg)

Long adibatic, then long hump

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-003.jpg)

Lots of periods of adiabatic waveguides

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-004.jpg)

Lots of humps

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-005.jpg)



Around the bottom section, we have straight waveguides.

![Image.png](../../assets/fab/2025-06-05-poling-funky-waveguides-006.jpg)

We will start from these guys. 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/7C6F3DB1-A47F-4131-B3E6-40A6F855765C_2/WeMjTN7yed1zJ1WxuaD3WbHPFUEyyWPtW9GGGxau4y8z/Image.png)

Bottom two are adiabatic linear chirp. The top two are sinusoidal modulation. Both of them have a long period of modulation.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/FECAC32F-C1A0-482E-ACDE-DB2DF81DD82E_2/PMTKYjvZCzbf3iVZXEOxkbUl8O45NiWLiIJFySgxc64z/Image.png)

N is the narrowest region. W is the widest region. P is the period. 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/75E861C3-2D9F-4F77-81C2-9AE085938276_2/Zdm0s5yx9ZGeGDmbfAemCq8j1JHO7VSTbAlI9Ssbc4Az/Image.png)

The last section is composed of sinusoidal ones.

# Plan

We should start poling from the straight waveguides. Because the average width of the waveguide in the hump region is (5 + 10)/2 = 7.5, it makes sense to test the 7 um wide straight waveguide to get a sense for the nominal poling period. 

We will then move to the slow adiabatic chirp waveguide. Let's work on the linear one first. The aim is to (1) maximize the SHG for a CW input, and (2) show that we can tailor the QPM grating to get a nice transfer function. We should always take a data alongside a naive poling.

# Preparation

We engrave an ID of the chip. 2025-05-23 #1 straight 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/DBC04884-35C5-477D-AC9D-024E746C55FB_2/13xEFkFLFmpH6ySA7zwyGMq3yiJJqygj78li7Vnyt9Uz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/B6AFEABD-A899-4B45-B1D6-E6226C806BBD_2/Dy6fhDRTq9bfyohEBXnsQGx4GFAT7KhyuTlhARx9Og8z/Photo%20from%20Library.jpeg)

We also need to put back an anamorphic prism

After coupling into straight 7 with edfa and asphere, we get 6.5 mW



# Alignment

We use ELMO for alignment

![2025-06-05-ASML-800C-straight-chip1-elmo-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/1A7CEF35-5D95-4546-8D8F-B4A0D82DA3A0_2/1HCsnDV6T5na0y8uI1OvtcQDP7HHo0oe6AIaHJYV0ecz/2025-06-05-ASML-800C-straight-chip1-elmo-2-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-elmo-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/4A509AF8-D6C3-4224-A962-7C291B6C5746_2/UyIuJa2UUBhF3vy7TxeoWyPeDfOgxcndKeo7oDb9EyUz/2025-06-05-ASML-800C-straight-chip1-elmo-2-peak.png)

# CW SGH on the straight 7 um waveguide

## Baseline with EDFA at 1570 nm

Using EDFA, we take a baseline.

![2025-06-05-ASML-800C-straight-chip1-edfa-1-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/E7E9A7FE-48B5-40DE-B16A-B1F4A5E9C330_2/MGDy9BYoznPyNz3qXK5sGbA0GCKEySg1xvj5l9b5LeQz/2025-06-05-ASML-800C-straight-chip1-edfa-1-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-1-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/00DDF964-558E-41EA-8EAB-82E2F52BE7CF_2/1xvRxsqgKjxZ0DGrUWwwDhSgMosE7yVZtxaLaPcPXmYz/2025-06-05-ASML-800C-straight-chip1-edfa-1-peak.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/F11995AF-E82D-4A4E-B4C3-FDD05C44DB97_2/3T1uKej8l9UqOvlJk8cX1UCQ0Tn5DXyWSkqh47FqGJ0z/2025-06-05-ASML-800C-straight-chip1-edfa-2-peak.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/4BB5E3EA-36BB-493D-8658-CF3ADCD83629_2/cSa5GaoVeQ4Yp4I2QGWfSKKaBbNIJ8aGxN5UtqFlxLoz/2025-06-05-ASML-800C-straight-chip1-edfa-2-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-3-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/653A09D7-115E-42FA-8672-E2F01AF532A4_2/Pf2ss1HzzD93VC4mTNtHjAuxkyVpExJgi14cQsgreo8z/2025-06-05-ASML-800C-straight-chip1-edfa-3-peak.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-3-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/5C84A695-AC6D-4F08-B445-5E477DC6DF00_2/S9quexnm7qd9TL9Y8xG2tQcEYVDTxH7wOLC5nKgpG1Uz/2025-06-05-ASML-800C-straight-chip1-edfa-3-peak-normalized.png)

Taking a fine scan

![2025-06-05-ASML-800C-straight-chip1-edfa-fine-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/9F4E0618-4009-486A-AF13-45CC48FE53D4_2/jtrtaij2W6kBxXa0NPemyJhiU275ToFkuXOf0O2ryKYz/2025-06-05-ASML-800C-straight-chip1-edfa-fine-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fine-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/65507648-2352-436C-94F1-3AC5B3D8A780_2/ZZaokVAS6aNyIVnCvc4WAkv851NiQqBSa8Bjvx2Tin4z/2025-06-05-ASML-800C-straight-chip1-edfa-fine-peak.png)

We realize that the signal level is better when we use 10 Hz bias, instead of 5 Hz. We switch the frequency for the plots below.

We align the imaging setup further. Also, there is a chance that the + electrode was casting shadow. Fixed the issue and moving on.

![2025-06-05-ASML-800C-straight-chip1-edfa-fine-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/19E5D3B9-9141-4752-9EB2-949191A0956D_2/O1CA8ZIaUnzKQDYjGDvlNajp36fjEyy2WX7NRutQjeUz/2025-06-05-ASML-800C-straight-chip1-edfa-fine-2-peak.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fine-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/64B39CF2-92AD-460F-89EF-DB3029E1C4AE_2/AxfWSBiyAM5xQwP3xQKWiwwlaBy1ZBRyT5YdjD7gjwMz/2025-06-05-ASML-800C-straight-chip1-edfa-fine-2-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/C52800D1-BA8E-41E4-848E-B9CFAA0C7D47_2/VfWvUHKFAJ2gML2nSxtiyat1gtWXeNHIDWptIQSWNDgz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/4B017CED-1D35-4974-8DBC-1698112564B0_2/1MKnCJQ5OCA4Gfdlx7g4xmquAmU5TXfWJiyn8TrX78Mz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-peak.png)

As we see a side-robe on the longer side, we set the poling period to the short side and maximize the signal.

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-2-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/374EE5C9-42D6-4B2C-882D-D8AA2C2539E6_2/Z8RxZxXO3scgQxiotyrh0Co4lfZQbausaanEMAwePTcz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-2-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-2-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/0561FFBF-479D-4632-BF01-8320B82C288F_2/xxsp344yfqxHprPW3PwnFpy8R082yK7uxpneR6k31mIz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-2-peak.png)

Didn't quite work out. We part on the longer side now.

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-4-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/10D0A15E-F3AB-4F90-BBEC-67844D3E4CF2_2/Z9Emy6xfRxQCdah3QL4vHZBoWiVGlxyEXARHEvO93Sgz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-4-peak.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-fast-4-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/CA386C88-73AF-4005-8851-B942D1323947_2/7Xm3xNJDJ1Bag2QQsgUOILDbxq5NWY5j3JtR0xT3xYwz/2025-06-05-ASML-800C-straight-chip1-edfa-fast-4-peak-normalized.png)

Doing the same again.

![2025-06-05-ASML-800C-straight-chip1-edfa-final-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/7FAB1940-A404-4E50-B904-A18BC20A5331_2/aC0aGCR56w3ryJKmBrQbYgPepsUipGku9x2x4vHL7Ykz/2025-06-05-ASML-800C-straight-chip1-edfa-final-peak-normalized.png)

![2025-06-05-ASML-800C-straight-chip1-edfa-final-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/AFDD19F6-CCAF-47C0-B06E-3BF871C3EF33_2/Dnp3qrNnlAPjhDG8tscmWOBYA8aV3AnM54aeW6pCrxYz/2025-06-05-ASML-800C-straight-chip1-edfa-final-peak.png)

This is roughly what we converge to.

## Santec 1570 nm

We take away the EDFA.

![2025-06-05-ASML-800C-straight-chip1-santec-1570-peak.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/14C0F063-510F-4629-9F8E-433DF91DEA4C_2/Z10XdkidBfAPfNvzAkMdVhVjLmpyyjVEye4APHc0AAkz/2025-06-05-ASML-800C-straight-chip1-santec-1570-peak.png)

![2025-06-05-ASML-800C-straight-chip1-santec-1570-peak-normalized.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/7DC0B133-0CBA-459A-BFC5-9DA554F09F22_2/jpLHusH4nsQXqUtx8O0wgWyCekn7uoihFAlyMLORDHgz/2025-06-05-ASML-800C-straight-chip1-santec-1570-peak-normalized.png)

Signal from Santec is well visible but a bit weak. Were using 6 Vpp and 10 Hz.

## Power measurment through the straight waveguide

We measure the power of light in and out,

![2025-06-05-input-power-measured_power.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/50CCB2ED-612F-4606-A150-CDB672551F47_2/AEZXAD3Zo7MdFdVwYPHF85Cwaf7nBNFS9ZwBy1LMGZEz/2025-06-05-input-power-measured_power.png)

And power out

![2025-06-05-output-power-measured_power.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/B9B6B8B7-962E-43AE-837E-D477BE824456_2/JS7jhv1yv34wIls1G5V7qzgLRPB11NFgKg4PhGbc3V0z/2025-06-05-output-power-measured_power.png)

## Wavelength scan

![2025-06-06-ASML-800C-straight-chip1-santec-scan-fineslope.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/BD13B18B-1CFB-4106-B5C9-673A210C9270_2/higDzpeNYpPnZuGE10mZApoDjNOukHKekpDzCPRRcOAz/2025-06-06-ASML-800C-straight-chip1-santec-scan-fineslope.png)

![2025-06-06-ASML-800C-straight-chip1-santec-scan-fineSHG-peaks.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/BBA3C6FE-331C-432F-AFBB-5041AA3D27D6_2/GLy8elRSY0s89xBuxgEzgUNElb8PdzuWaUWyNdKS9gUz/2025-06-06-ASML-800C-straight-chip1-santec-scan-fineSHG-peaks.png)

![2025-06-06-ASML-800C-straight-chip1-santec-scan-fine_fit.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/87A9A388-718B-4E4D-863B-EA5A7806692E_2/rAt1Tbjwkpsx2yevQLndAbCyuG5PCJzHsx2ZnvAdCMgz/2025-06-06-ASML-800C-straight-chip1-santec-scan-fine_fit.png)

# Summary for [`Thu, Jun 5`](day://2025.06.05)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/11D79D86-D457-4072-830C-2FB6861E15F0_2/EgxaqTOdr3D2lGQ2GVET2U4KVcm7OYY9NZlPDQGd34Ez/Image.png)

We finished testing the straight waveguide, getting baseline measurement results. Important takeaways:

- The image focus is reasonably good in the longitudinal dimension. Probably it is best not to touch it when sliding in a new waveguide.
- If there's issues with power, only move the illumination in the transverse direction withr respect to the waveguide.
- The frequency of the bias voltage is now 10 Hz. Let's stick to this number.
- The SHG conversion efficiency is not bad, but also not the highest. It is likely due to the relatively bad coupling. 
- To normalize such effects, always take power measurement with wavelength scan for each waveguide.
- A natural next step would be to slide in a new waveguide, repeat parts of these measurements (you can copy and paset cells) as if the waveguide were "normal", to get baseline results. Then, move onto optimizations.

# Adianatic waveguide

(you can continue here [`Ben Ash`](craftdocs://users?id=d9d2fbda-3d0b-154c-637c-be9f41830cae))

As a baseline, we find that (out of the long adiabatic waveguide), there is ~13 mW with EDFA.  I am honestly very impressed with this level of transmision.  Below is a baseline scan with 1570 of the poling period.  Obivously there is going to be a bit of a weird spectrum, and we will then have to figure out how best to do this.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/6FAC515B-C6F0-471E-B2DB-F3C20BA1F7B7_2/Q6MnfcyxV06zYQ0NaxWGzko8TvMLGSrMnKly42Oxqqwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/7A88B9A1-3F3B-474B-A91A-D544B82CFAD0_2/F2ZgogDqDJkzBgmjWveJeBbmanD73Bq6sN5LbBlY3Zwz/Image.png)

We see an objectively very wide poling region.  This is somewhat to be expected, as the waveguide has a large variety of widths.  We also notice that the height of the signal is rather low.  Again, this is to be expected, as each poling period only effectively poles a small region.

To get a rough idea of what the real poling structure looks like, we are just going to do a phase-pp scan of the entire waveguide length.  This should just tell us the general shape, which we can fit to later once we have some intuition.  There is probably a fair argument that we should use quadratic fits to check that we are working in the ideal regime, as waveguide should not matter at all for the region we are poling.

Below is the poling from one of these phase-pp scans

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/F9206ADE-240D-4FCF-8CBD-18AC775EC445_2/N0D4FRcMycUx5yf8T5wrTDf1qGWENJFqltO0lkDBbosz/Image.png)

The beginning is off because there is not enough signal.  But the ending section looks more like a V (which is kinda what we expect

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/C09D187C-48A2-4EFC-99F5-D07C7A947233_2/tiC7qBH9eUllHhnIEVOyylU07xo8yLtzg6IvgfoH28Iz/Image.png)

So, when we parameterize a nicer fit, our free parameters are middle position in x, top poling period, slope.  Alas, this is still a large space.  I can kinda fit for center x by intuition about the poling structure, as I can look at the GDS file and know what it is.  In the future, if we make more chips like this, we should put markers for where the middle is to make our life easier.  The first and more important thing for us to figure out is how do make the phase continuous.  The basic idea is we want to have the phase be continuous at any boundary between poling structures

I am going to code a quick correction algorithm for the first few points (though they could struggle from a lack of illumination)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/EF51BA98-6461-4CD4-A9E4-2342474E3F8F_2/w6y0nybbCyRQVcfhiFyKuFFxMynhxQSKpOMnkPFx1JYz/Image.png)

Space

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/407444B0-D1DC-404A-9ABD-3CEFB37B7E39_2/dTzZpkxiPCYCcxiRCAyeUfnqiz5sZQ68XJuXeCjyy3Ez/Image.png)

further along

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/48A6E363-5574-4B15-8880-C10316D2F054_2/lsoGpXqt9V9WZuaQuExcVKAkWySTNR9hxIczpcYkYL4z/Image.png)

space

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/828C286B-5072-4876-BD59-9601F623024B_2/IurBzIQq2ms2cbtze2BViExKm2uVLuWs7Lmp7VqfWPYz/Image.png)

While we wrote code to make the phase continuous, it does not seem to be working.  We don’t seem to get as much signal as we would like and even when we scan the poling period piece by piece (using the phase inference method), we just don’t see much signal.  Honestly, a bit of a pain.  I am going to take power measurements and move onto the sine hump waveguides.  I will just do pp-phase scans of those.  I was hoping the phase-inference method would work, as that would be the easiest way to move onto poling with a structure whose poling period more closely followed the geometry of the waveguide.  I am also mildly annoyed that this waveguides seem so narrow.

Poling of hump waveguide

![Screenshot 2025-06-09 at 5.15.54 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/16280A14-2306-452D-9462-D658B8E68808_2/4mKLx5STcHXEhBCwO9fpxrBMYrehzSMV6dr0mtSRyEoz/Screenshot%202025-06-09%20at%205.15.54PM.png)

Lets part at 14.9 um and optimize the couping a bit more.  We will then run the optimization scheme.

When I run forward pass with zoomed in scan (26 points)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/BF46EB73-2F8B-4139-9FF8-2C795645BBA9_2/Mcxv2YIPFEjdYAx1yBPkKRna3lRNxDAlO7JWi4jCygIz/Image.png)

When I run forward pass with zoomed-out scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/B2FE153C-17D6-4310-89BB-11CC543F1776_2/V9hkGoI8Qxmb0UxiV2eqiJXWmAPAqWjmGuT8syWnKn0z/Image.png)

So the zoomed out scan is actually better.  How about that.  Below is the poling as a function of position for zoomed in and zoomed out scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/72AE431E-DC6F-4344-87DF-E20F1601C234_2/5NPSKUExIwZ82HHqD9LzwbfggTEHjXaC1qCTiUGXy8Uz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/786E69EF-9D40-4CBC-9F96-A07206E497A6_2/q8Hx6l67s4UCnP1cee738aFg0yIc8BfBJlPc2RQoWHgz/Image.png)

It seems zooming-in too much gives extra noise.  So I still feel like we should get something that looks smooth.

I think the biggest issue I am having is I can’t seem to “see” the ideal shape of the poling structure.  I would expect it to smoothly transition around, but it seems to not do that.  Some of this could be the limited poling region we have compared to the length of the waveguide change.  I will move to some of the faster varying waveguides just to see if we get a more useful-looking shape.  We expect that we can pole 7 mm, so lets go to the longer adiabatic waveguides.  We can work down from there

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/E5A1E323-EC34-4FF8-84E4-EE6C11882455_2/pdKyyjyaMxvwpIGpbrnN2CtTvaLljJJlccywNrJ2drQz/Image.png)

Above is spectrum from 1400 period chip.  Lets do 20 secions and scan from 13 to 16.  We are now running the scan, we will see what we come up with.  I see no reason to add extra sections later (so the multiplication factor will be 1).  Lets just zoom in the pp scan a bit

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/F60A7B9E-EAC6-475C-9657-CC9C3A98D2A4_2/ch5lEDp71ZVn85zMkt8fzR0DPkfoeXiHpZlW9o6iTu8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/B15186C6-EBA6-47D0-B2C6-9A99E3316D9F_2/bFcZif00bL7EuqxYNci7y8Bg10nYiDsdcY39nZZQ0T4z/Image.png)

You can definately start to see periodicity.  To make this better, we would simply need more points.  We are now going to try something that might be a bit faster.  We are going to use our intuition that the poling structure should be smooth to slowly optimize the poling.  The main idea is we take a very detailed scan of the first section of the waveguide, lock-in, and then do much smaller phase-poling period scans.  Each time we optimize, we only scan around the previous section’s optimal point.  This is because the ideal poling period should not have moved too much

Below is 40 point brute force scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/63ACB1A9-0C3E-4C2F-92C1-191154473541_2/YqIcUCxBuM3Efo5PhCG70ULDeE8KADwP4RIvQPXYw6Yz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/BD3CB2D4-2247-4040-900F-73EB5DE0F3FC_2/50H2MdSHl1dqeCdChAXKcIm3FW9tSmJdUVUcy6kosfYz/Image.png)

This is definately a reasonable poling structure, though it is a tad annoying that we see slightly less signal.  It is also not much better than the perturbative optimizer for a similar number of points

Below is the transfer function with the useful poling pattern

![Screenshot 2025-06-11 at 10.57.44 AM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/CAFA61BD-5D31-4593-83AC-BB6908DC09CE_2/HDZXxpQlH3jGTs5hxK5HdYzj7mKNHfco6qpEsobouOcz/Screenshot%202025-06-11%20at%2010.57.44AM.png)

Below is the transfer function with a naive poling pattern

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ECAB3CA7-2287-4192-8EFB-A10B8E774F44/BB86A49E-7185-491E-9661-CAEE7F552E11_2/V9cqbUQcARqumUNkM841svmEBIZl1CAbfqj8xVxwixcz/Image.png)