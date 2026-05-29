---
type: craft-export
title: "2024-12-06 final dc ln device for 800 nm with annealing b38"
craft_document_id: 2B9DDD52-174D-4392-AB41-FCA949D90DDB
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-12-06 final dc ln device for 800 nm with annealing b38
Given our new measurements with B38 annealed, I am going to update our simulations for this type of device just to make sure everything looks ok.

A general pdf of the code is below, but I will also include some highlights

[2024-12-6 B38 DC LN Device.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/5542649E-CA0A-4547-82E2-FDFF5268C9B7_2/nUKDqT5no47yIJ9g4wLGQD1gGzOM5FHJtPCMr57ObQAz/2024-12-6%20B38%20DC%20LN%20Device.pdf)

Modulation efficency: 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/E1594777-3217-4F1A-A5D7-E77A14AD19AF_2/6dylgpVs8yoXFFsuo3PAZfFGGP7TBIsfydMaHPMMKO8z/Image.png)

Substrate loss

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/8FB5C315-8A00-4652-9236-E4E091034728_2/kWxqZY960KFCsTSg4C2NByq5H9xM9i4rREhtzhxlhZkz/Image.png)

Delta_n perfomance:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/C9BC7C48-88B7-4FAB-8A9B-2984961B2298_2/ebytUNijq4gUGpfJtUS39yxkedAbgxt9MLU6gCOFF1gz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/ED695F13-6685-4655-8DAF-5F62502BA04B_2/aPxDR1IRBd3fxsLxGO6zyrQHMkw5q1ItsLyX0HiVmBcz/Image.png)

Steady state field

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/E1FF2F42-B706-48E6-8212-91307ADD1CCB_2/a9w6Azq79WqiFCzdp8cyZK4fmSVCd0AlvaqPoh1b7Mwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/57D6CAA2-1B30-4187-8355-57C34BB1230E_2/klt7Znh2BtnCrbYImcq4lbHhbyWss588IybiByql3ewz/Image.png)

A generally interesting thing to note is that the max field in DON occurs in bright state, not dark state.  So that is what I am plotting above.  Because it is more conductive than SRN, it seems to ahve roughly constant field

Transient solution (SRN constrast = 300, volt = 545)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/CCB79A10-CC26-4675-AD24-3A20B3BEA7A1_2/xHBD76yDaTsweGNfpRkxoPi9WLgB97vq7rVpEDcLrycz/Image.png)

Below is the relevant plot for DON breakdown (just trust that SRN is fine)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/43f26339-bc92-458a-1caa-05a83bc2dc0a/y9hkU1terdlt59uNBgYQr1iBqLyA5eYMR59kgkEHsOAz/Image.png)

I don’t love how close some of the capactive regions of DON are getting to breakdown, but oh well.  My feeling is that the permitivity could be higher than I am guessing.  We also don’t perfectly know the LN conductivity, which could mean we are lower.  I am a bit scared the SRN won’t have as much contrast as I would like, but that can be solved with a more intense top imaging setup.