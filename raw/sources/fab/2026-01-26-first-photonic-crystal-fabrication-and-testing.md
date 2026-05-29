---
type: craft-export
title: "2026-01-26 first photonic crystal fabrication and testing"
craft_document_id: 7277444A-3193-4640-807B-8C7E67D3BB45
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2026-01-26 first photonic crystal fabrication and testing
As our last experimental demonstration, we want to show phase-matching on photonic-crystal waveguides.  Presumably I will start with phase matching on straight waveguides again (with better alignment of the illumination optics), but this will immediately follow.  

Here is our first GDS design

[Photonic_Crystal_pass2_final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/43657C18-F81E-4525-81F6-1006B8BF1640_2/9eyrcOYji5UC7hmgh728LkZflGcBg9gkNLL7Ylski3Ez/Photonic_Crystal_pass2_final.gds)

This pattern really looks at the size of the perturbation.  There is something to be said different doses can kinda screw with this, but to first order, we can use a dose that is roughly right and move forward with that.  While we do look at different grating periods, it is fair to say that we could scan that more.  I generally just trust my simulations as being pretty close (and other literature papers for much smaller waveguides are close-ish).  Afterall, the way you calculate this period is actually pretty simple, and the period is not super super sensitive to the errors we are likely to use in the neff.

This experiment hopes to observe a photonic bandgap using the 10th order diffraction mode.

## Fabrication

Below is the fabrication we plan on using

1. Spin clean the wafer (we don’t need RCA, as losses won’t be tragic for us)
2. Deposit 6:35 mins of PECVD smooth oxide to get 1.1 um hard mask
3. Spin coat 1805 resist using 2000 rpm, 8000 ramp, and 45 seconds. We know we have an etch selectivity of 4:1, and we want to etch through 1um of oxide.  So we want at least 300 nm of resist.  I think this thickness should work, but just…
4. We will develop the wafer using the hamatech tool.  We used recipe 6 in the past (MIF726 for 1 min).  Just check the number
5. Descum for 45 seconds on oxford 81 (I know we usually do 1:15, but I feel like 90 nm should be good enough)
6. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe (it seems we raised this time slightly from 7-1 to the 7-30 deposition)
7. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
8. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
9. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition

I would just check resist thickness after development and after descum to confirm that we can clear.

Below is Ellipsometer of starting SVM wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/AB40D56D-D40F-432D-B426-E7A9A96CCE1D_2/IbFMpy2HxqpyqiiNsTKnDqsQ0CCUXhEIluzgGTmywdkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/79BC1885-8C28-4D2F-BEE1-C41EC29F35C7_2/RFDpNhpWpNnoxPxZfyXC7WhNi3ELHUjo0lbUf68gVHsz/Photo%20from%20Library.jpeg)

### Top oxide depostion

I cleaned the chamber for 6 mins and seasoned for 1

Before top cap dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/75893969-F19B-4D94-B2CA-5100FCD014B1_2/l3axgcUQLu3gRi5GAJrkboHuUlyIfv4WMYyiayeU5lgz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/2833D1D4-9798-4869-A7EC-ECAC62FFBAD8_2/wwUYF9vE4kkAckY0fxYuLgE8Y7iYCMXNxj4aKNCEA3Iz/Photo%20from%20Library.jpeg)

Before second dep on different wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/CFABCD82-57EC-4607-BA85-F81E627B53FF_2/SQaXK9lBZ7vQeUxKEMwmYbAAcBp386SGx6WHarWGBX8z/Photo%20from%20Library.jpeg)

we do a 10 min clean and are going to season again for 1 min before doing the last wafer.

Before last dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/AD9FC982-62CC-4942-BCE3-B138D5DA33C1_2/O1rjwJCUjEGicQhqKkkJ710J4hrcg4Zs0LigcbNWrGEz/Photo%20from%20Library.jpeg)

Ellipsometery check

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/AD8314CB-BFDB-4A58-8146-5CABBE414B2C_2/Y5x7TzsNdMNxXhuyyYNNrTyZQLyBmdxUhQF1RfufCFUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/51F81777-BED3-4C09-842B-854804AD83E9_2/1T535tr221zbLCMCKSWdqfFo8fWaLAs2yVJXUHChywYz/Photo%20from%20Library.jpeg)

Just some misc notes about organization 

Below is the SVM box

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/EE52790F-8DE9-4174-86CE-74F26E94FD56_2/c4fhbfSdA0x8K937mBJO0bl34OcrFos6dSb0yzUOzIYz/Photo%20from%20Library.jpeg)

Middle three are SVM with oxide. Back are just SVM. Front is not fitting, but I suspect it’s 800 nm SRN3

### Lithography

Below is the thickness we expect

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/39765EB8-696B-422E-B025-6EE6EF423F34_2/xjqSPJUNdu6rQc1B7919rF1dYZIBAFNxWFpq9zTbUY8z/Photo%20from%20Library.jpeg)

So 1805 at 2000 should be good

we used 2000_8000_45 for spin coat, and 90 C for 1 minute to bake

Before exposure

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/26F58B49-91FC-4985-8D75-80609215C6E9_2/RQyCYp121boT5CEGKIjOpywGnpBvoHK9cOaWznQHnq0z/Photo%20from%20Library.jpeg)

We develop with recipe 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/50FF9FF1-05C4-4996-90A2-338E1E22E098_2/TlvLfxm5H6n6Cr0FekGSpD3LsYGNtVXuJgtyt7AQlrwz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/F90D3FBD-D369-4F56-B0A7-AB6BD1E59A5E_2/ZykS5rFh0zujkozFG3ly9d3SNE30ijhLp40pwAuXzb0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/4EA99637-B148-4741-8522-D7AD3BFBE793_2/79lXfLB0FP4YtvRZS7W5rv5gVnqS2RWOSu1SYzynyyQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/D70EE10F-457A-4638-B22B-0E4EE59A3B3C_2/jBdLPrsQiW4csu1afHwN1Slt3gZAMITCw3ICLyb2uFwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/C6D34564-4107-4891-9436-0B993B8A4EEB_2/iYxreUOn5tvgynmUIQMpNPmdcpFgoef76f5euMzdMNwz/Photo%20from%20Library.jpeg)

There is an obvious blur, but that could be from over exposure or bad MLA. I say we continue.  This goes to show we will have to be more deliberate about dose tests in the future, but the period should be right (which is most important).  And we should get qualitative feedback on what perturbation size is best. 

### Etching

We run 5 min pre clean on 81 and 100.

Before oxide etch season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/D4F6C4B6-31AD-4692-BFED-32450E1C4255_2/twgPxJ4jHBgxQuoaNndofOdW8kfbYE7oKP3lPlHHhZAz/Photo%20from%20Library.jpeg)

Before descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/162B2A8A-C475-42F6-A87F-9CD517529C97_2/XIohPmPxaSPox0yXvPzVWONwD9hgcg5V4dZbSRSu9s0z/Photo%20from%20Library.jpeg)

The He flow on the etcher seems fine

Profilometer for resist thickness

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/679E913A-C873-44E9-9994-DF38416ECAFB_2/qzTBg6rltxprgyHqQxCBMiJSOKk0RbPdQ1K4x1j4KyYz/Photo%20from%20Library.jpeg)

At 550, we will make it

As a note, before the etch below, we wiped off the edge bead (almost forgot this, as I am used to ASML doing it for me)

Before oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/64A85C13-DC6F-439E-A563-AC1D71337A88_2/4rPYYgdXt5Kp2uQNdoOnwSzsbUcPYoZvsg8zyWRv9MEz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/5672673B-1843-4E0E-B4E0-5C3E19DC2B56_2/NJomekL10ykN1mxpEm1424Eju0hJzlfmGwy7my6pC5sz/Photo%20from%20Library.jpeg)

He flow is a bit high, but we are getting a seel still. Settled closer to 4.7

We now run a 7 minute clean on 100.  Ontop EcoClean for the wafer

Before eco clean starts

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/60019502-1D32-4815-A1B0-38A80230FA54_2/q5Z5PxfrYEOarPaOMnQHGGaXhG3yiDWehVeTInxquckz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/54A036FC-7BC4-4D35-A805-5CFF9C1DFA9C_2/fAP164kuUs6yeJDA6Ux1SobU1GgsZZ9749maQLLOKr0z/Photo%20from%20Library.jpeg)

Before nitride season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/270E8B5E-298A-429C-AF77-2C1CADD3C6E6_2/NGob9dXyW2fVQU7LQi3Ovr6ar548TJ0YQwAgqSMSri8z/Photo%20from%20Library.jpeg)

Thickness of oxide

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/E8F69CC0-065D-4FD6-B75E-2E83FF3C1625_2/I87adkGYUGMgZESMYs7vCKdIsByRwOuhPMNkvgZRfZUz/Photo%20from%20Library.jpeg)

Basically spot on

We are going to skip piranha for now

Before nitride etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/40763F50-EB13-49F4-BB21-E97DA47D36B9_2/I9YRPR5J0kMuuFMyOfxCa8L89yr4eKTAULLNSNoY0XQz/Photo%20from%20Library.jpeg)

During nitride etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/70F46727-FD28-46C1-B46F-953692A6C23E_2/kD7yr3M8wSyXNVg3P3KAd7ViBkvV4CAxmSvycIHchM8z/Photo%20from%20Library.jpeg)

Thickness of nitride

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/EBA39223-D65E-43B4-A6E9-E6524AD4F0CB_2/FGgosFCo4LukKUESeyKR6eQWBPEO3BxdEYJLZxm5wE4z/Photo%20from%20Library.jpeg)

2.4 um, so we still had oxide

Images

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/44A9742C-7007-4186-8943-D90F6D613E2A_2/SCqRBifUybjJBPJ8o5cMv8EZ1fT4G6H3c7QvHQbpRQMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/E5AE33B7-5C62-4C71-9923-D281B1023546_2/qVOWoJFX1I60yJhwgxRvAQaLlOhPYyfWI8pmNunuqAYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/89BEAB2A-2D18-4D94-8D60-8C07B5F7E4C8_2/3p1P2EMxFitwyES08uD832GItRovlZDk4op2Ae93shkz/Photo%20from%20Library.jpeg)

I am not sure how nice our tapers are

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/78AFBFF9-D090-4E2A-952A-5CE24FAB4606_2/garvypTY77rKdekZMgFhD9ZkdHMCOMg3jyeNUZsugd0z/Photo%20from%20Library.jpeg)

Given that some of the tapers look a bit funny, I am going to cleave around them for some of the chipes.

I am going to anneal 2 non-cladding pieces, and all the cladded pieces

### Top Cap

We now run 6 min clean and 1 min season for oxide.  We will run 16 min dep to get ~2.5um of oxide

Before cap

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/5CD4D4E2-6EF2-4CA9-A01C-3FAF1A989C1B_2/lUdubNgzE2A0k52iMZEocg4JyTYnY2Zn89U2iSpWGLcz/Photo%20from%20Library.jpeg)

During RTA calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/8554BE36-292C-44BB-A8E4-AB79A2C9E3F2_2/ZO6FN2yYgRCsyZO8pn6nYSLc5JKIQhWcIbx2NKVx7wIz/Photo%20from%20Library.jpeg)

Image of non cladded waveguides with annealing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/6044E58E-E499-4615-85C4-7E12142C1487_2/NT69EDGhysXcyuRIQWqaZAEzWZdHtjUfPuiQhV6Uzvcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/1A7EFC19-D82D-4E8D-A2B5-EC6AA101BC13_2/ERTiTH07NCkL0W9J04lYFRDmLpYSeppFiDNsrSNIyG8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/938C8C19-1D7E-4A98-9530-4926318CFB0A_2/l1RFCgk8HELo2PmMFFhVyApptx7Lxf3n0UAtQltiBtYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/5631EFFD-E36C-4E59-AD53-A658F559A876_2/tUHf7bCT3dIMVXVliyFhbc2moakxXFfp57oEw3ayPeMz/Photo%20from%20Library.jpeg)

Now with cladding

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/8212EA0D-A656-4553-92DC-C39A040C0FD9_2/ReWiNjcHSi7Uxk4KoSUXRH5idFrXXJDPOUWDgujxvB8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/4201FD1E-7F2E-42C8-B2E1-3A958ED5C1B9_2/lCYK2xOqxRgunM3I9SEErSDiZz11vexA5JIOQ5wQYTMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/5CC3B3E2-FE52-466D-A268-9E1F7D0EF6DC_2/h1pjlncy2kK9E5b2hynKryVfuv90R8Uyl0GWlxn0mlsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/FA64D174-7C84-441A-B039-D60535F6C737_2/zVSZxgiMkZ3ezCAfZiQTbaBuPyKV82E3RfsoRRH7CJYz/Photo%20from%20Library.jpeg)

### Supplemental Dose test

We are going to run a followup-dose test to figure out what is the best dose, as I really should know the geometry

We will scan from 40 as the dose to 60.  We did 2000_8000_45, and 90C for 1 min.

Before starting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/1FBB858F-7C1A-4026-B5B9-0CFDACB45A57_2/5Gdqw6Oa6cHaFU6p3mXHhPhbfrFLeg0os0xcugbyOxgz/Photo%20from%20Library.jpeg)

We run this process on 1 um of thermal oxide wafer.  We did use optical focus for this, so that is one difference

Exposure starts in top left

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/654109BE-B0A1-4205-AFEF-B83206A0B408_2/IdhdpUiJirRtJSOjYaAk0afGfxAmafOQWN9WHhaP6tsz/Photo%20from%20Library.jpeg)

Second is on the row of 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/A55F36D9-F11B-48C9-998C-A101FF232702_2/qVyYM4gmSJMd9bZcxh3Obw6xAlAwuuCyGJOTJz5l9gQz/Photo%20from%20Library.jpeg)

So it scans across a row first, then does different rows 

We use program 4 to develop

Taper on top left

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/7C1D2129-7FFF-42D6-BBDA-1F7C9E40DD69_2/eqSidFQE6nBuCintVMVsgX9v5lgRoi4JnqTFt9UtGnsz/Photo%20from%20Library.jpeg)

Each division is 2um

5 by 8, period 4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/1CBF6899-3A26-4E19-B1FE-51249A866233_2/AiQnbBTlpxFeykpttcToSn5xY3p29Zy7P3HOkfuxEEkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/F23BFAD6-A095-4714-82AC-17694E82931E_2/w8CfF4pqbKybUzYFfp88WySAwxfhJHmmpiI0R5zjrxsz/Photo%20from%20Library.jpeg)

Third, top row

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/E9925B0E-8256-4AC6-8C81-DFC0A8058DBE_2/ZeSoYSxGuELVpoBYVieM1u7N6XH132iiQs2yYDciZsYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/EF6BE03B-FC36-4007-BE74-A1A559F27CAC_2/BBYB4xgoDmWsuTSC3xIxHQzGlXlEU10EeSw0kncRoHQz/Photo%20from%20Library.jpeg)

Taper

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/7EB6BD61-8236-4037-818A-62C6EE260595_2/B4fEPRQRqgCnoxxZIDwhWJsFyesuhqftZMeQ7rWmUzoz/Photo%20from%20Library.jpeg)

This taper is def a bit less then 2um

Bottom first

Taper

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/673F6820-F3B2-45BE-9D19-F482C9DC3E28_2/1l2rNXyyg16Yb9TxgheG7wxDfOyPlu3A8pJ3LKyZSzcz/Photo%20from%20Library.jpeg)

Crystal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/459B4593-0A5D-47DA-8635-75C6D24AC0E9_2/wSugNiWiQ4iK4xzuSvXj8VibAdDbqhoOQRxjD0X30Mgz/Photo%20from%20Library.jpeg)

Further over (largest dose)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/A89FC894-AB4A-4667-B7C2-5704E059EC24_2/8VURe306p28c7FxmjVr4qAJEQzRR0PrzeWj3wr3WWVoz/Photo%20from%20Library.jpeg)

We might have had functional tapers, but they would have been small (and this was was optical, not pneumatic, so that is also a difference)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/87BBD1AD-F074-452E-921C-88C8062E3C5F_2/YpNCqlgfsvUTqx4EWbIobEU0P981zUlNqMw8aCIJS8Yz/Photo%20from%20Library.jpeg)

## Testing

Skip the first 20 waveguides at the bottom, they are straight

Next couple vary length.  We should skip those for now too.  there are 16 of those

Using the camera, below is what

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/FF108451-D6DE-4B42-A7B6-5951C9D285A2_2/5FLbr1stcXIBvFGoBOVwDG8UUUOdKMxRfdZ28VGFpf4z/Image.png)

With a finer scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/5C87B993-C75B-4A7B-9111-E3E9035C7B52_2/xW73Tr1btxh656S2YN70QUS4UR3e0lnP5yKKeoKnYyIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/D02E93A9-2421-4F52-8F84-A9F77B4A68B1_2/xaFqRpPVPr7t9yddEG5IbFyKsQ22vxJzgC0f4Fs19Ucz/Image.png)

This is a touch annyoing, as I don’t see an obvious discontinuity.  Then again, this background has always been a problem.

Some issue is the stopband (With the worse index contrast and lower resolution) is our stop band could be really really small.  Again, we are looking for a distinct drop in tranmission, something that looks discontinuous.

If I were thinking of what could have gone wrong, below are some hypothesis:

- Because we are over-exposed (and the MLA struggles to resolve small features anyway) we truly might have very small features at the spatial frequencies we want.
- MLA increases resist roughness, which increases loss (this point I think goes undermentioned, but we only saw a maximum of 100 uW instead of several mW.  Meaning, at least a factor of 10 higher loss.  I suspect we need smaller perturbation sizes, as we were not able to see any light in the 5-8 um devices.  I suspect that using 5-6 um is probably safer)
- Our waveguides could be a lot narrower than we suspect, which could cause the dispersion to be much different than suspected (though we did test several periods, and we know that we have a decent amount of room for wiggle room with index).

We generally see that people use first-order diffraction, so it is perhaps posible that getting higher-order terms to work for us was just going to be too hard.  We should still investigate second or third order diffraction, as they are only removed from the fundamental period by 1/2 or 1/4.  Basically, they should be noticable.  I am generally less willing to believe that we were super off on the expected period, as most periods I see only are very close to what I used.  The size of our perturbation was not insane either, but most people use DBR structures that are much shorter than ours.  I guess it is possible that our DBRs were too effective, but I kinda doubt that.

We should take a picture of our waveguides with no cladding under SEM.  I want to see our exact feature size and look at the dose test as well.  I don’t think we will be able to use the MLA to get these made.  On our ASML mask, we should also leave a section for normal periodic tapered waveguides, as that is just a nice experiment to include.  

For the next fab, I would indeed try to use the ASML.  I would only have two waveguides of each type and I would make the photonic crystals much shorter.  Of course, the issue with this is that the dispersive section might be so short that we hardly notice on the nonlinear scan.  I could just see this being hard is all.  We will of course want to use the EDFA, but in some sense using higher-order diffraction was a saving grace for this.

Lets try something where we vary the length of our waveguides.  We should try something where we use waveguides that are 10 um of perturbation, 50um of perturbation, 100 um of perturbation, 500 um of perturbation, 1 mm of perturbation, 5 mm of perturbation, and 1 cm of perturbation.  We will make waveguides default 5um wide just to be safe.  I would also choose to make waveguides either 6.25 um wide or 7.5 um wide for the larger sections.  We can otherwise very the grating between 3.8um and 4.3 um (with iterations of 0.1 um).  I will double check the period length later.

Below are the SEM images.

Narrow = 5, Wide = 8 (I think the period for all of this is about 4)

![Etched_N5_W8_P3.900.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/A2D4FEC7-2605-4D31-84E7-E15F2988912A_2/CtiNJ48vxPmfnaXah6rwhZEjcH1159qOPUVZyJIgKikz/Etched_N5_W8_P3.900.tiff)

![Etched_N5_W8_P4.501.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/30D5E331-31A4-44F3-BAFD-6A2C5C2AFA97_2/Psar5L6KEej75yyCvYXQvqtIeyqnGgFoUFWFesQxYHwz/Etched_N5_W8_P4.501.tiff)

![Etched_N5_W8_P4.502.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/B55D4E5C-BF08-4004-A55B-2695B4C7A4A1_2/b3Y1yP3Zbs7aYHkhC8BXuQHkqbo4gsn1Od94yzED4UUz/Etched_N5_W8_P4.502.tiff)

![Etched_N5_W8_P4.503.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/09C2F8E7-0664-4CA2-8251-ECE1A67E425B_2/xV0DG3rDhDWrxO4yfRa6Pf0yU4NEgO5768FdxPetszMz/Etched_N5_W8_P4.503.tiff)

![Etched_N5_W8_P4.504.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/2A2F0581-4E39-420A-8837-642436DD8379_2/6HG2BSQLJBRm9PpviPCwYAUZ1szeVel0GpNEZVyNekYz/Etched_N5_W8_P4.504.tiff)

Narrow = 4, Wide = 5

![Etched_N4_W5_P4.507.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/2E8F3B00-5EE1-4D5D-BBA4-5809334F597C_2/egBUvmyJMy22ENbnU7DyQsRlCrjq1IPQpcylxxQFc60z/Etched_N4_W5_P4.507.tiff)

![Etched_N4_W5_P4.508.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/BFE8B332-5FCE-48AE-AFB8-3EAF0953A0EA_2/68WUOCKH9zE6gQuJoy0JHE8A5l1LjFhOPu4iCqV4drgz/Etched_N4_W5_P4.508.tiff)

Sidewalls of etched devices

![Etched_sidewall10.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/63EE9608-6483-4C30-A734-07C43E0DF161_2/76QDd9y6O7EYjomjIna06W41omzQBvUNcEfbYmHIRE4z/Etched_sidewall10.tiff)

For the lithography test, everything seemed to be the same size.  Nonetheless, below are the dimensions for the things we exposed

![Litho_7_N5_W8_P418.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/4228EB3C-4F2C-4323-9160-BDE568AC7F6D_2/k43LQRuoeuw3yQEVG7lcxFJXY8dx3voWLPngyQpXxKIz/Litho_7_N5_W8_P418.tiff)

![Litho_7_N5_W8_P419.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/E3E319A4-93F2-4DA6-BECD-B87DD51AFD47_2/iMxXqUngxSsNf3XBzCr777ybu7wsEyZcn5YnCO1arQEz/Litho_7_N5_W8_P419.tiff)

And sidewalls (though they are a bit more blurry)

![Litho_Sidewall22.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/4BF5BCF5-354F-49B2-9148-720687236CCA_2/Mx0UQPAtLv0rWxfNxr60bron0SISqK01d7OkurfvuVUz/Litho_Sidewall22.tiff)

![Litho_Sidewall23.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/603129C4-9A84-4F10-8237-6EAB2B623CA3_2/CXFrxoCrjctPXEfwoT0TGLJ99NRBMhYhsxkXQZGF1GYz/Litho_Sidewall23.tiff)

![Litho_Sidewall24.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7277444A-3193-4640-807B-8C7E67D3BB45/67DAB133-E9BE-4C6B-A84A-5123468C76A2_2/mJn9iyas482WPC3PxycIR9tIF6EkBlkAAXfbAF9BMnIz/Litho_Sidewall24.tiff)

A lot of the roughness I see after the etch I don’t see on the resist.  So our sidewalls are pretty shitty, and this is probably because we are etching so far down.

So now we really want to focus on designing the new GDS.  Firstly, Mandar had a really nice suggestion that we ought to have a wide input coupling region, but then have short tapers.  This should really help us mode-filter.