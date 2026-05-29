---
type: craft-export
title: "2025-06-11 fabrication of tapered waveguides"
craft_document_id: B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-11 fabrication of tapered waveguides
While we have shown super linear scaling over large distances, we seem to be struggling with sub-optimal scaling (closer to linear instead of quadratic) for the ending regions of our waveguides.  This makes Ryo and I suspect that there is some multi-modeness issue causing the SHG signal to couple to higher order spatial modes at bends.  Because different modes don’t interfere, we will get suboptimal scaling.  Below is the newly designed GDS file that I want to use

[Pad6_Pass4_negative_final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/BDF390B4-A58D-4D05-9BA3-0E59A122C7F5_2/AZN0HE6yWicokidN0SBzkPvoflEH13xww0B0SrqHj8Ez/Pad6_Pass4_negative_final.gds)

In this file, we taper things from 6 → 2 or 6 → 3 um wide bends, with differnet poling distances

# Preparing wafers

We received a new batch of wafers from SVM. They have 2 um PECVD SiN on 1 um of thermal oxide. The substrate is conductive Si.

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-001.jpg)

15:15 RCA cleaning them.

We process 4 of these wafers,

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-002.jpg)

# Pecvd

Before season

![Photo from Library.jpeg](../../assets/fab/2025-06-11-fabrication-of-tapered-waveguides-003.jpg)

## Main run 1 for 500 nm

We do 3 mins of smooth oxide deposition.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/E1ADD51C-34BE-4921-A55C-7A17FF06FAA0_2/VibgIwQHQKByrYKygBO40sAk20aXAU4iJyHMpggKrd4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/A5E99169-1B9B-4096-BC72-804C635EF3D4_2/tZzRy6zo61B7YDQPwOCjD9aQiJ18XRGUvJQ16WNxMYAz/Photo%20from%20Library.jpeg)

This should give us roughly 500 nm of SiO2.

16:02 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/D8659781-6872-44BF-8778-53731C3005E7_2/dYVKgNpibrl5SIzfxKvdTmch9HX1buq07PeAzXJbnsEz/Photo%20from%20Library.jpeg)

16:05 Finished.

## Main run 2 for 500 nm

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/66E05001-EC48-4D96-8C11-848E1A4B40A7_2/Sy1tIlbmg5QuwV8gdyiyNKmr87lSj3UrS0f889wae0Iz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/DA3E6DF3-8067-465C-94BB-5E180A608C47_2/aLcfjDoPW387duilhR6mFwyoa8AGIm8VWtl3LkaFCOMz/Photo%20from%20Library.jpeg)

16:14 Finished.

Venting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/AC8001CE-618F-41B2-8CA1-CC0D541CE776_2/z9whi0kbnNb3YbJQPXx8lqfKIs2p8xiKvYZSlb0lRtAz/Photo%20from%20Library.jpeg)

## Cleaning 10 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/34640DBF-41C6-4B2B-98CE-53E43974FE72_2/deTJsknwTjxGrE2XdmyuJOtxmsmnnlcwG9zRV1XHRU4z/Photo%20from%20Library.jpeg)



## Seasoning 

We do 2 mins of seasoning.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/6EE50608-BA73-49CC-8EDC-87F85C16EB8A_2/yGIFUaYxNyxxfkIyesBDstDEWbTfa0tKqRNPC53L6bUz/Photo%20from%20Library.jpeg)

Made a mistake of running this without setting the time. We jump through.



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/31C5F72A-2588-4042-9CAA-E3B99C30657C_2/cvXyqHhf9N3Vb2cqybLCiEkeFtCItvzCw5aDrJfptK8z/Photo%20from%20Library.jpeg)

## Main run 3 for 1.5 um of oxide

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/6E98C57D-ED54-4F04-A417-C9ECCCA48E92_2/xoxYjmg6DIcx2eqXvzJxqEyg02ut7Qd8Kjfg02AnLKAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3CD363A6-0EBF-4626-BBBD-106873B6313F_2/yf3m3x2JQfIpfnBIQhoyKuyyhTLd8hL03TW6vgKXDgAz/Photo%20from%20Library.jpeg)

9 mins smooth oxide.

Starting now.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/73EF8AC4-A75D-43CE-B4F9-D7F35ABC7033_2/ecZTjwBkef23laAuTydDTxRLt39eEfqpwxlV9q6Oxagz/Photo%20from%20Library.jpeg)

17:01 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/DFB1E49F-93AE-403C-A26D-DC20D7B0031E_2/4NAkLyxqdCZgjSizGw8Avj7z3DDmSbLe8LrEaiy6UyEz/Photo%20from%20Library.jpeg)

Finishes.

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/CF7EE831-E850-47F3-BE30-295E08014C23_2/vI6ptd1wQPNqUSyOWKswBJ7LFmEYCq6FmJotXyKTfQ0z/Photo%20from%20Library.jpeg)

17:03 Starting.

## Seasoning　

[`Ben Ash`](craftdocs://users?id=d9d2fbda-3d0b-154c-637c-be9f41830cae) run the seasoning

## Main run 4 for 1.5 um oxide

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/61F2F387-D259-4EA2-97C0-D565AB8AA1F7_2/rYsCmbpO5SAmVUNu98CioAno71qzZy3jbZYZr8IwTCwz/Photo%20from%20Library.jpeg)

We use this wafer. The other processed wafer has been moved to the ASML step [2025-05-23 Oxide Hard Mask Testing](craftdocs://open?blockId=122F1589-6CC0-4921-B10C-DEEA9900CD36&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/78E9363E-0B86-4DC2-9F43-364137C23EA6_2/DDyRiXMAfhMDMBUzOerxUb9nfbHYkIpnpXAV84q7lb8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/E42D661F-4354-41B6-BC29-613E5E384247_2/f6lrDcmxlabrfLJyVzkOmHSLh7vnEu1yp7eMBje7Zrgz/Photo%20from%20Library.jpeg)

9 mins smooth oxide

17:41 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/80877282-F8DA-4C93-8872-751F852BA5F0_2/9fnVd65Dmh3ajyZYpuH0voHCGkmqGyBlQdVvyM6yp1Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/D8556729-D3F0-4558-9DB7-FF67F7031AE1_2/GrN3qbQegMK2JxwUNzx7Et9U5llgTw6MykAuOsaj9dYz/Photo%20from%20Library.jpeg)

## Cleaning

We do 20 mins cleaning.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/BC3AF49D-BDBB-43A5-9768-9745665221D9_2/J7Lzt2Pyun97fNQoYZU9y4msPWZyvetN7hw2cbcRmyUz/Photo%20from%20Library.jpeg)



### AJA

Sputter recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/61564F4E-9FCA-43EC-803F-186AD5E3F61F_2/sOWBxY2hpAxxqMrtG4C4Y4b64xV1sTihby4akY4Qwzkz/Photo%20from%20Library.jpeg)

Pressure at load

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/A2B52260-8C23-4F4A-ABD2-38328F008F8F_2/WAbnB3XzjqhvlxnfJbfxSfjynyIeaY7pybw0W199jO4z/Photo%20from%20Library.jpeg)

During first wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/93578F43-E474-4C56-95CF-62818B6CE6B1_2/474bdWtN9SSCkXEFkMLzs7i5QSHBEr983oHVx5o7xpoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/1C4D277E-47E3-4745-BD2D-DA5A133D7CCA_2/xphXJ7BEElXDvXghb9LCmydIag9fgm2A3COiZCvzxqEz/Photo%20from%20Library.jpeg)

Pressure at load for 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/06609F9B-0117-4B10-BE3E-862636DB2CD7_2/tkX9arlHpCNSZsb7DNpWAS2x4q2Kr2zJVfObxtuukYUz/Photo%20from%20Library.jpeg)

During second wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/7FBF8663-E8E4-4AC8-B455-E3A431C6B54D_2/Bxm8lRBsutJO6gwNG93HjQw22tQ9iSzzyiz2fZyzsQcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/733355FA-904B-4D9F-990D-B72DD6A5C1A0_2/w0DDumS1Vw9ityV4FpegGH9xX3u3ISshZuyWJUmsmMAz/Photo%20from%20Library.jpeg)

### Lithography

Our recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3A9B08D4-6F66-48B7-A72C-2F4A6D22D088_2/Qa5GRgRuPDVpyroqHSjjVIMAlqCcoS16e8Z4yWyRwYYz/Photo%20from%20Library.jpeg)

We use 1805

During 90 bake for 1 min

New nominal focus. Still use 53 as dose

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/EFF98D2F-1439-43D7-A262-03257FB4DC6A_2/x7eqkzbPgDJPqiNMHTc86OpWPhzmly8hvoHsw2bDvcIz/Photo%20from%20Library.jpeg)

Development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3E52C766-2058-491A-962F-4F4E22C03ABA_2/LxmPULfAYmT7oI04vHB81FKn0XHG1hxC1mbckGi9GjEz/Photo%20from%20Library.jpeg)

We use recipe 4



# Oxford 82 for descum

Venting the chamber 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/2250F614-1A93-4F46-BDA8-389F4D8C5F00_2/tJ5mHvwXDbLmAlTFEOrbKZCxfCYCJXr2sq8yMCdaXy0z/Photo%20from%20Library.jpeg)



We realized that no Cr etch is left. We call it a day. We will need to run descum and Cr etch tomorrow.

The next day, we resume where we left off.  I am running 10 min preclea of the 100

We will descum for 1:30

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/7C61C508-AABC-4469-8726-8E1A09667536_2/DCbChM3gZ4S9qKdHvojIVN6KfU7qzbnY380k5fwj8UIz/Photo%20from%20Library.jpeg)

Before season for 4 mins on 100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/0E3E7F5C-34E8-4F2E-BD9F-A1746426B419_2/yJELG13SFh54sUVsHxwb7c9Pj7JzmSrvsARJg2IAfWcz/Photo%20from%20Library.jpeg)

We then do the full etch for 7 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/D376DA29-7D11-49C9-A598-339771205191_2/m9ynw90eoGRFUZxi8w4sxaDU3uBCsNGxZxJc2oWGRIYz/Photo%20from%20Library.jpeg)

Took 2 mins to Cr etch 

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/4A033FF5-597E-4BFA-A786-B44743EE2A02_2/c1gnXs0G4vacsMehnIucwmeXRXX5EkF632zWfS0WhDoz/Photo%20from%20Library.jpeg)

I forgot to remove edge bead, so we are going to do a quick clean clean before acid etching

Some gunk on wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/5B3CAFA9-8ED5-4395-B4EA-FB9C3EF01E53_2/BLDE9sLyRuTxSrmqwKlK4IELCIYHLE6Mjon22ozsgAoz/Photo%20from%20Library.jpeg)

we now do Cr etch for 20 mins and BOE dip for 20 seconds

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/84A270EB-B4CA-4AF5-9584-22F5144D1D18_2/45CHBkXmUxkKU0c1hVoMwNYeUVhTnXnsxLdZuj8pK1Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/62EA29D1-5BF8-454E-A250-0C44FF36D932_2/J8pOlBdF8RxLkzQxx5DFy2xmXfDPaNhrggbuXhrikPcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/CB995771-E95E-46F2-880C-8B3EA11E4A64_2/Qr99lKd6rxRh9c68hvk6Wx8AbZsRJ7SeoffYarjLxl8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/B0CD820D-1B90-4F9C-9292-96498B638941_2/Jv93pirv7kP8MZUUY3HfwEyAcxY4e6PChZyYTYPWeX4z/Photo%20from%20Library.jpeg)

Waveguides look un effected by dust. Probably just water or edge bead issues

### Oxide Capping

We first cleanf or 10 mins.  We do oxide deposition for 9 and 8 mins

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/003229C6-7FD1-4109-A66C-1FE319B921B8_2/aNRCKUm4kBqxXX2mDkmhM4WJadCFb1nanBdrJMqdTTgz/Photo%20from%20Library.jpeg)

Before dep 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/DA660AE4-63BC-4F1A-97C2-900D9379A0AC_2/xkq4vUDqtkleyp0znYexKTfXBGY96HEwbuJDbHNbIUEz/Photo%20from%20Library.jpeg)

Before dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/536DAED5-C7BD-43EC-9C9A-4DD83B9C2572_2/o124gay9CrOJ2c2GulNGOOuZyZunIbvM5Hi3D2LB8woz/Photo%20from%20Library.jpeg)

We do 8 mins smooth oxide dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/CA5805EA-94A7-4AF3-90A3-688FC0110368_2/SyIn6d3hypQYXsRDJGylh2xcXdhIpDLIuIxUkTG2oSoz/Photo%20from%20Library.jpeg)

Cleaning 10 mins

### Oxide Thinning

We now do season of the 100 for two mins (I left it clean).  We then etch for 13.5 minutes like last time.

Before seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/60F878BE-2BCE-41D6-B35D-58E8F9A6B546_2/KFnCFU0gvspoHq19cKncymUZandZiB3WJQxZycROxUkz/Photo%20from%20Library.jpeg)

Edges are comically dirty

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/FB300022-1FA8-4FD7-842D-0DCEF203CF31_2/6plyaBnxgIwHYdrTy7x3j77w5WmlOPLV1yKD4x73160z/Photo%20from%20Library.jpeg)

We now do 13.5 mins of etching

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/69FB60E3-0CA6-4F05-A4E1-ACB56F7F0DBF_2/dsDyVaExj9b43gtQuOPy8tyReK6xJZyho7Ez8dNG7PIz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/53940D37-8C48-4AB6-85D6-D3F7F05B2C41_2/VYD2vIpKEO4A5RxOmQFIsM7XpwAbMxOdpeKVXhvDx6sz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/FAAE40C7-2BFE-4566-9C87-CBCC41F764F9_2/xZ5bCxg14RglAINdcVaVQ2xWsEyRmeZNvpCRgXbyZoAz/Photo%20from%20Library.jpeg)

This is less than I expected. We should have around 2000, though I am going to check the sides now

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/6B877413-6E51-4AA1-95FE-0DAE531680D4_2/ZH5TD3gDRbkTVi1MZBIEpvM0Rt1iVstdzkdy8ylTw8Uz/Photo%20from%20Library.jpeg)

No idea why the middle had so little. Mate we should put like 2 mins of smooth on again

Another central spot

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/550BA6BD-B119-4BA9-92E5-7DE006359015_2/SmexV1yCmMWdpJFmeIXHlUBaaHrS1gYzYGwS7MmAgrcz/Photo%20from%20Library.jpeg)

We, def less. We probably over etched a bit. Either way, we can at least do RTA

During calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3051DB27-62D4-4BBD-AFFB-B4DDA96C3A91_2/9LiwNd0d3xGApW664TiUYEI63R2eHoDvhZsj7n1sTrkz/Photo%20from%20Library.jpeg)

During main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/D798F749-0918-4214-B85B-74413D3FD2E6_2/xOBdYIfxDXcZZNmLWTucZsVzL4BG879qKTmU278yXScz/Photo%20from%20Library.jpeg)

# PECVD

We add some extra oxide. We do 2.5 mins of smooth oxide.

## Oxide dep 

After cleaning.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/68FD69F5-9E43-4904-B5D1-9810101B243B_2/DSUak7gIsrO0PULjTiwT4qKgksxm36yq4qVaTFm6decz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3086D54B-B203-4CAC-B9A2-68858878D151_2/CeH8YbTt8fqIYbQLgCMAX8kFtEeL9S9yRFHgUXMyivQz/Photo%20from%20Library.jpeg)

14:52 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/A514A5C7-2311-4432-8C77-10A799ECF65D_2/Zrcbg2n5Boio84q0hcaC5XGHMe0MI63XypYPEH8z9Z0z/Photo%20from%20Library.jpeg)

## Cleaning

We do 5 mins cleaning.

Starting

## Seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/300E97A6-652A-4F62-8AEC-BEA2492B5305_2/5Fdxsndv6B33LM92fXoawNzRE9k1RH7jFuxjXO4FVrgz/Photo%20from%20Library.jpeg)

15:14 Seasoning start.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/D5900E4C-DFE5-4262-A576-0DEE6083052D_2/J05RTV6y4QdByG893jMBA701X6QvDOhpuDFxeGXVKg8z/Photo%20from%20Library.jpeg)

## SRN deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/9E18190D-7A2F-4178-87AF-39D864A480C3_2/awY8AyeKOP2mQ4ea93yxkIoAgfD6dl4bMGlXYBqxHCAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/3A9A40E3-8F9D-46D0-8D67-51BCFB6D1591_2/x0duyid2RFe9aTSszNwMogNyt5twrQTSCNbSscyi0oMz/Photo%20from%20Library.jpeg)

32 mins starting now.

16:01 Venting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/98DED071-B6C8-4B05-9D35-D5E13AAC410D_2/PYoWMSBer5eizEBQ02ZSwAcE4cd3YYKrelByYk1NEx0z/Photo%20from%20Library.jpeg)

## Cleaning 40 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/FD21F9CE-B001-48D2-8CCD-042512289E79_2/thYFUC8uvThaXxgyOY3bYzqxaUKXrqYizwGIUGyvp7Yz/Photo%20from%20Library.jpeg)



After PVD

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B16CDCC7-668F-4E65-8CDB-EA3E4F8A3D3E/BBA6DEDE-5F2B-4A9D-9F18-965D276419A7_2/YZ4gMdR2AJEvKzziVjtYggywcAAhd7DYRyABnm1L63oz/Photo%20from%20Library.jpeg)