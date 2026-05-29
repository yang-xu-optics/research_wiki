---
type: craft-export
title: "2025-04-07 special oxide deposition and etching for reduced bending losses"
craft_document_id: CABA1948-4897-432B-840C-3E02E2383972
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-07 special oxide deposition and etching for reduced bending losses
While testing the previous waveguides, it seemed that we were seeing a lot of bending loss into the photoconductor due to bends in the previously fabricated negative devices.  While I have not run rigorous simulations of these bending losses, intuitively, more oxide is always better.  The way we do this (getting more oxide on the side) is either CMP or etching.  CMP is down right now, so we can’t use that.  But a way to do this is deposit extra oxide and then do a very directional etch after.  This is nice in the sense that it is very controlled (Even if it won’t solve the lower breakdown issues).  We are going to do this to the 4 layer device.

Currently, the device still has Cr hard mask on.  So we need to etch that off.  That requires 15 minute Cr etch and 15 second BOE dip.  We then want to move to the PECVD.  For TEOS, we know the dep rate is 55.5 nm/min.  This means, if we want 2 um of oxide, lets deposit for 35-ish minutes.  Obviosuly, the clean afterwards is going to take forever, but that is totally fine.  Please also add 12 minute pre-heat.   We also want to put in a witness sample.

Next, lets etch.  From previous experience (a while back) we found the etch rate of oxides on pieces (so attached with cool grease) to be 150 nm / min.  We will first season and etch the witness sample for 3 minutes.  We can use that rate to calibrate the etch of the main sample (though we guess an etch time of ~6.6 minutes.

If we overetch, we can always just deposit more high rate oxide.  So I am not super worried about that.

Below are the steps:

1. Preclean for 5 minutes and season for 2 minutes PECVD chamber (season with TEOS)
2. Run TEOS deposition for 35 minutes, expecting 1950 nm of oxide.  (Add witness sample too)
3. Clean PECVD chamber (do this is parallel with things below)
4. Clean Oxford 100 chamber for 10 minutes, and season for 1 minute
5. For the high rate etch (below is an image of the recipe) for 3 minutes on the witness sample.  Measure the etch rate on the witness sample
6. Etch such that you have roughly 1 um of oxide remaining on the top.  
7. Try to use ellipsometry to test that things turned out ok.  If they did not, use high rate PECVD to make sure you have enough top oxide

Below is the etching recipe we want to use.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/696fb160-0893-a92c-adea-89ab784f0767/F04HayeynvxpddoXEsmPohTWv1wG7oendD34Lb7jy6wz/Photo%20from%20Library.jpeg)

We want to use the four layer device wafer box!!!

# Note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

14:47 Cr etch started. We did acetone bath beforehand.

[2025-04-07 Fabrication of etched waveguide with thick core](https://tdwg.craft.me/5C86K6Mt8nfxJx)

Beginning part of the process

15:15 Acetone bath

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/144DED71-E2B4-4221-A10B-09F0DAF0B278_2/rKNyIptxwbaY7ZOK8snk5aAxwrDKykQVhwibgQBkJ6kz/Photo%20from%20Library.jpeg)

17:43 Logging into the tool

## Precleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/CE5B8EA3-5C1C-4086-A270-F17C8E160E7D_2/8SUMu8nIMCBkh1SscDPI83k6vRWKZppfrpCwnTz0zlAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/403907CF-AF42-4F6E-91DA-AB63EEDAA041_2/MHp2yt8yOpaxu0l38vKYVEZgErybqQ5nkTcYNpMcx4Uz/Photo%20from%20Library.jpeg)

5 mins starting 17:45

## Seasoning

We use CNF CMOS TEOS

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/829F0E07-BB56-49CF-BB5B-F26DE58A0701_2/xEhTYhMiuTSUE6tIV9D8v615yT7kbR5HBJMeKlU2x1Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/2BD2E39F-FD46-4501-A429-1DD16DBEABD9_2/DSh03UuY2HiQzDJ1OxY5qDZRm367RKHvIGsryujtZBUz/Photo%20from%20Library.jpeg)

17:54 Seasoning

This time, I’m not setting the heating to 12 mins. We do it for the main run.

18:01 Finished

## Main run

35 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/F49CDE67-4367-4BA3-9FF6-94ECC352EDAE_2/RXHyod3LSgYNrfhaqczhdDB0kswCg6KQcpMOWM0eWSAz/Photo%20from%20Library.jpeg)

12 mins heating

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/770B322E-7709-415B-B576-101A011EEC45_2/ZjTVGyIQWpllLpDMxHReyWguEU6QHuFAPiXPm5XgXNYz/Photo%20from%20Library.jpeg)

35 mins dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/6052E14F-D5E1-4D08-A742-8240397FAD0B_2/cePNC8VBCF0DLtax9FJyixiPoUqEdvjVfBurHuOYfKMz/Photo%20from%20Library.jpeg)

18:04 Starting

![Drawing](https://resv2.craft.do/user/preview/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/4610F8D3-0FB0-4B59-BC5A-733B6D31F02B_1/gTuAmtRCZIqEqKv0P7GoHUYG0p8ZOQI2cxxYgMRtibgz/Drawing.jpg)

This will put extra 1.5 um of oxide

18:54 Finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/4032E7B1-013E-4620-AF29-6737ABB07F89_2/hcO3tZf9cAjGSFkw0Yh469q5IxT2EyQYJCTuV8pEt4kz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/D265C387-6348-4B76-A311-85E40460EB74_2/wxw8HGSa7HBXnKReWH9c7QubRcLzMNSPTm01WmXBVlUz/Photo%20from%20Library.jpeg)

No oxide? We need to do this again.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/9B961308-D44A-4EF2-A139-F057BDF591DC_2/YiKJBGuAWYq6HRMgHUkv6eZAU9tlG1MBHkxnzUOmckYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/5C5CAF46-70C7-4641-B9E5-29B04574AC50_2/eO5tdc9H4oEHExRLA0snNGvVT68i8w4Ngy7LpFqFJvAz/Photo%20from%20Library.jpeg)

No clear indication on how this went wrong 

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/0194499F-1662-422C-B8C9-310FDE3EE78E_2/eDCbfBmyUGKyya07IY63wPYnC9eRlKByMkZUqN2tfiQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/015F58D2-BB54-4510-8F8F-BE7CFBA928FA_2/e5n4lP4bhAOPLvZ5wbuWJhCZAAU6SqHxJoYnXjGM0Zsz/Photo%20from%20Library.jpeg)

We skip this process

## Retake the main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/6FC18572-BBB6-4530-BAB7-990974599480_2/1otrLc1OayRBgqSeQ0xxYduzIVmBDQ9CCsmv3KxnJzsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/79B884E9-EA1B-412B-8F56-7024E5A0A1B2_2/j4XsPDpobznaAF2HBi2GhLydYq1YySGmsUfL8in4qYgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/D62C874E-B831-405D-9742-76AC8D39EDDE_2/YaEyHQVg67boYxVICBBm8inEIXdbKzh4AiuSOPF2SWgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/F9AE7404-9C8D-4AD9-8CDE-B3E8ED7597B9_2/UOFYKV1uJEp6hWTqxrGOy0RFLKNDWOgdXghSlhdy588z/Photo%20from%20Library.jpeg)

12 mins heating, 35 mins main dep

19:22 Heating finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/1BDD664C-0635-459A-8A4C-2913E994A074_2/6CJ4Rf20EOTUWjYUlHz4T7Xk99cNlPTbzYQTRwtVsw8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/805FE56B-DFCC-4825-91AC-4E28DC7F19CC_2/jKCQQpcZwp6G4VnMqH7Y3JZPpmTzSnvQkysIO3cNOAUz/Photo%20from%20Library.jpeg)



We now start the pre clean for 13 mins on the Oxford 100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/9E9A42A9-47EF-4A2A-8FBA-2A8C71D19DA9_2/we0gwYZUBEr8Wh5hv4UoIOzGoWorkGp8sxqrg0xdEE8z/Photo%20from%20Library.jpeg)

Reminder of recipe below

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/F8D8D74F-3EAF-4EBB-88B6-0849EFA2C769_2/QipHxXrc4CeO9xoaJyEy993OmTYAApoD2ZQiSCBnNiAz/Photo%20from%20Library.jpeg)

Oxide and nitride are the same

We seasoned for 1 minute

Yesterday was a complete failure, so we are restarting now

I am running a 5 min preclean on the PECVD.  

Jeremy recommends we use the smooth recipe, pictured below

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/98B0158F-F3A4-4EFD-B04D-0804AFC00A91_2/dqFoztNVNh4mxsXC9AtsZGYpIyIhi8SaVvUKJZ3Q73Uz/Photo%20from%20Library.jpeg)

I will run with witness sample to get dep rate

# Note on [`Tue, Apr 8`](day://2025.04.08)

16:06 cleaning 5 mins

## Seasoning

2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/36F58925-27BA-4DDE-8FFE-79AEA8B8CF85_2/Y9Slc3y6pry0oLKV4yBD9ioBwOT1w6GocraLcxrTK7Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/D2F0125A-0CFE-4A1A-A208-8C09B6063857_2/zLVi8IYCfuwNLuwdHyZEwiD8yM4AGIVaQ36kop7sF1kz/Photo%20from%20Library.jpeg)

16:08 Seasoning starting

16:16 Finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/10E905AE-3F30-4F37-9578-A1CC274471AB_2/s3TKJWh4yYn6HM9u2k5Du9Kqh5hCybIE8U0pu4Skjtsz/Photo%20from%20Library.jpeg)

330 nm per minute. This means we need 15 mins 10 s of deposition

![IMG_0592.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/18DC9871-F352-44FC-B4D0-1474FE1B6683_2/nNDWRNbyZWeYvHDXvqSG77RjlQDUWzjjYxcMgDlU5Kgz/IMG_0592.png)

## Main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/D38F9EE3-0D27-46B2-B75F-45FF44CE0556_2/25eXA3IjFB62kPLxRqxsBheGJc57W48oou5HWCEUdaEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/985A2A71-8438-42CB-B669-2F4FA420F8DC_2/6b499Ip9pMKHpwDIW7fbrAFB0JKe650THy0zUr3QJAkz/Photo%20from%20Library.jpeg)

We aim at 2.5 um

16:22 Starting.

16:42 Finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/3F4BBC56-DA2E-408B-8CDC-376D73604EFB_2/LwxVuZIElx15zpj3tA0yJxtsCOi5qfxTwinN8raKR34z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/45ACEBDE-BA5B-4088-8AAE-F7888EC4BD7B_2/xluGN1AyCrtpdxkilNdVMtxkzE7h6CzMyUq6ejg0kbgz/Photo%20from%20Library.jpeg)

2615 nm.



## Cleaning

30 mins





I am running a 5 min pre clean on the Oxford 100

I am going to run a 1.5 minute season of the Oxford 100 and put a witness sample in to verify the etch rate

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/250ACA82-C600-49C4-8EE9-6DB87FCEA989_2/GIOkq4sZBuY9eY3cZwBnZykjpjM3uEE6HUXkK09KaQkz/Photo%20from%20Library.jpeg)

We use the thinner

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/C7D32200-DDB0-4256-8C3F-BFA3929774F4_2/klPO7Wvw91RdsSeI2qRYzoSyhZ49xPX87lygPHcLexoz/Photo%20from%20Library.jpeg)

16:54 Seasoning finished

16:55 Venting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/1635410B-165A-4A17-B859-9A925B0F3B20_2/GFmZx7lAV3s3dcqSYhpI5GxMF3Spyw4yvTpRF51Ewb0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/556BA6E1-DE23-43A6-83E9-A650CFF2AD62_2/n0d9pukMTLE5XutQZboEq7wVc0YjtnfiLHxgQFupWlgz/Photo%20from%20Library.jpeg)

115 nm. This is 330 - 115 =215 nm etched. 215/1.5=143.333 nm/min

215/90=2.389 nm/sec. 1600/2.389=669.736 seconds. 11 mins 10 sec.

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/E05220BC-EC41-4778-B096-7EC5E7CF285F_2/hbhBTQxQx17LWUE5yUke99pBoiadYrNLu4sfJ9n6GX8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/5DFC624A-2586-4708-BDF5-BE1F38CD89EC_2/o1PQzZlXPiy9sdCOqmbpCYz7VqBXYnhI2bb1E9WhqB4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/DEA217AB-1691-43AB-AF88-B43DD9DD099E_2/icYwJ6Ugd0SJzLx3EhvR7ah9Px6s9Syqkuv3gmiMgDcz/Photo%20from%20Library.jpeg)

Plasma on

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/280FA174-F997-4B0F-BF6A-CEC4C06C6BEA_2/j2NimxSqYg3MKjgm48KEIxMe4ID7SmyvihRHfzFFO40z/Photo%20from%20Library.jpeg)

17:23 completes. Stop and vent

17:30 Cleaning. 15 mins.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/A8244F8C-4B29-40B4-9417-5E4CCBC66225_2/Zx3C6sqOAinDMg6sSjUPXF8nJEf4gz3E8egWan32BEoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/464AEBDB-1ED0-4AA0-ABAD-5E0A4723007C_2/IzPLiC9iERYTkvGmzSu2tjVHMkSzEzdYyGNQsci3gnkz/Photo%20from%20Library.jpeg)

Almost perfectly 1 um!



---

# Retaking data with the IR camera on [`Thu, Apr 10`](day://2025.04.10) 

# Measurement of loss with oxide deposited

Using the IR camera and 1570 nm light source, we measure the propagation loss of the snake and snail waveguides with oxide cladding but with no SRN on top. 

## Snake waveguide chip

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/a9ed212b-716c-dbd3-4c52-f32af95fd958/CGJQpAu4tPJhMJG7LvGfGXdvf0Mde7LKWzy0skCWFJIz/Photo%20from%20Library.jpeg)

### First snake

3 mW / 49 mW = 3/49=0.0612 

### Second snake

2.7 mW / 49 mW = 2.7/49=0.0551 

### Third snake

2.4 mW / 49 mW = 2.4/49=0.049 

### Fourth snake

2.4 mW / 49 mW = 2.4/49=0.049 

### Fifth snake

0.47 mW / 49 mW = 0.47/49=0.00959 

### Sixth snake

0.6 mW / 49 mW = 0.6/49=0.0122 

### Seventh snake

0.3 mW / 49 mW = 0.3/49=0.00612 

## Snail waveguide chip

### First straight

9.5 mW / 49 mW=9.5/49=0.194

### Second straight 

9.2 mW / 49 mW = 9.2/49=0.188 

**Third straight**

9.4 mW / 49 mW = 9.4/49=0.192 

### Fourth straight

9.4 mW / 49 mW = 9.4/49=0.192 

### First snail

1.5 mW / 49 mW = 1.5/49=0.0306 

### Second snail

1.7 mW / 49 mW = 1.7/49=0.0347 

### Third snail

0.35 mW / 49 mW = 0.35/49=0.00714 

### Fourth snail

0.35 mW / 49 mW = 0.35/49=0.00714 

Below are the loss measurements for thick oxide claddings 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/93f8dfd3-ceca-5fc3-843f-1265021734b8/7yUf9bXeLlm1Bgd4I7BVLjTkfxJDUqtnxGASqwD02Noz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/be6098b6-1157-d74e-375a-f5773f594738/xw46ygMjKzaHCOS4aPanMWBrAz92ZjGyoAxdvblHhuAz/Image.png)



---

### [`Fri, Apr 11`](day://2025.04.11) Measurement of loss after SRN deposition

We measure the loss of the waveguides after SRN is deposited.

## Snail waveguide

It was difficult to couple selectively into the straight waveguide. There is a good chance that the power numbers include the contributions from the photoconductor modes.

### First straight 

5.4 mW / 49 mW = 5.4/49=0.11 

### Second straight

6.3 mW / 49 mW = 6.3/49=0.129 

### First snail

0.057 mW / 49 mW = 0.057/49=0.00116 

### Second snail

0.16 mW / 49 mW = 0.16/49=0.00327 

### Third snail

0.23 mW / 49 mW = 0.23/49=0.00469 

### Fourth snail

0.21 mW / 49 mW= 0.21/49=0.00429 

## Snake waveguide

Quite challenging to selectively couple light into the straight ones because we end up optimizing for the photoconductor mode. We saw about 1 mW in that case.

### First snake

2.7 mW / 49 mW = 2.7/49=0.0551 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/05B99522-6271-4632-8627-172FC50F4A93_2/sk8tSJQWUkOx3CbAcsrZZLsKS3MrjjMHGEt2wNX8FoIz/Photo%20from%20Library.jpeg)

Somewhat very good coupling and also the mode is solitary.

### Second snake

2.3mW / 49 mW = 2.3/49=0.0469 

### Third snake

2 mW/49 mW=2/49=0.0408 

### Fourth snake 

2.1 mW / 49 mW = 2.1/49=0.0429 

[Recording 2025-04-11 131317.mp4](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/E78A0187-C44D-4B25-BE58-35BA35850230_2/Rl5LKRWPCNc2jgfzi7nmyAB66EiEtKFf2RA5YwMu8PIz/Recording%202025-04-11%20131317.mp4)

We move the beam up and down. Moving the beam up couples the light into the weaker mode with tails of light. This seems to suggest that the brightest mode is indeed the main mode.

### Fifth snake

0.33 mW / 49 mW = 0.33/49=0.00673 

### Sixth snake

0.4 mW / 49 mW = 0.4/49=0.00816 



![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/DF23D846-E58D-4694-A7DF-69E09CDB3410_2/9q1TpTr7oPNxiKLrHbE9TFqhhO5TBUj6F6WLjKnZMxIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/B59D2EEC-5742-470D-9BF5-A0F17BFF4C22_2/mYeV24vs7cnyLrzSC4U4xeFlxTO1vaMC5cRUIy5eDOkz/Image.png)

From snake data, it would seem we have very similar loss to before.  It is slightly higher than we would like as baseline, but that is.  So thick side oxide seems like the trick

## Air cladded snail device

### First straight

8.1 mW / 49 mW = 8.1/49=0.165 

### Second straight 

7.6 mW / 49 mW= 7.6/49=0.155 

### Third straight

7.9 mW / 49 mW = 7.9/49=0.161 

### First snail

1.2 mW / 49 mW = 1.2/49=0.0245 

### Second snail

1.4 mW / 49 mW =1.4/49=0.0286 

### Third snail

0.32 mW / 49 mW = 0.32/49=0.00653 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/19D8141A-CBE8-4152-B96C-F5C4099EF16B_2/nOAo3zOZsI5hFaV5KZrohQnRriK2kkkCHYSqgEht2N8z/Image.png)

Interesting that we observe again that the longer difference, the lower our loss guess.  Either way, I am generally confident side oxide worked.  Below is the full document for all these loss calculations

[2025-04-10 Cutback Loss Measurement.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/CABA1948-4897-432B-840C-3E02E2383972/974F8941-317A-46F1-A774-A7A4CE80313C_2/ujagf62CPvhzLAefSxcyEyozyO8rYEzzyRU2Tv0xZecz/2025-04-10%20Cutback%20Loss%20Measurement.pdf)