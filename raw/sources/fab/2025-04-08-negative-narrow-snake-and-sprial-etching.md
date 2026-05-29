---
type: craft-export
title: "2025-04-08 negative narrow snake and sprial etching"
craft_document_id: 3FDDE500-85E2-4EA7-A013-774B7FE0B9E1
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-08 negative narrow snake and sprial etching
We previously fabricated negative spiral and snake waveguides, but they were too wide.  This leads to loss to other modes from the fundamental, meaning these are not super useful.  So we designed a new GDS (attached below) that has much more and narrower spirals and snakes.  They are not quite as long (the max lenght is ~7 cm) but that is ok

[pad4 pass1.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7A6A0695-9B23-46E5-8D67-B0D2B0AAED2B_2/8N3L95EOFCbZkfoKuRx2Z93fnely0z0xuRKOxnXOVdwz/pad4%20pass1.gds)

All rotated as well

![Image.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-001.jpg)

We are also not going to use a Cr hard mask for this.  We will just spin clean, spin prime, and coat the wafer with 1813.  We are following a recipe Gui gave us, which is attached below

![Image.png](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-002.jpg)

He claims this should give us a micron, but I am going to quickly check on a dummy piece.  The procedure is going to go as below

1. Spin clean, vapor prime, and spin coat 1813.  Use 5000 rpm, with 8000 ramp, and 45 second spin.  Bake at 1 min at 115 C
2. Expose on the MLA with 70 mJ dose and defocus of -1.
3. Develop the resist with MIF 726 for 1 minute in the hamatech
4. Descum the resist for 1 minute in the oxford 81 or 82
5. Etch the SiNx in the Oxford 100 for 9.5 mins (as we clocked the etch rate on these samples previously to have been 210 nm/min).  In the book, it says we should get 4:1 selectivity
6. Remove remaining resist with O2 plasma, resist strip, RCA.  This we will come to later

Now I will coat an Si piece using Gui’s recipe just to verifiy it works as he is telling us

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-003.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-04-08-negative-narrow-snake-and-sprial-etching-004.jpg)

115 C, 1 min baking.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/AC9DBE8E-5713-4193-AF8A-C99B44F1B338_2/hItnts54UmUBajWWfE2nmwvY4DEcD5ynVzyDRARqbQoz/Photo%20from%20Library.jpeg)

It is a bit thinner than we want. We make the spin speed slower.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/D14FA5D8-D872-4EF7-B38B-B7ACE7B547E3_2/1jfKzeLL0x5CxlgIlXowNB4mSON966GhTgYUz2eDxX4z/Photo%20from%20Library.jpeg)

Coating done

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/AFE62926-F997-4739-96BF-BB8FF089DDBC_2/VjaKdArBIZNoEFku0P1S6p2AJblhZnHlCppxy5MZ09Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6FBF8C0A-DF44-419F-99A2-4C3B88BAB308_2/pP8OcVgKKxSHX6B7qjNG2fke5tpwYns9BXPMprmZ9mAz/Photo%20from%20Library.jpeg)

# Development 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7714ECC6-5F96-4DB5-9B2C-B1FC1EEA815B_2/Xi52Z2iUEsaVgtHpYYdoUDIrnsIN8VlKHifxcZ031Acz/Photo%20from%20Library.jpeg)

Program 6

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/07885EE6-92A0-4553-91D2-058C3EF89E01_2/UhzuAunTsH7ahdsq85AoZx630CZGAisq8gbXK8naXhEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/756D1CD0-EB5A-4D8C-B5FF-64C4E9051727_2/vSPlsoCzAxvxbo6uevvTzKCQ4gj8J2DBhysKoZMduiIz/Photo%20from%20Library.jpeg)

# Oxford 82 for descum

21:37 Logging in

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B84F3440-A18D-4810-8432-2074114A64B2_2/aLy09Na0xe0KTc9h3ief35V8HDF4h1wzqtOVlzawANUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/0EF48CA4-D880-4A77-A9FA-A1D1683AE2AF_2/D0bzxCOI05y9nKDEXDs3XVnV2jOzzsBVRMwgCe68S2kz/Photo%20from%20Library.jpeg)

21:38 10 min oxygen cleaning

21:57 Venting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9A158B31-A274-41F1-9BB4-35BC1B5337B1_2/JcWavOAyU1BLytMExWVjJVfnszG1MyAdMxfmxVad6Okz/Photo%20from%20Library.jpeg)

1.1 um left. We can do 90 sec of descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/0F63C046-C7A4-4179-819E-25FD086E5A18_2/dcAVj06zgjyCsgJ2Q48uAkI6yidN2V5zuGL7Yfhf01Uz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/D00D197D-0AC9-4299-850F-4505B4F92875_2/ocno6qUwRw7T2xAjhgGeaXDsNNk2oZxMjWIasjAiswUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/A288C796-A254-4853-B4B4-D26BDC79FF8A_2/wyozo11MZyuDl1klensZnImOPWAEhGgpYKG9KLXjyyYz/Photo%20from%20Library.jpeg)

22:04 Start

Descum eats photolresist by 90 nm per minute

22:09 Venting



# Oxford 100

Below is before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/5C91A162-7D37-4A6A-983F-96FAE071B932_2/kklESxw3pdRnJZplrVTMr0hxr8d2hU2nXzx5yHGJDb8z/Photo%20from%20Library.jpeg)

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/084070CE-67C8-4040-B6D5-E8624932C5CC_2/aAdwK5Fg7gGtIh2xOTgsZca5Z5HxfSb6uWmyEBKUSe4z/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/A6EF5771-213A-442C-AD25-D9709592BC1B_2/Z8S5hylEyXX5ynV8EiFtyBmzO9thod3x26wd4lEMt8Ez/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/86F2C9AB-DCB1-4FB6-A5F6-CE5E1DE1D38C_2/V64RiTvuXAh0WOuxrIML72xusPEWiM5PWTzb8wTh7RQz/Photo%20from%20Library.jpeg)

Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/87E8770D-BF09-4B04-A365-D54E71D350A3_2/phyBSmZxXMtDUcPj6A0exKNpoVaIGHlazRGLPWBkka0z/Photo%20from%20Library.jpeg)

15 mins

We have the Si wafer inside

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/F9D6F165-8D90-4BD0-A40B-C3D85FE354F3_2/7dRTqKoJfGUsGXAhzxwExazcarecGWa7hZPBYZzPPMIz/Photo%20from%20Library.jpeg)

We have height of 2.5 um



# Oxford 82 again

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/8CEA35C8-D6DF-4117-BE21-E4084102F111_2/lFZCeWXKVFjZdBLx1CaZMS9yWnjAeHpGysU87aZqM6gz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/DC2FB132-A787-43CF-B6BA-6CF6D0D5AC24_2/iXys3i5P8Vc3XDm5sF5JNc1vGgTpIBC7jEKx3ZSXEvQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/F1B9418E-62F3-44BB-AAD7-196BAE220B3C_2/gwDJydtGlSuqVzHmKIol9ly7JioviZO1Y0JAyYLmyp0z/Photo%20from%20Library.jpeg)

22:47 Mild descum 10 mins

Finished

We saw roughly 2 um of height after the profilometer, roughly confirming the 4:1 selectivity (as the descum removed ~ 500 nm of resist).  I will also put the wafer in the resist strip bath just to make sure.





# Note added on [`Thu, Apr 10`](day://2025.04.10)

# PECVD for SRN

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B31183A4-AB49-4662-A026-D054FDB71C20_2/lFcU5KlxieyxTrhkENZxoBXzU3dF0fhJ5YUlF4lzA9Yz/Photo%20from%20Library.jpeg)

16:42 Cleanimg 5 mins



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/C4CFEB8E-1417-41EB-9D6D-1B9B61A13396_2/TzBs7JEsBZt74RHbsGgLe6LVg4jNkxlQDyqwhdSrzUAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/748F62E0-1D58-49CF-96D4-745985FF5AF6_2/sygLK3Mojco29etpmQzX4DyJZfyn4suOsRXZsxrT7yMz/Photo%20from%20Library.jpeg)

17:02 Done

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/764ADF5F-8CF6-491E-B31A-2A96B6AA2A02_2/K3tmuH7TKUC0sRrWfNkOSavD5l1fpfo0juEbXO8QJXUz/Photo%20from%20Library.jpeg)



23 mins for 1.5

23/1.5*2=30.667 

31 mins

### Main run

31 minutes

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/54D69E81-3C23-4676-A466-09FE2DE1CB61_2/B19RFUG44wQsiWkMkUxcmxkYsMge4usCUDiNxFqGxTEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6EAA0306-0C1D-4C5B-AC90-7A63319711A7_2/IuyvegyUYKwqfFKMwmwxGyZXqmxq3uA1Mj0vyRs7Cy8z/Photo%20from%20Library.jpeg)

17:06 Started.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/0022AF3A-6413-4461-A6B1-F8E4B6C2EE40_2/jAUtN0VQU4BFxCwR2WJQY6m7oUTxsjK2VeAATQFLT5gz/Photo%20from%20Library.jpeg)

17:41 Done now.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/766A1125-CE8A-4389-8D22-3C95D27C97BB_2/aDEDesHypqWA3rDyYka0tpeX4t9MEjWpPmEazGjb5rUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/AFF8BF20-0073-49B9-9CD8-24EF5E577084_2/UAVH0yFTnwcbcJJVxFq16P9rem5hc3kWp8ClhjXWhNMz/Photo%20from%20Library.jpeg)

Thickness came out mostly as expected

### Cleaning



---

# Note added on [`Fri, Apr 11`](day://2025.04.11)

We intend to perform PECVD deposition of smooth SiO2. See [2025-04-07 Special oxide deposition and etching for reduced bending losses](craftdocs://open?blockId=CC67967E-0650-4044-8C24-17BF920C8645&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8).

Last time, we got 2.5 um of SiO2 after 15 mins 10 secs of SiO2 smooth recipe. Dep rate is 2.75 nm/s.

![IMG_0596.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B2FB9387-DE07-4FE4-B753-B519A7FD4791_2/7QrKHvUkpPZH09YXCzQGIvbCyhxwGuXJjQcLtpLMvyoz/IMG_0596.png)

We aim at 1.5 um

![IMG_0597.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/72BBA31A-71F8-4C80-9E1E-B72B8280BAC3_2/8Xk3nO5ATbQWytBlyjFHOqFTbY1ecqXOOzpgM8bRJdAz/IMG_0597.png)

546 secs=9 mins 6 secs for 1.5 um. We do this twice.



# PECVD

## Cleaning 5 mins

15:39 running

15:45 Finished.

## Seasoning 2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/EF313334-DD53-4956-8FA9-C03037EB4657_2/yFyxRwWaN6Ys4eBEBP527TsGECsNytU2yywzCTcTDDkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/EC4CB98D-7337-4DDD-B643-0CD4F1155476_2/xBx8hx7E5CxhvkrQmbyjHCGMd3i2qfi7DlCt2tUl2Lwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/35F71FB7-64A9-4709-88E9-D5079B08979D_2/tilV8tNr2druxhRdLHrfBPFuM4biCEjGFX1XlkhhUB8z/Photo%20from%20Library.jpeg)

15:46 Starting. We expect to see 330 nm after this.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7168AD6B-72CD-4A37-B135-7171F3E06845_2/LIypecwypraCVe94VI3tNQYi18kAwEUbWpXy23utbxwz/Photo%20from%20Library.jpeg)



### Main run 9 mins 6 secs

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/02C511AC-AFC0-4C67-B409-36EA06F08E10_2/8GiBq6L7hisqIB4HPxmGgkgQNpxlKO7L4haGwDZaAlUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/797B85B4-E09F-401A-A893-FA36B7D94345_2/EFMlxOnsigSPfnOytvjyaFRuEa9Ey6gzyvx3IrHWh6Az/Photo%20from%20Library.jpeg)

16:14 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7B3BF5E6-2999-41F8-948B-91AC1E4E7EA8_2/t771diEu2j7bgKj7GC1t74nt5NDdSEPIsEeoLa9J6DYz/Photo%20from%20Library.jpeg)

### Cleaning 12 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/45F64574-91ED-4B81-ACE3-CCACB473B7D3_2/Vxym8xEXftQHnZWU7oe5GZoyNbv0mC0PKPAKSy4k0B4z/Photo%20from%20Library.jpeg)

16:17 Starting

16:34 Done

### Seasoning 2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B3174A81-9C1E-4036-9B89-CF13DCB64388_2/2s8OB1fuq4JTzBYlKH0ZCPfgBl5yMt7GZFgxPJurbD8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/C67CD28A-68DE-4BFD-BF91-61B1B06AFE8E_2/JQx7uZcBgDMcpoMwpFfdzP1oAfyMU4yqbtJBr58ZaRkz/Photo%20from%20Library.jpeg)

16:43 Done

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/95DBA08C-3F05-4F3D-A3D0-D6346B47312E_2/o6NYe54sk87nwLS0JMG0km1I7Huo0zwCq4ckea5BsuMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/83BF98A2-03DF-496B-8E0F-D7CF1F6D2B29_2/xpDDznJ3JUrhoDVs6hdyfd8z6D7PQiXlImMyaONVfYAz/Photo%20from%20Library.jpeg)

Thickness good. May be a bit thinner.

### Main run 2 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/FCCF1849-272A-41C5-81A4-562FD85758C3_2/eBIIEj3F4BgzOz1MuKSX1xH8qmNLLVSmRFO6KgfWi0Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/D4F0D82C-333B-4603-8B2D-8E2844BB0C89_2/Ez3wTyaSlTaPm4YlIqUZDBSlS8jRPXxnUCBImtTXxr0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/E2D4D0ED-2DEC-4960-801A-D631567E87D8_2/0ZRkFy9rjVAB5yOy2agTEBFgEpTUITzd78A1JR1XVmkz/Photo%20from%20Library.jpeg)

Second run. 9 mins 6 secs.

16:45 Ｓｔａｒｔｉｎｇ．

16:59 Completed.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/C52BBF0D-D03B-4587-992A-792484E7C6C6_2/imxbkdTKLZvVQmtuY9hn4xxo8u9dOSxvKxIyPuW5zRIz/Photo%20from%20Library.jpeg)

### Cleaning

24 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/87E548A9-5898-4F78-9E6D-2EDEDB4C0015_2/resJ1xeqkhRRG5oATkXVT6G62m8uBKVtZ0mh2QzBToYz/Photo%20from%20Library.jpeg)

Started

# Oxford 100 etcher

- Clean 10 minutes
- Season for 1.5 minutes
- We aim at 1.9 um etching
- Last time, we got 143.3 nm/minute or 2.389 nm/sec. If we want to do 1900 nm, we should do 1900/2.389 = 795 secs=13 mins 15 seconds. 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/7687C00C-087E-4588-AB1E-5C9C66B40530_2/E01EZwLSERjvsqCnKL0A9YyDZLLym7AxQsrlYEvboyUz/Image.png)

- To keep some safety margin, we can do 12 mins 45 secs.

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/E39752E2-B756-4B2F-8530-E7CFD6459C1D_2/6NnIpqztQFVl6yDwd4kUDDD6WJiXqbeUtnGKohqM6Isz/Photo%20from%20Library.jpeg)

I see a wafer inside already.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9D47960D-1D9B-4B55-8010-26DB19DB743D_2/pwQZUqXAlxnOcqAEx0HDVgrHYa3e7o5yIIjqYHbrNiQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/5A4771DF-ADAE-408D-B17A-112FA583D7D0_2/kUTyw6UzL9auSoyFeeSAM4pGdShbFUTI6PyoTpU1Rlkz/Photo%20from%20Library.jpeg)

10 mins Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B15464A6-BA8F-443D-9D0A-35C191B3DA76_2/Pc6dlUR1fQ15yf60CbezQUe8uK82Vli8tJx0fqTYsxUz/Photo%20from%20Library.jpeg)

Because there’s already a wafer, we do the process on this one.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9169B1AA-82C3-4656-9B9A-8555B49F6797_2/euee46UyxWxtZW9phbVTXGBloNt9BYuoqnhaXsQ6g5Ez/Photo%20from%20Library.jpeg)

16:56 Started.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/99B28EDD-F5FC-4214-8448-D5E16E801073_2/FSf2iigig08jYABB8Eee5ImSyQwGfQpMU4iOF3aTtFsz/Photo%20from%20Library.jpeg)

Plasma is on.

17:09 Wafer came back



### Seasoning

We use this one. 1.5 mins seasoning.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6C5E3F1F-9060-41CB-B33F-A3FB15CE6FB7_2/wq0BFbrM5yDJmXyorGlOMf4T9Myq2z5eqLI98eHOpUYz/Photo%20from%20Library.jpeg)

This is the same recipe as before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/71154CD3-9EF9-448D-ACC1-0DAC5D785803_2/Bfy5ZOVM4ixj7W4Q5yyfqy4rnLdmxIyIceReCzvwQC8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/CC51DE83-D94A-4B6B-A8F2-109749C8E3DE_2/G1LYg2YwOGZT941WqYW1WD3gr32d4O8FJox2MHixj5Yz/Photo%20from%20Library.jpeg)

Wafer is loaded.

17:11 Started.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9E862B64-E2A8-488D-BE7C-02F42FD9A09A_2/djlh7qzIf24uV4mmU0txkAQkHNrrh6kHj8DjUkhzFFYz/Photo%20from%20Library.jpeg)

Flow is okay

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/8EC2930F-D44A-46B5-AC36-DEF5058548A8_2/7d8g4JXFdQkCrBdH7wTXBRSTl0HTdwtFzr2HTsBUpN0z/Photo%20from%20Library.jpeg)

Plasma on.

17:16 Finished. Venting.



### Main run

12 mins 45 sec.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/5BEE3D36-2E98-4969-AEAF-CE48829B254B_2/Y3mY9sDEcBzxSbivvYHsYmM215QOOnHktwsJbY5cyQkz/Photo%20from%20Library.jpeg)

17:21 Loading the wafer.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/71E0AEA4-E78C-4189-A4D3-DE8F67376139_2/5ZKXwB9wcwDhEvezyocVdC6EdrLuyt0XLvcHNgxnlXAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/B51C3034-C0A0-4253-A012-326A18A5DB5D_2/rb3Jlb7lA7FeufAX18GWs6fHQVaU0LdjfkVCJLbwcI0z/Photo%20from%20Library.jpeg)

17:22 Started.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/EBAA5BB2-079A-4939-AEF1-5E51ED9930F6_2/rxm8gxcTDoji1F5CbV3je9OLi5ISFhne0Gn5iQutBzUz/Photo%20from%20Library.jpeg)

He flow seems okay

17:40Venting

### Cleaning

15 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/742CDB4E-6423-4764-ABA4-C767322F93F5_2/rhsdl8GPrr6rxFIM0LQkREHwWEA1NEODo3XSAryjYVgz/Photo%20from%20Library.jpeg)

Loading wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/00EBED46-B40E-47AD-A140-82FC58E8B89D_2/OxxADxTgOVqGnQSWSfhBAtgXzPYRYMjIZmqweOYuTJoz/Photo%20from%20Library.jpeg)

17:45 Starting

## Ellipsometry

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/D76A2E03-A6FC-4DAB-967D-1351A5DC7BFB_2/mx62fkd26yPHmXNPngSC1PIcLyHhi7axfPczfjGxbykz/Photo%20from%20Library.jpeg)

The fit is pretty good. We might have left a bit too much SiN though. The oxide thickness is around 1.3 um. Again, we could have made this a bit thinner.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6FC04C14-88FE-4B76-AB53-4E05073C6EA7_2/Oypa9LchyXpIHJxFk0iPlINDSQu6Hhu3YKerNxTbWI0z/Photo%20from%20Library.jpeg)

The fit does not change even after we enforce the pre-determined values of SiN index.

Now I am precleaning the PECVD for SRN deposition for 5 mins.  I also spin cleaned everything after cleaving

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6725DAA8-83BC-461A-99D3-8F396A4663E1_2/7hdVynjo9hCGrifqxcbKFfuwiMOq5rywEo1yEpY2eyAz/Photo%20from%20Library.jpeg)

Lets do 3 deps of 32 minutes to get our 6 um of SRN.  I realized after the fact that the recipe I input was slightly off.  To be clear, below is the full recipe we want

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/64a45b7b-8811-9ab6-7a7b-f35461127583/vRxSsdZS8guQuQhq0niKsuvM7vh1wRmVMNvc8PnBxsUz/Photo%20from%20Library.jpeg)

Before first deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/BA07420F-665F-4920-9E23-7B7DE9B34925_2/fFXBsyOhy0xxtAYC7Prbfsk0HQZQFgAMtMUOTOpJUUgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/FFBB4449-A173-4CC8-8ACF-3568F1BD4837_2/dSsCsZafEuDB4RmB1pQKxX9xPyyGf3tCOW5HF0MgMlsz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/D616C061-3A80-4DE5-8113-8A73A6399937_2/qyFa5KPA7AwwGrx2IWeuFb6KyTFChbuYdbNU09qn56Qz/Photo%20from%20Library.jpeg)

First witness sample

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9126379B-1A51-4E2A-9A44-5E7C5E53F6A4_2/7lOCgRHvM4PktNlDXBdzlgP8gZH5WcyMCdSihYZUBBUz/Photo%20from%20Library.jpeg)

Looks good to me

24 mins of cleaning worked. 

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/8AD0951A-8F62-4D87-9170-B61AC45DC28F_2/u54mI11tWjrBFUZqvIvbm76hmy5U13xsydEBwCC8bSIz/Photo%20from%20Library.jpeg)

Before second deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/DA9F8ED0-3E5A-441E-B786-8EC820E8771D_2/nKBIp6h5gjHdxwF3iZEJTBNyw7pFOo0UYpFEwquO5Wkz/Photo%20from%20Library.jpeg)

During second deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/DFADEE3E-7637-43B0-AF97-3663830F857A_2/bH0HCbd74fZ21ITRTBR3bY9oApl99ewtxlxPFPAmx2Qz/Photo%20from%20Library.jpeg)

21 mins of cleaning worked

Before season 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/9E9A498F-CD12-49BE-8FFF-7CF32EB17285_2/XVxoiNfkFP1uMg0vkeIgQWeinf0ylUVvBy1zwaXBsw8z/Photo%20from%20Library.jpeg)

Before dep 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/8D90F916-3BBA-41B1-97B0-DB86635BB86E_2/xYaDukDxSiTQceErJ58ubxKafJp2KRJYVNjQUpejgK4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/1289EEED-9933-4914-9297-D698AF12FFFA_2/kXsUk2TEd0PKgLLgw1znIn7FGpRhzbCN2FXIjVmyfOwz/Photo%20from%20Library.jpeg)

During dep 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/4DBE69E0-F5A4-4C1F-A09F-646F42243EBF_2/KhQ95Z1bOXSTA9GkLwVDznZZIKimmhfTWPdD4tTxN5Ez/Photo%20from%20Library.jpeg)

# ITO

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/572040B2-0423-4015-9DB3-F72B196394A9_2/a5m6OuAhQI2d0luWjGkxDYnSIEvuPgV65o8yvnDm1f4z/Photo%20from%20Library.jpeg)

At end of sputter

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/58CBD7D2-B273-4EF7-8AC5-8BAF0EDCCD94_2/NIpJJsJvIu2KxZd3ZY064eRc2B6pKsgFyxnwwTCklOAz/Photo%20from%20Library.jpeg)

---

[`Sat, Apr 12`](day://2025.04.12)

# Measurement of loss

## Oxide cladding device with no SRN

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/35E329B5-E191-434A-8029-2B797D692921_2/vdgLiNQ1xDW1xIWD9ON0PXmx9S9z2MF99PTXhmfnrYgz/Photo%20from%20Library.jpeg)

This waveguide has very low transmission. We measured only 4 uW at 1570 nm, out of 49 mW coupling.

## SRN device

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/82DDA2E6-A8E6-4AFE-B29C-460C50B07EBF_2/P21boz9Euf6pgiyIC584ucQe7N0eabD3pP6x6bk6mSYz/Photo%20from%20Library.jpeg)

We got a bit more transmission, e.g., 400 uW from the straight waveguide.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/BFD08F7C-00B9-4580-80EE-4CFE12E104F5_2/d8lLtOW2GsSlDxOCWHwa8fpsDhTyCziXtEbIdTb0d1wz/Photo%20from%20Library.jpeg)

However, the mode is very messy. Also, the coupling is much less critical. This seems to indicate that the most of the power come from the photoconductor coupling, unfortunately.

Below is image of mla job

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/6B2CFFC5-43DC-41D5-BBA8-E0A2BD38E4E5_2/ASyFJzb8WVK3alMD2x1wN3S2hiXZkxAbTvJ8QgJUxPcz/Photo%20from%20Library.jpeg)

New one

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3FDDE500-85E2-4EA7-A013-774B7FE0B9E1/30BA1F6C-C04D-493E-826A-CF6A36ED8776_2/bx0d5fZpuQyEzQfwPxOGML0GF0DpsDy7fKpbM0FaIPoz/Photo%20from%20Library.jpeg)