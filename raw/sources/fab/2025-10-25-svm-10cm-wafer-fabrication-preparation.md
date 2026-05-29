---
type: craft-export
title: "2025-10-25 svm 10cm wafer fabrication preparation"
craft_document_id: 2C998262-A302-4551-A135-EBED0CEF2E82
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-10-25 svm 10cm wafer fabrication preparation
While SRN3 has lower propagation loss, we know SVM has higher conversion efficiency because it has more Si.  We would like to get an SVM wafer ready such that we can test higher conversion efficiencies on it.  

We will put oxide on SVM wafers (which will be used as a hard mask).  We will do this for two wafers just in case something happens to the first.  In the past, we followed this proceedure: [https://tdwg.craft.me/idzUWVVxdYBYsl](https://tdwg.craft.me/idzUWVVxdYBYsl).  We will use 6:35 as the oxide deposition time.

The first part below as done on 9-28

During RCA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/E2080974-AB05-41AB-B97D-E659617A5037_2/qveOksjvxkuqkYWnu3ssUPnTAMSWLPJy86uxgVNr4lwz/Photo%20from%20Library.jpeg)

### PECVD Cap Deposition

We run 8 min pre clean, and will run 1 minute season after.

Before 1 min season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/07DF6BA2-0D44-4B4F-96AD-8D0F5C7F466C_2/LwaC1Ev9PV8TBcEFPRSI2CZTxwkg1eFyFOhtbMqhBgYz/Photo%20from%20Library.jpeg)

Before first dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/21BCCF76-3A62-4A77-BDAE-093715DCF7B2_2/IkKR5O0pQSkvrm2m4VunR1BIFCTA7peCpIubkedyqxgz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/1F06A1DD-60F8-40B8-9E6B-C849B1D056E5_2/9hoWSxpazqVYryBsUo3NGIXjEwbITDXIr6unXt7U6pgz/Photo%20from%20Library.jpeg)

Ellipsometery of first

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/960979E3-0249-4611-820D-A3EBE31AFA47_2/4PC3lkxcSTJ011pIbpHPl6KrM6mobPINEY8UZGqQV0Uz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/DE853B45-1F0D-4A85-B848-2652B2D67A64_2/qXjgrOx8jIlDx7kSrIRty8YjEZIyK82IeUZqCTpxaBcz/Photo%20from%20Library.jpeg)

SiN is a bit thicker than I remember, but Pecvd is good

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/7C5910E8-EEB3-44EC-918C-B85F3D22665D_2/P94meE14D4ETtFZxFfcToFTT8nIyNPfaoyEtsn03HBQz/Photo%20from%20Library.jpeg)

First is 800 nm SRN3. Back two are today’s SVM

### Remaining Plan

This part was picked back up on October 25.  The Oxford 100 was down for a whlie, so we were not able to get doing on this for a month.  How clean the top oxide is does not really matter, but we can do a quick spin clean just to be sure.  Below is the process we are going to follow to pattern a wafer (and we only need to make one.  Nice to have the other in reserve in case something strange happens).  We currently have 1um of bottom oxide, 2.1 um of SVM (suppose to be 2um, but I guess they were generous), and 1.1 um of top oxide.  Obviously fits with this much film are not perfect, but it gives us a starting point.

1. Spin coat ARC on gamma (recipe 1002) and 800 nm of DUV resist (recipe 1206)
2. Expose in ASML using defocus of zero and dose of 18.  Do edge clear first
3. Develop in gamma using recipe 2010
4. Descum in Oxford 81/82 for 1:20
5. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe (it seems we raised this time slightly from 7-1 to the 7-30 deposition)
6. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
7. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
8. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition
9. Thin top cap oxide (while preserving thick side oxide) using CHF3/O2 etch recipe.  Run this recipe for 9:30.
10. Cleave wafer (so the bulk SiN parts are as sliced up as possible)
11. Run RTA at 800 C for 5 mins.  I would ramp at 5 C/s.  Hopefully this will help prevent explosion
12. Deposit SRN8 for 48 mins to get 3 um.  Do this 4 times to get 12 um of photoconductor with 25 minute cleans and 1 minute seasons between.
13. Sputter ~35 nm of ITO (including the material sputtered beforethe shutter is fully opened). Be extra sure not to put electrode over any exploded SRN.
14. Cleave facets at this point and potentially polish facets.  If possible, try not to leave too much propagative room after the end of the poling region.

From intuition, given the losses of SVM, I doubt anything longer than 10cm will be useful.  Given the plateauing effect of SHG power near the peak, I don’t think 10cm will be that destrictive.  I think we sohuld just expose the 5um and 6um 10cm long spirals.  I think the poling condition for SVM will bias towards 6um, but we will see.

Below is the distribution of our images

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/06B1CBCF-8F40-4E7C-B95E-4A74F1F21CF7_2/dOXcnlTS8Dy1TUba6OB3Xg6v1eAL13pexQHLNVOoKnAz/Photo%20from%20Library.jpeg)

I accidentally overwrote the old job.  We should probably shoot an Si wafer beforehand just to check

Double check that we have right wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/67D5CD55-2A7F-4E1E-A351-28801C6720B0_2/pbMGPQ7uNHFgq29PPH1JTqccZwBBO6WB1wRqviyRSfUz/Photo%20from%20Library.jpeg)

We will spin clean and get started 

## Photolithography

Before ARC

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/B23122CF-3B28-4C59-9431-F48577040995_2/nswLusxxCBACalOYcJcRlQx5IgD1hdpMosvxFUrYaykz/Photo%20from%20Library.jpeg)

Before resist

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/F150F84C-DDC3-4304-A471-835FE0733F26_2/ELNSpPBW4H3Q2UbhRnElu55HkqhyTFbhiFvEn1tssHwz/Photo%20from%20Library.jpeg)

During edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/311634E1-59ED-4356-A76D-940510413BDF_2/dSP9wnxDW16jZx3jdmEruekhxQgm111wGnVjW5B9Smgz/Photo%20from%20Library.jpeg)

During main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/186E4522-7146-4E69-A00E-CE10FBCAA5D2_2/unk6kVwJW24FvgX4uUAa9ds69D71OewyxKtiXzrk6skz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/A9B10EFE-D670-4625-BE5B-1AE4EFA63CE5_2/i5IWDovI5ShuAYSA9nqwQaziMCBUxjz1N6dC2ipqw3oz/Photo%20from%20Library.jpeg)

Before developing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/F3B4B5A7-FD7C-4789-94E1-0604FF6EEB5F_2/rwZDpx6hLjChDf6YzJh4qDxZoTnzg7Hhe3foBxgIV0Yz/Photo%20from%20Library.jpeg)

After exposure 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/16F3485C-AE0A-4D65-B932-76E58DD27C01_2/x9AjP1xNMoAX3XBRlWQo3JakyDo2dEhHX9e5sLrdxuYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/FCE90813-90B0-475F-95B7-0E5DDCC672E0_2/TWBLWVsKpar2Vai7yp05QCnScCGfKLQe8KSH9yTcSawz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/29CF452A-7753-4E6A-890F-021A8270A91E_2/3VhpMHiCV0reOTnuA4SxNGJRwoZzw8jq6niYmdop2psz/Photo%20from%20Library.jpeg)

## Etching

We do 5 minute pre clean on 81 and 100

Before season on 100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/B6150508-CBA4-47C3-8997-1729F0F8DFF6_2/vSU2Zewst0PvAYsyDz1gMJUcAMW3e2MrbJ9EVkEE3lUz/Photo%20from%20Library.jpeg)

Before descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/676C1EDA-0DFF-4D2A-9B6E-FF071E3214F0_2/y7MigLeewfqS9csboexC7Nn5IbCqA0gT7rHPhyuopu4z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/80F2F920-FD25-4CA1-AA83-444068AD105F_2/Yan76o1e2lkx4cqLwDzWE6hzYxf5HQIsOHeO3y5d9W4z/Photo%20from%20Library.jpeg)

Before oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/54D2F99E-CB3D-4850-AA36-46AD13BA325D_2/hnWUHHONI5BEAyBAGcFVTXUKcur1uLGjpjU0HgUH3c8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/E0B49888-3336-4718-825C-A03458F7885F_2/DhVHtewcmKuVXd09Onp9bueUxnkStRN0XcTc82MG9Agz/Photo%20from%20Library.jpeg)

We run 8 minute clean

Ellipsometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/801B2CD4-A7A5-4A8C-85A0-B816202890E1_2/ZmuAArUX9yHio9CKnp7sGqNTCl8Mi7xCK83ylPx2MYYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/81EB57D9-D78C-45C5-BB05-CF18A5E303E9_2/BZ8WATUVIBRDHSaSnpgZRi7YrQt5LdrQxMCs9bp0yq4z/Photo%20from%20Library.jpeg)

During eco clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/5CC08C0F-1BE5-46D7-881D-D90E6B44E444_2/5cqtmZFaSQHyU7NYUJYjsdrdg0soCWiSSooIbqEJzI0z/Photo%20from%20Library.jpeg)

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/21E990BC-4D3E-4CDB-87AA-E635B74C75B1_2/qqBosV4rynAEy5utvUR6FaalqEdtCBUUxvDUnFS5PXEz/Photo%20from%20Library.jpeg)

Before piranha

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/469B127E-3B2C-4289-BE66-E46780818CFD_2/0ofc3osoesEBEQw4xs8uChjbWlx7BdLL5DxWAi8UmzEz/Photo%20from%20Library.jpeg)

We have a lot more oxide than we expected.  Lets do 6 mins nitride etch.

Before nitride etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/FFE97E5D-8349-42D2-8B96-56479F92A2A4_2/BqeFVggKH746UyPPb6c5uxW4I3uzKclonEexqf5j85wz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/530C5C37-B684-4DDD-AB72-C2AE2C5C1DA8_2/RNqehzD7mDc23P9ywzsOHggLgIN3X2GUiHLSPdmXgh8z/Photo%20from%20Library.jpeg)

we run 13 minute clean

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/FCBDC1E9-2668-4536-BD35-A4A85873105A_2/UwHLloziXsVy0LR84yqQV5nxzT3DfJ0KYrocyizUK2Yz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/7B1CB9CE-C390-4400-863E-F4B96E3D2AA2_2/7jg65y0Vn8u1ojoA2uXQACkSX83GeWJ8hlkw9t2GvCAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/7313B5CE-61F2-4CEA-A154-4A2861FB5FAF_2/VOIJQ22JeJdjCwyACssMHGCqxM5oPyEgV2vsaq8CdPMz/Photo%20from%20Library.jpeg)

We now run piranha clean



## Top Cap Deposition and Thinning

We start 10 minute clean of PECVD

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/A1CE5ED1-E641-4EE0-B6EF-5DF097475F9E_2/m0zwqjL0V4guQlVtVsMrfvj0Lfp3Smybu7EqSfHZAW4z/Photo%20from%20Library.jpeg)

We are going to skip BOE dip

Before first dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/310C4D1C-785F-466E-93CA-497349C764A7_2/pyhifK9qsMTvr7FjTeSAWSgxVNP5RJaB4PrOp1Myfy0z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/2507AD2C-59DD-419E-89EE-B166500EEC3F_2/d16HqxD966bIwvwjaUADeJUNSqFFzRsAJUxrANdAgocz/Photo%20from%20Library.jpeg)

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/071A657F-7244-4425-83DA-2490AF4775C5_2/m1aYOCP4xlF2TRQ19LZFU2YfWxfI9WasIMqwxaPVKykz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/E96CF22F-36F0-4ACA-89A6-C32164F1F10E_2/gI9rl7QNIfbE7Do8guDIZgS3aGy9Sx9M4CtydFCpvSgz/Photo%20from%20Library.jpeg)

During second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/23AA53C8-E2D1-4740-B688-8F975FBD28B9_2/wCqxG5XUSROdd1CxdY2MrUIZBxEYzsy2leufMBavRcUz/Photo%20from%20Library.jpeg)

Before thinning season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/DD0FE1FD-A6C1-47B3-8FD2-49FB7954C86E_2/eeQHGGrcgvxW4dWyDytAL1K2yk9ZYZpxZziD5Zykk5Az/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/5B4EB90C-24EA-4B46-875C-3C1D367BB648_2/LwPp3Q6xPzYRMTyNfkswQ2zFzVvz3FhVDay9xx812z8z/Photo%20from%20Library.jpeg)

After deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/01A31375-93C9-4AB7-9260-CFAD204C1146_2/jgsRPGlB1Rkgx5fidifBPmZo6mByTjYRFJxcwgyk70Mz/Photo%20from%20Library.jpeg)

We know this recipe etches at 168 nm per min.  We want to get rid of 1800 nm.  So I say we etch for 11 mins, and slightly over etch (as we do have slightly too much to oxide anyway

Before etching

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/EE0808CD-0BEA-4F9C-8C1D-A82296BC9BEA_2/Y1tXoGVtN5w36RxgzaWbxoUunZyx2bpVgaKN61VQaVwz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/7A494060-13E1-4BA4-A4CF-582E74F4C349_2/JAwNRAthR8gDZIkAmD4LHLXbeAJGMu5urw4u0D8uHtwz/Photo%20from%20Library.jpeg)

We aer going to jump at **10.5**, I think 11 is a bit much.  Afterall, we know we really only need a minute extra of etching.  Besides, given the time and cost of making this wafer, lets do it right

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/D39D1D10-7564-4904-B9D5-C4CCFBE9E540_2/oFZvYVTefXqTY2bhiOeYLxCnqwy1tymNf5rBIgThINQz/Photo%20from%20Library.jpeg)

Ya, probably needed the extra time lol. Either way, I don’t think this makes a tremendous difference. Given the risk of radiative losses anyway, this is probably fine for longer waveguides 

Now we run RTA.  We do 5 mins at 800 C.  Lets ramp at 5 C/s, just in the hope that this somehow reduced film explosion.  We will cleave first, and then we will spin clean after RTA.  Lets hope cleaving goes well, as that is the hardest step to control.  Technically, we should test loss before doing marathon PECVD depositions, but I just don’t think I see any reason this won’t work.  We are going for 12um, as a reminder, so 4 runs of 3um each. 

Our recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/206A5B93-AF30-4E5B-B6E0-0B4F46CB9C40_2/dQdyznqh68T6cyyfxm6pikTnykG7V7hjwzds2UL1cDgz/Photo%20from%20Library.jpeg)

After calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/499562BC-A92B-4106-8D9F-90C590C149AE_2/rbcxZtFSrfthPBGinnQeFZZrXS3gDky0yrTn4vQ8ax4z/Photo%20from%20Library.jpeg)

We are going two at a time. During first two

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/09FACED6-70E9-4FE2-BBFB-8421291F1133_2/4t5cyUdwFooPkMrqjbRnqFuxVxCuUxUFB5GAaXYXSw0z/Photo%20from%20Library.jpeg)

During second two

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/3871F0D7-0A4B-484E-ACD0-D8C033D2A24C_2/n7eWAXIO97qE9JynKiOG2CwGaOEINbtnYjhyeTazUroz/Photo%20from%20Library.jpeg)

Small dip and then recovers

After spin cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/CDEB6DA3-5FB3-4B2B-8419-D4D6DA27C51E_2/pThgGHY5yXDSNs9K4lklNZ6hJAkHKDNVGCjFAJ0bR0Iz/Photo%20from%20Library.jpeg)

Minimal explosions compared to before 

## SRN deposition

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/9E141DF2-8158-4C99-9B3E-2FAD7EE42172_2/kYmv8Pu8RZ32LyFvzLagxXWWAcAj8Vmd5FTky8c0I84z/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/9C6CB306-0378-422B-A9D6-71295D5F160F_2/yyjkd4Rq3Orm0W6IdSHdiUoWCX6xAp4GWMe8ianG8d0z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/D622E098-95FF-4576-8866-69D13D6A0402_2/ANGMcb6weouZqccThQgY9VrygmR2o0pMzXEWNLVqYbEz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/B781CD63-E185-4568-B6D5-C8A89CB31A6B_2/t6jZ0DcJhic8EVy3vwKcqyonazRpajRin51rdgxkRxAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/BF0410F4-20DB-400E-B041-161253399368_2/IOUfvnBD7prkSnufn5TLyIjcqjZCPYipIhUjnDOw4owz/Photo%20from%20Library.jpeg)

Fit is a bit bs, but we got the right amount of film

We now clean for 25 mins

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/671C41CC-EB79-410D-A1C1-8D645BEFB0D9_2/2URTp1dI0dFg6i5AgDBTIeTlLKnJqsCXqJCX3w7gpF4z/Photo%20from%20Library.jpeg)

Before dep 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/9F51E409-E6F0-4A8F-AE7A-1E4B440395A2_2/4onNLEwvdXFaGqHoAqRlSl0yw0Atckp5TMy0hw68XEQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/9504A24A-7A02-4AA4-BAF7-FD9D9EB1DC86_2/JmV8byO2XsHhxFIynJZH9mygRcyLSI9HCgeZNGeemUwz/Photo%20from%20Library.jpeg)

We are now resuming on the following day, so we get a 5 minute clean going.

Before season 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/46149181-4D49-4F57-AA5A-D6319E16F30F_2/57xrMkb32iVV1b8UFETJD3gANala3X4Nyxkmz4Ccva8z/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/B67A8D9A-B41E-4F03-B8BA-C3B1F18BB0FA_2/nerC0g4u3Kykl6IqnS8tG64AMiVutJ3c9Hh1WSm1dL8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/3A5E68E4-8DD8-46FD-BDA1-3F57C93E761E_2/bs0q2FoEIvgxeERtgGH8xnS8v8RmlJgdHDyiNoJ2aXgz/Photo%20from%20Library.jpeg)

We now run 24 minute clean (we will keep ramping this down lol). In future, we do 25 min clean

Before season 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/91585798-923D-4A2F-AF28-4DD21807FCA1_2/7aFufqDjdBWL9reAQfNSDLtsz2nMxmbvGGD6a8GBhJwz/Photo%20from%20Library.jpeg)

Before dep 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/7DB66900-807A-4252-85BE-9F6F87977822_2/TKLbIDh8xYoMF81beqwwYLJcS4FCjWATfxIUyTy02mcz/Photo%20from%20Library.jpeg)

During dep 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/3FB24689-6289-401F-A3AD-051A16D1F080_2/B4kKMdtcVtKRniPzZYu7w6X7ggeYNdY70fBcPXx5PS0z/Photo%20from%20Library.jpeg)

Before loading for Ito

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/FD6852EC-BD96-46BA-B43D-CA83FA99BFA5_2/YZWxmykQrjXVRlAYQNYmiuZ2FiBTxZil3WaON9aDy1oz/Photo%20from%20Library.jpeg)

Before ITO

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/32E206C2-C72E-4CCC-863F-9DCE41567CC9_2/ryBhhVIrIdtmygXh9tVC7IV7FNAxB8wtZsVdMz6wqzwz/Photo%20from%20Library.jpeg)

At end of Ito 

We started normal sputter with almost 10 nm. Will stop a bit under 35

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/0F80F118-AB2A-4942-ACBE-4DB2790F8BFF_2/fCSyEbgxdzWPowzvebXHSh44xOhDaFveyXmz5BBZGKsz/Photo%20from%20Library.jpeg)

At very end

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/DC8E7382-8143-4B8F-A2EC-DD82A3320733_2/GxFEGlrbE9qCye6VxapoH8hNbfORfVedwL7JAqyPtkMz/Photo%20from%20Library.jpeg)

At very very end

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2C998262-A302-4551-A135-EBED0CEF2E82/B024E273-97D7-4FED-8BAA-E5A31BFA19CC_2/sxxYTe7Ofaeua5OguU2AlzGIyhyAOiTAwFDSGuZtTLMz/Photo%20from%20Library.jpeg)